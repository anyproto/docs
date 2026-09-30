# Members

Owners and admins manage people in **Members** in the Admin Console. The list shows each person's role, status and how they joined, for example **Invitation**, **Google auto-join** or **SSO auto-join**.

## Invite members

1. Open **Members** and click **Invite member**.
2. Enter the email and choose **Member** or **Admin**.
3. Click **Send invite**.

The person gets an email with a link. They join by signing in with the invited address, using Google, your organization's SSO or an email code. Invitations expire after 7 days.

Invitations that haven't been accepted are listed under **Pending invitations**, where you can **Resend** or **Revoke** them. They don't use a seat.

You can't invite:

* an email already used by an account in another organization
* an email on a domain that belongs to another organization's SSO

{% hint style="info" %}
The number of invitation emails is limited, and resends count too. The limit is lower during the trial. If you reach it, the Admin Console tells you what to do.
{% endhint %}

## Change a member's role

Open a member and choose **Admin** or **Member**. You can't change your own role or the owner's role.

## Revoke access

Open a member, click **Revoke access** and confirm. They're signed out, can't sign in again and are removed from the organization's spaces. You can't revoke the owner.

To let them back in, invite them again.

## Who counts as an editor

You pay for editors: members who can edit in at least one space. Members who can only read are free.

New members are added to every public space with that space's default permission. A public space with **writer** as the default makes every new member an editor. See [Spaces](spaces.md).
