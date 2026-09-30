# Custom SSO (OIDC)

Connect your company's OpenID Connect (OIDC) identity provider so people sign in with their work accounts. The Admin Console has presets for:

* Okta
* Microsoft Entra ID
* Keycloak
* Authentik
* Zitadel
* Authelia
* Other OIDC

Set up SSO in **Settings** → **Single sign-on**. Only the owner can change it. Admins can view it. If Anytype support set up your connection, contact support to change it.

{% hint style="warning" %}
Activating SSO needs a paid plan. During the trial you can verify domains, connect your provider and run tests. To activate, click **Go to billing** and subscribe.
{% endhint %}

Setup has five steps: **Domains**, **Identity provider**, **Test sign-in**, **Activate** and **Enforce**. Each step unlocks when the previous one is done.

## 1. Verify your domains

Prove you own each email domain with a DNS TXT record.

1. Enter your domain, for example `acme.com`, and click **Add domain**.
2. At your DNS provider, add a TXT record with the **Host** and **Value** shown. The host looks like `_anytype-challenge.acme.com`. If your DNS provider adds the domain for you, enter only `_anytype-challenge`.
3. Click **Check now**.

DNS changes usually appear within minutes but can take up to 48 hours. To check the record yourself, run the **Self-check** command in a terminal:

```
dig TXT _anytype-challenge.acme.com +short
```

You can add up to 10 domains. You can't add public email domains such as `gmail.com`, or a domain another organization has already verified. If another organization claimed your domain, email [business@anytype.io](mailto:business@anytype.io).

## 2. Connect your identity provider

1. Choose your provider's preset. It shows setup steps for that provider.
2. In your identity provider, create a web application with the values under **Add these in your identity provider**:
   * **Redirect URI**
   * **Scopes:** `openid email profile` (Okta and Authelia also add `groups`)
   * **Grant type:** Authorization code
3. In the Admin Console, fill in **Paste from your identity provider**:
   * **Display name:** shown on the sign-in button, for example "Acme"
   * **Domains:** the verified domains this connection covers
   * **Issuer URL:** a public `https://` address
   * **Client ID** and **Client secret**
4. Click **Save** and check the **Identity provider check** result.

{% hint style="info" %}
For Microsoft Entra ID, use your tenant's issuer: `https://login.microsoftonline.com/<tenant-id>/v2.0`. The `common` issuer doesn't work.
{% endhint %}

### Provisioning

* **Automatic sign-up (JIT):** on by default. New people on your domains join when they first sign in through your provider. Turn it off to require an invitation for new people.
* **Default role:** the role for people who join automatically. **Member** by default, or **Admin**.

### Advanced

Under **Advanced** you can change scopes, PKCE, claim mapping, **Token endpoint auth method** (`client_secret_basic` or `client_secret_post`) and **Email trust**.

**Email trust** starts at **Preset default**:

* Keycloak, Zitadel and Other OIDC require the provider to mark the email as verified.
* Okta, Microsoft Entra ID, Authentik and Authelia trust any address on your verified domains.

You can override this with **Require the IdP's email_verified** or **Trust addresses on my verified domains**.

### Replace the provider

After saving, you can't edit the issuer or client ID. To change them, click **Replace identity provider**, then **Delete and set up again**. Set up, test and activate the new connection. If SSO was enforced before, turn enforcement on again. Members keep their accounts and are linked to the new provider by email when they next sign in.

## 3. Test sign-in

Click **Run test** and sign in in the new tab with an account on one of your domains. Finish within 10 minutes. The test doesn't create accounts or sessions.

Run the test again after you change the client secret, the provider preset or anything under **Advanced**.

## 4. Activate

Before you activate, the page shows how many of your members use these domains. They're linked to SSO on their first SSO sign-in.

Click **Activate**. When someone enters an email on one of your domains, the sign-in page shows **Continue with {display name} SSO**.

## 5. Enforce (optional)

Turn on **Enforce single sign-on**, check the affected members and confirm. Members on your domains then sign in only through your provider.

The owner is exempt by default and can still use their other sign-in method, so a broken provider can't lock you out. Anytype records each of these sign-ins and sends an email about it.

To stop enforcing, turn the switch off and confirm. Members can use their other sign-in methods again.

Saving a new client secret, a different provider preset or changes under **Advanced** turns enforcement off. The button then reads **Save and turn off enforcement**. Run a new test, then turn enforcement on again.

## Disable or delete the connection

In the **Danger zone**:

* **Disable:** nobody can sign in through the connection until you activate it again.
* **Delete connection:** removes the provider settings and SSO links. Your domains stay verified.

Members who signed in only through SSO then use email codes.

To remove a domain, first uncheck it under **Identity provider** and save. Then remove it under **Domains**. To remove the last domain, delete the connection first.

## What members see

Members enter their work email and click **Continue with {display name} SSO** to go to your identity provider. People on your domain who aren't in your organization can click **Not part of {display name}? Sign in with email**.

## Troubleshooting

<details>

<summary>"Not part of this organization"</summary>

The account's email domain isn't in this SSO connection. Sign in with an account on one of the connection's domains.

</details>

<details>

<summary>"You're not a member yet"</summary>

Automatic sign-up is off and the person hasn't been invited. Invite them from **Members**, or turn on **Automatic sign-up (JIT)**.

</details>

<details>

<summary>"Email not verified"</summary>

The provider didn't send an email address, or didn't mark it as verified.

* Missing address: check the `email` scope and **Claim: email** under **Advanced**.
* Not verified: if your provider never sends `email_verified`, set **Email trust** to **Trust addresses on my verified domains**.

</details>

<details>

<summary>"Sign-in session didn't match"</summary>

The sign-in finished in a different browser from the one it started in, or cookies are blocked. Try again in the same browser with cookies allowed.

</details>

<details>

<summary>"Couldn't reach the sign-in service"</summary>

Anytype couldn't connect to your identity provider or load its settings. Check that the provider is online and the issuer URL is correct.

</details>

<details>

<summary>"We couldn't read the OpenID configuration at this issuer"</summary>

Check the issuer URL and that its OpenID configuration is publicly reachable. For Entra ID, use your tenant's issuer, not `common`.

</details>

<details>

<summary>"Your identity provider rejected the client ID, secret or authentication method"</summary>

Check the client ID and secret. Under **Advanced**, set **Token endpoint auth method** to the one your provider uses.

</details>
