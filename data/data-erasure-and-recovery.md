# Data Erasure & Recovery

You are the only person who holds the [Keys](../basics/key.md) to your data and can manage it.

## Delete your Vault / Account

Anytype cannot access your data or verify your identity in any way. To delete your data, you must do so yourself through the app.

1. Go to your [Vault Settings](../settings/vault-settings.md) by clicking on your profile picture in the Sidebar.
2. Click on **Login Key** in the menu on the side.
3. Click on **Delete vault**.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Delete.jpg" alt=""><figcaption></figcaption></figure></div>

## Deletion Process

1. **Export a backup** — [Exporting](import-and-export/) entire Channels is the easiest option.
2. **Cancel deletion** — You have 30 days to cancel the deletion process. After that, your Vault is deleted permanently, and you can no longer sign in.
3. **Delete from other devices** — All data is stored locally on Anytype. If you are logged into multiple devices, you will need to delete your data from those apps by uninstalling them.

{% hint style="danger" %}
**After your Vault/Account has been deleted, it will no longer be able to be recovered.** Ensure you are certain before triggering deletion.
{% endhint %}

## Recovering your Vault / Account

Your [keys](../basics/key.md) are generated locally on your device, so Anytype never has access to your Vault/Account. And because account creation doesn't involve an email or password, we have no way to verify who the rightful owner of an account is. In short: if you lose your Key, we cannot restore access to your account.

#### What can I do if I can't access my Vault?

If you have signed in to Anytype on multiple devices, your [Key](../basics/key.md) is available on each device. Open Anytype on another device, then navigate to [Vault Settings](../settings/vault-settings.md) to obtain your Key. Use it to sign in again.

#### What if I can't delete my Vault?

If you are unable to retrieve your Key to access your Vault, Anytype is unable to delete your account for you because we have no way of identifying it correctly with your identity. Your Vault will remain encrypted on our backup nodes without anybody being able to access it.

{% hint style="danger" %}
**Anytype cannot recover a lost Key.** Save multiple copies of your Key using a secure method.
{% endhint %}
