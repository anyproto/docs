# Sign-in & Google SSO

Members sign in in one of three ways:

* **Sign in with Google:** with a Google Workspace or personal Google account.
* **Email code:** enter your email, then the 6-digit code we send you.
* **Continue with SSO:** through your company's identity provider, if your organization has set up [custom SSO](custom-sso.md).

{% hint style="info" %}
There's no Microsoft sign-in button yet. To use Microsoft Entra ID, set it up as a [custom SSO provider](custom-sso.md).
{% endhint %}

Use the method your account already uses. If you try an email code on an account that uses Google, Anytype asks you to sign in with Google.

## Google Workspace auto-join

Auto-join lets people with a Google Workspace account on your domain join your organization without an invitation.

* **When it's on:** organizations created with a Google Workspace account start with auto-join for the owner's domain. Organizations created with a personal Google account or email start without it.
* **Role:** people who join this way get the **Member** role. In **Members**, the **Joined via** column shows **Google auto-join**.
* **Invitations:** if someone on the domain has a pending invitation, they join with the invitation's role instead.
* **Existing members:** their email accounts on the domain are linked to Google the next time they sign in with Google.
* **New email sign-ins:** new people on the domain who try an email code are sent to Google.
* **Removed members:** can't rejoin through auto-join. They need a new invitation.

### Change the auto-join domain

Only the owner can change this. Admins can see it but not edit it.

1. In the Admin Console, go to **Settings** → **Google & Microsoft**.
2. Enter the new **Workspace domain** and click **Save**.
3. Confirm the change.

{% hint style="info" %}
Once you save a [custom SSO](custom-sso.md) connection, this tab becomes read-only and shows **Managed by your custom single sign-on**.
{% endhint %}

## Confirm it's you

Some changes, such as sign-in settings, need a recent sign-in. If you see **Confirm it's you**, enter the 6-digit code sent to your email.

## Sign-in problems

<details>

<summary>"Your access to this organization has been revoked"</summary>

An owner or admin removed you from the organization. Ask them to invite you again.

</details>

<details>

<summary>"This email already has an account that signs in with Google"</summary>

Your account uses Google, or your email domain uses Google Workspace auto-join. Click **Sign in with Google**.

</details>

<details>

<summary>"Your organization requires single sign-on"</summary>

Your email domain uses your organization's SSO. Click **Continue with SSO**.

</details>

<details>

<summary>"Your organization's free trial is full"</summary>

The trial has reached its member limit. Ask the owner, or an admin with billing access, to add a payment card.

</details>

<details>

<summary>"You have multiple pending invitations"</summary>

Several organizations have invited you. Open the invitation email from the one you want to join and click its link.

</details>
