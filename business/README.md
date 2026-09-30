# Overview

Anytype for Business is a separate Anytype app for teams. It adds:

* **Sign-in with your work account:** Google, your company's identity provider (OIDC), or an email code.
* **Central member management:** owners and admins add and remove people, set roles and control access to spaces.
* **The Admin Console:** a web app at [business-api.anytype.io/admin](https://business-api.anytype.io/admin/) for managing your organization.

The app runs on Windows, macOS, Linux, iOS and Android. It has its own download and its own accounts, separate from personal Anytype. Get it from **Download Anytype** in the Admin Console.

{% hint style="info" %}
There's no Microsoft sign-in button yet. You can connect Microsoft Entra ID as a [custom SSO provider](sign-in/custom-sso.md).
{% endhint %}

## Why it's a separate app

Personal Anytype is zero-knowledge. Your keys stay on your devices, and nobody else can read your content, including us.

In Anytype for Business you sign in with your work account instead of a recovery key. To make this work, a service called the **auth node** stores your team's encrypted keys and gives your key to the app after you sign in.

* **Anytype-hosted (cloud):** we run the auth node, so we're technically able to access your content. Our policy is that we never do.
* **Self-hosted (coming soon):** your company runs the auth node on its own servers and controls the keys. Email [business@anytype.io](mailto:business@anytype.io) to get notified.

One app can't offer both models without weakening privacy for personal users, so they're kept apart.

## Roles

| Role | Can do |
| --- | --- |
| **Owner** | Everything admins can, plus SSO setup, Google Workspace auto-join, the Local API policy and cancelling the subscription. Each organization has one owner. |
| **Admin** | Invite and remove members, make members admins, create spaces and manage who's in them. Manage billing unless the owner turns this off. |
| **Member** | Use Anytype, work in their spaces and join the organization's public spaces. |

Space permissions (Reader, Writer, Admin) are separate from organization roles. See [Spaces](spaces.md).

## Pricing

€20 per editor per month, or 20% less with annual billing. An editor is anyone who can edit in at least one space. Members who can only read are free.

New organizations start with a free trial. Cancel within the first 30 days for a full refund. See [Billing](org-settings.md#billing).
