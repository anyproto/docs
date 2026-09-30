# Get Started

## Create an organization

1. Open the [sign-up page](https://business-api.anytype.io/admin/start).
2. Click **Sign in with Google**. Or enter your email, click **Continue**, enter the code we send you and click **Verify**.
3. If asked, enter an **Organization name** and click **Create organization**.
4. If asked, complete billing setup. Otherwise you go straight to the welcome page.

What happens depends on the account you use:

* **Google Workspace account** (for example `you@acme.com`): if your domain has no organization yet, Anytype creates one named after the domain and makes you the owner. Other people with a Google Workspace account on your domain then join automatically. See [Google Workspace auto-join](sign-in/README.md#google-workspace-auto-join).
* **Personal Google account or email:** you name the organization yourself. People join only when you invite them.

Once you're set up, the welcome page walks you through three steps: install the app, sign in, invite your team.

## Install the app

Open **Download Anytype** in the Admin Console. The main button picks your operating system. On macOS it defaults to Apple Silicon, so pick Intel under **Other platforms** if you need it.

* **macOS:** Apple Silicon and Intel
* **Windows**
* **Linux:** AppImage, `.deb` and `.rpm`
* **iOS:** App Store
* **Android:** Google Play

Sign in to the app with the same account you used to create the organization.

## The Admin Console

Owners and admins manage the organization at [business-api.anytype.io/admin](https://business-api.anytype.io/admin/). The sidebar has:

* **Dashboard:** organization name, number of active members and spaces, your role
* **Members:** invite people, set roles, revoke access. See [Members](members.md).
* **Spaces:** create spaces and choose who's in them. See [Spaces](spaces.md).
* **Settings:** organization, billing and sign-in settings. See [Organization Settings](org-settings.md).
* **Download Anytype:** the apps for every platform

## Invite your team

Open **Members**, click **Invite member**, enter an email, choose **Admin** or **Member** and click **Send invite**. The person gets an email and joins when they sign in with that address. See [Members](members.md#invite-members).
