# FAQ

<details>

<summary>Is Anytype for Business end-to-end encrypted?</summary>

* **Anytype-hosted (cloud):** no, it isn't zero-knowledge. We run the auth node that stores your team's encrypted keys, so we're technically able to access your content. Our policy is that we never do.
* **Self-hosted (coming soon):** your company runs the auth node, so the keys stay with you and encryption is end-to-end within your company.

In both cases, content is encrypted on your device, in transit and at rest. We don't use it for AI training or advertising, and we don't share it with third parties. Any Association is based in Switzerland and follows Swiss data protection law.

Personal Anytype is always end-to-end encrypted and zero-knowledge.

</details>

<details>

<summary>How do I get zero-knowledge encryption with team features?</summary>

1. **Use personal Anytype and share spaces between accounts.** You get no SSO or Admin Console, but nobody else holds your keys. This suits small or technical teams.
2. **Self-host Anytype for Business** (coming soon). You get SSO, the Admin Console and member management, and the auth node runs on your servers.

</details>

<details>

<summary>Can I move my personal Anytype data to Anytype for Business?</summary>

Yes:

1. Transfer ownership of your spaces to your new organization account.
2. Invite your team from the Admin Console.
3. Ask them to rejoin the spaces.

Your content stays the same. Only ownership and access change.

</details>

<details>

<summary>Which platforms are supported?</summary>

Windows, macOS, Linux, iOS and Android. Owners and admins manage the organization in the web Admin Console.

</details>

<details>

<summary>Can I sign in with Microsoft?</summary>

There's no Microsoft button yet. The owner can connect Microsoft Entra ID as a [custom SSO provider](sign-in/custom-sso.md). Activating it needs a paid plan.

</details>

<details>

<summary>Who pays for a seat?</summary>

Editors: members who can edit in at least one space. Members who can only read are free. Pending invitations don't use a seat.

</details>

<details>

<summary>What happens to our data if we cancel?</summary>

It stays on your devices. We keep content stored on our servers until you ask us to delete it. See [Cancelling](org-settings.md#cancelling).

</details>

<details>

<summary>Can we self-host?</summary>

Not yet. Self-hosting will cost €300 per month for any team size. Email [business@anytype.io](mailto:business@anytype.io) to get notified and receive the technical requirements.

</details>
