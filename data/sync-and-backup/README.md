# Sync & Backup

Anytype is built on local-first principles, combining the seamless experience of modern cloud applications with the privacy, security, and absolute ownership of local software.

Everything you create lives locally on your devices, encrypted with keys that only you control. Our infrastructure handles background syncing and backups automatically, so you retain full ownership of your data without compromising your sovereignty.

## Why it matters

In the past, local software meant complete ownership and privacy — what you did was your business, and nobody else's. But it came at a cost: collaborating with others was a huge frustration.

The internet solved that. Cloud technology let us collaborate in real time — but along the way, we gave up our privacy, security, and ownership to the apps themselves.

With Anytype, you never have to choose. You retain complete ownership and control of your data at all times, while still using the internet to sync across devices and collaborate with others.&#x20;

It's the best of both worlds: local ownership meets cloud collaboration.

## How It Works

At a high level, Anytype gives you complete control in three ways:

{% stepper %}
{% step %}
### Everything is local

All your content is stored locally on your device, and even your access keys are generated on your own hardware. This means an offline-first experience: the app always works without an internet connection, protecting you from downtime, lockouts, and vendor lock-in.&#x20;
{% endstep %}

{% step %}
### Sync is end-to-end encrypted

Before any data leaves your device, it's encrypted so that only your key can unlock it. The Anytype Network acts as a "blind orchestrator" — relaying updates across your devices without ever being able to view or access your content. Even if your encrypted data were intercepted, even the world's most capable attackers couldn't break in. This is verifiable through Anytype's open codebase that's constantly inspected by the public.&#x20;
{% endstep %}

{% step %}
### Recovery is built-in

To ensure you never lose your data, the Anytype Network keeps an encrypted remote backup. Only your private key can decrypt and restore it to a new device — nobody else, not even Anytype, can access your encrypted data. Being in complete control also means you are fully responsible for your [keys](../../basics/key.md) to access and recover your data.&#x20;
{% endstep %}
{% endstepper %}

Anytype was built to be a convenient safe haven for your digital life. To learn more about how this works for collaboration, please [see here](../../collaborate/collaboration.md).&#x20;

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs E2EE Sync.gif" alt=""><figcaption></figcaption></figure></div>

## Anytype Network

By default, everyone joins the Anytype Network — also known as local-first sync. Every user gets a remote backup node provided by Anytype, with free storage that can be increased with a membership.

Objects and other content don't count against this limit, so you can always create and edit documents without restriction and will never lose access to your data. Only files — like images and videos — count toward the limit. If you go over it, you'll see a warning and can request more storage. You can keep using the app even past your limit; the only effect is that new files stop syncing between your devices.

While using local-first sync on the Anytype Network, you can go fully offline and/or sync over your local network peer-to-peer. Think of the Anytype Network as a backup system: you can always work offline and sync locally, and once you're back online, the network will sync and hold a remote backup for you.

#### Where are the remote backups based?

Our infrastructure is hosted on dedicated servers in data centers within the European Union. The domains we use for our Anytype network are:

* For syncing: `*.anyclub.org`
* For our analytics: `*.anytype.io`

## Other syncing modes

Anytype also supports two alternative modes:

* [Self-host](self-host.md) — use your own infrastructure to host and sync your Anytype data.
* [Local-only](local-only.md) — don't sync through any server at all; your data stays on-device.

We recommend sticking with the default Anytype Network for local-first sync, and only switching to these modes if you have the technical expertise to manage them.

### How to switch back to Anytype network

We strongly recommend using dedicated identities for each network. If you are switching from a Self-hosted network, export all your channels, and import them into a new identity after switching the network mode.

Please note that all your devices should be manually switched to Anytype Network mode.

#### Desktop

1. Log out from your current identity.
2. On the onboarding screen, click a gear icon in the top right corner.
3. In the “Network” field choose the “Anytype” option.
4. Click the “Save” button.
5. Create a new identity or log in with an existing one.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/image (43).png" alt=""><figcaption></figcaption></figure></div>

#### Mobile

1. Log out from your current identity.
2. On the onboarding screen, click a gear icon in the top right corner.
3. Click on “Anytype” in the “Networks” sub-menu.
4. Create a new identity or log in an existing one.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Screenshot_20240411-104810_Anytype2.png" alt="" width="375"><figcaption></figcaption></figure></div>
