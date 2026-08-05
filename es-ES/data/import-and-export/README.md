# Import & Export

You can import content into your spaces and export it at any time.

{% hint style="warning" %} Available on desktop only. {% endhint %}

## Import

1. Go to your [Channel Settings](../../settings/channel-settings.md).
2. Click on **Import** in the side menu.
3. Based on the type of content, choose your option.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Docs Import.jpg" alt=""/><figcaption></figcaption></figure></div>

## Export

### Export One Object

1. Open the Object.
2. Click the three-dot button in the top-right corner.
3. Select **Export**.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Docs Export Object.jpg" alt=""/><figcaption></figcaption></figure></div>

### Export Multiple Objects

1. Open a View with your desired Objects.
2. Select them using the left-handle (in Grid and List layout).
3. Right-click and select **Export**.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Docs Export Objects.jpg" alt=""/><figcaption></figcaption></figure></div>

### Export Views

1. Open a View with your desired Objects, such as Type, Query, or Collection.
2. Click the three-dot button in the top-right corner.
3. Select **Export**.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Docs Export View.jpg" alt=""/><figcaption></figcaption></figure></div>

### Export Channel

1. Go to your [Channel Settings](../../settings/channel-settings.md).
2. Click on **Export** in the side menu.
3. Choose your preferred format: Markdown or Any-Block.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Docs Export.jpg" alt=""/><figcaption></figcaption></figure></div>

### Export Settings

When choosing your export format, you will see various options:

1. **Export format** — choose depending on where it's going.
   1. Markdown — to use the content in other apps.
   2. Any-Block — to use the content in another Anytype space.
   3. PDF — a contained and shareable file.
   4. HTML — to use in a web browser.
2. **File format** — You can use either JSON or Protobuf. Protobuf is not human-readable, but it usually delivers the best results.
3. **Zip archive** — to provide the export as a zipped folder.
4. **Include linked Objects** — packages any linked Objects.
5. **Include files** — packages images, videos, and other files in your Objects.
6. **Include archived Objects** — packages archived Objects with the export.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Docs Export Options.jpg" alt=""/><figcaption></figcaption></figure></div>

## Not included in Exports

#### Space Members

Each member in a space is tied to a unique encryption key, which is inherently separate from the shared Channel itself. Space Members can therefore fail to export properly, which may cause breaks if you import the backup into a new space. For examples, an 'assignee' or 'created by' property may not display the correct Space Member.

#### Chats & Discussions

Chat messages and Discussions are tied to each member of the space, which are tied to unique encryption keys for each user. Thus, it is not possible to export chat Objects and messages because they are inherently tied to the space itself.
