# Organization Settings

Open **Settings** in the Admin Console. Which tabs you see depends on your role:

* **Org:** name, Local API, billing access and access for new members
* **Billing:** subscription and payments. For the owner, and admins with billing access.
* **Single sign-on:** [custom SSO](sign-in/custom-sso.md)
* **Google & Microsoft:** [auto-join](sign-in/README.md#google-workspace-auto-join) through Google Workspace or a Microsoft tenant

## Local API

The [Local API](../features/integrations/local-api.md) lets apps and scripts on a member's computer read and edit their Anytype data. Examples are the MCP server and Raycast.

To block it for everyone in your organization, turn on **Disable local API** in the **Client API** card on the **Org** tab.

* **Default:** off. The Local API is allowed.
* **Who can change it:** the owner.
* **Scope:** the whole organization. You can't allow it for some members only.

## Billing access

**Admins can manage billing** lets admins subscribe, update the card and download invoices. Only the owner can turn this on or off, and only the owner can cancel.

## New members

**New members can edit in General** sets the access people get in the General space when they join. Existing members keep their access. Owners and admins can change it.

This only affects General. New members still become editors if a public space gives them **writer** access. See [Spaces](spaces.md#public-spaces).

## Billing

The **Billing** tab shows the days left in your trial or your renewal date. It also shows your paid seats and editors. Click **Subscribe** to start paying, or **Manage billing** to update your card or download invoices. Payments go through Stripe.

* **Price:** €20 per editor per month. Annual billing is 20% cheaper. Members who can only read are free.
* **Trial:** you aren't charged until the trial ends. During the trial, the number of members and invitation emails is limited. Add a card to raise the limits.
* **Refund:** cancel within the first 30 days for a full refund.

### Missed payments

If the trial ends without payment, you can't create spaces or send invitations until you pay. If a renewal payment fails, you see a warning first while payment is retried. The owner, or an admin with billing access, clicks **Complete payment** to fix it. Other members see a message asking them to contact the owner.

### Cancelling

Your data stays on your devices. We don't delete content stored on our servers when you cancel. You can subscribe again later, or email [business@anytype.io](mailto:business@anytype.io) to have it deleted.
