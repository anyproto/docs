---
description: Upload images, videos, audio, and files as standalone Objects.
---

# Files & Media

In Anytype, files aren't just attachments — they're Objects in their own right. Upload an image, video, audio file, or any other file, and it becomes a standalone Object you can reference just like anything else in your space.

This means a file exists once but can be linked across as many Objects as you need — no duplicates, no clutter.

> A photo from a team retreat can be referenced in a Planning doc, a Team Profile page, and a Retrospective note, all without creating multiple copies.

## File Types

There are four built-in File Types in Anytype. Each File Type has its own default Properties and its own dedicated layout optimized for the content.

<table><thead><tr><th width="164.37109375">Type</th><th>Default layout</th></tr></thead><tbody><tr><td><strong>Image</strong></td><td>Image preview at top — JPG, PNG, GIF</td></tr><tr><td><strong>Video</strong></td><td>Embedded player — MP4, MOV, AVI</td></tr><tr><td><strong>Audio</strong></td><td>Embedded player — MP3, WAV, AAC</td></tr><tr><td><strong>File</strong></td><td>Download link with metadata — PDF, ZIP, TXT</td></tr></tbody></table>

## Creating File Objects

#### Directly in the editor

This will add the file as a block in the page and create a standalone Object in the space. There are multiple ways to get a file into the editor:&#x20;

* Drag and drop the file with your mouse.&#x20;
* Copy and paste with shortcut `cmd/ctrl + v`
* Add the 'File Block' from the menu with the shortcut `/file`&#x20;

Adding files via the editor will treat deletion differently, [learn more below](https://app.gitbook.com/o/Ssa9i5QAuI6HhV4jXCLv/s/uI82XLdf1100Q75OKbEQ/~/edit/~/changes/46/creation/files-and-media#deleting-file-objects).&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Files Editor.gif" alt=""><figcaption></figcaption></figure></div>

#### Directly in chat

This will append the file to a message in the chat and create a standalone Object in the space. There are multiple ways to get a file into a chat:&#x20;

* Drag and drop the file with your mouse.&#x20;
* Copy and paste with shortcut `cmd/ctrl + v`
* Click '+' button on the side and select **Upload from computer**.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Files Chat.gif" alt=""><figcaption></figcaption></figure></div>

#### From the sidebar create button

1. In the sidebar, click the Create dropdown button.
2. Choose **Upload from computer**.&#x20;
3. Select a file, drag and drop, or add from a URL.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Files Upload Sidebar.jpg" alt=""><figcaption></figcaption></figure></div>

#### From the sidebar types section

1. In the sidebar, click the File Type's plus button.&#x20;
2. Select a file, drag and drop, or add from a URL.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Files Upload Type.jpg" alt=""><figcaption></figcaption></figure></div>

#### From the types&#x20;

1. Open the File Type of your choice.&#x20;
2. Click on the New button.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Files Type New.jpg" alt=""><figcaption></figcaption></figure></div>

#### Into a collection

1. Create a [Collection](../organize/collections.md) or open an existing one.&#x20;
2. Drag and drop directly into the Objects area.&#x20;
3. All uploads will be part of the Collection and their corresponding File Type.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Files Collection.jpg" alt=""><figcaption></figcaption></figure></div>

## Using Existing File Objects

Once an Object has been uploaded into your space, you're able to use it again on other Objects. There are two methods:&#x20;

* In the block menu, select **Add file** in the Links category.&#x20;
* In the block menu, choose the desired **Media Block** (File for PDFs and Image for JPGs) and navigate to the Library tab.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Files Existing Use.jpg" alt=""><figcaption></figcaption></figure></div>

This is great for ensuring you're always working from the same file. For example, you can reference the same PDF across many documents without uploading it multiple times, keeping things up to date.&#x20;

## Deleting File Objects

Objects in Anytype are not organized by hierarchy, which means that everything exists independently. This means a file on a page exists as a block, but it can also be used across the rest of your space independently in other pages or as a standalone file.&#x20;

Deleting the file block from the page does not delete the File Object itself, it only removes the block or link. To do delete the file, you must explicitly select **Move to Bin**.&#x20;

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Files Deletion.jpg" alt=""><figcaption></figcaption></figure></div>

If you are worried about storage in your space, there is a [Cleanup section in the Bin](../organize/deletion.md) that suggests files to delete which likely no longer serve a purpose in your space.&#x20;

## Working with File Objects

#### Finding files

There are three ways to find your files.&#x20;

1. **Types** — open the File Type from the sidebar. Click 'Image' to see all photos, 'Audio' to see all audio files, etc.&#x20;
2. **Queries** — create a Query for finer control, such as a filter for files larger than 10MB or files uploaded this week.&#x20;
3. **Search** — use the button in the sidebar or shortcut `cmd + k` to look directly for your file.&#x20;

#### Adding metadata

Like any Object, a File can have:

* **Description** — for brief information
* **Tags** — for categorization
* **Object links** — to connect it to other Objects
* **Properties** — additional details to help with organization

#### Block vs. Object File Settings

When you add a file inline in an editor, you can choose how it's displayed:

* **As an embed** — the file is shown inline (image visible, video player embedded, etc.)
* **As a link** — a compact link that opens the file when clicked

The default is set in **Vault Settings > Preferences > Content > File block default style**. Either way, the file exists as an Object you can find through Queries and the sidebar.

## Storage and limits

Files contribute to your Channel's storage usage. Owners can monitor this in **Channel Settings > Remote Storage**, where they see per-member storage breakdowns and total Channel usage.

#### Configurable download size limit

In shared Channels, large files can eat up bandwidth on every device. To prevent this, you can set a **maximum file size for automatic sync** in Settings.

Files larger than the limit won't be fetched automatically — they're listed but stay on the network until a member explicitly opens them. This keeps storage manageable on devices with limited disk space.

To change the limit:

1. Open **Settings > Local Storage**.
2. Find **Offline Access**.
3. Set your desired value.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Offline Files.jpg" alt=""><figcaption></figcaption></figure></div>
