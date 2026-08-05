# Block Types

There are many different types of blocks, each serving a unique purpose. Feel free to add and test out as many as you like.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Block Types.gif" alt=""><figcaption></figcaption></figure></div>

### Text blocks

<table data-search="false"><thead><tr><th width="244.21484375">Block</th><th>What it's for</th></tr></thead><tbody><tr><td><strong>Paragraph</strong></td><td>Standard text</td></tr><tr><td><strong>Title, Heading, Subheading</strong></td><td>Section structure, also known as headings (H1, H2, and H3)</td></tr><tr><td><strong>Title</strong></td><td>Title of the object</td></tr><tr><td><strong>Quote</strong></td><td>Quoted or highlighted text</td></tr><tr><td><strong>Callout</strong></td><td>Boxed text for warnings, tips, or notes</td></tr><tr><td><strong>Code</strong></td><td>Monospaced code with syntax highlighting</td></tr><tr><td><strong>Toggle</strong></td><td>Collapsible block that hides nested content</td></tr><tr><td><strong>Toggled Heading</strong></td><td>A heading that also toggles its section. See <a href="toggled-headings.md">Toggled Headings</a></td></tr></tbody></table>

### List blocks

<table><thead><tr><th width="200.66796875">Block</th><th>What it's for</th></tr></thead><tbody><tr><td><strong>Bulleted list</strong></td><td>Standard bullets</td></tr><tr><td><strong>Numbered list</strong></td><td>Auto-numbered list</td></tr><tr><td><strong>Checkbox / To-do</strong></td><td>Tappable checkboxes for action items</td></tr></tbody></table>

Press Tab inside a list item to indent it (creating a nested sub-list). Shift + Tab outdents.

### Media blocks

<table><thead><tr><th width="165.9921875">Block</th><th>What it's for</th></tr></thead><tbody><tr><td><strong>Image</strong></td><td>Inline image (uploaded or embedded by URL)</td></tr><tr><td><strong>Video</strong></td><td>Embedded video player</td></tr><tr><td><strong>Audio</strong></td><td>Embedded audio player</td></tr><tr><td><strong>File</strong></td><td>Generic file with download link</td></tr><tr><td><strong>PDF</strong></td><td>PDF preview</td></tr></tbody></table>

Drag a file onto the editor to insert it. Each file becomes a [File Object](../files-and-media.md) you can find and reference elsewhere.

{% hint style="info" %}
**Tip:** Use the `/file` shortcut to add an existing image or file that's already in your space into a block. This way, you don't need to re-upload the same file. Instead, upload the file once and re-use it over and over again.
{% endhint %}

### Structural blocks

<table><thead><tr><th width="205.1328125">Block</th><th>What it's for</th></tr></thead><tbody><tr><td><strong>Divider</strong></td><td>Horizontal line separator</td></tr><tr><td><strong>Table of Contents</strong></td><td>Auto-generated from your headings</td></tr><tr><td><strong>Table</strong></td><td>Spreadsheet-style data block</td></tr><tr><td><strong>Columns</strong></td><td>Created by dragging blocks side by side (no separate "column block" — see below)</td></tr></tbody></table>

#### Tables

Insert a table block via `/table`. The table starts as a small grid you can extend by dragging the right or bottom edge. Each column can be resized — drag the boundary between two columns to set a custom width. Custom widths are preserved when you export to PDF.

You can also select multiple cells at once:

* Click and drag across cells to select a range
* Apply formatting (bold, color) to the entire selection
* Copy multiple cells to paste elsewhere
* Delete the contents of the selection

### Reference blocks

<table><thead><tr><th width="205.19921875">Block</th><th>What it's for</th></tr></thead><tbody><tr><td><strong>Link to Object</strong></td><td>Card or text reference to another Object</td></tr><tr><td><strong>Inline Date</strong></td><td>Reference to a date in time</td></tr><tr><td><strong>Inline Mention</strong></td><td>Inline <code>@</code>-style mention to an Object</td></tr><tr><td><strong>Inline Query</strong></td><td>Embedded live Query</td></tr><tr><td><strong>Inline Collection</strong></td><td>Embedded live Collection</td></tr><tr><td><strong>Inline Chat</strong></td><td>Embedded Chat thread</td></tr></tbody></table>

### Property blocks

<table><thead><tr><th width="193.50390625">Block</th><th>What it's for</th></tr></thead><tbody><tr><td><strong>Property</strong></td><td>Add an Object's Property as a block in the body content</td></tr></tbody></table>

Useful for surfacing key [properties.md](../../organize/properties.md "mention") prominently. The Property block stays in sync with the Property's value — change one and all others will update. This enables fancy templates and designs for all of your documents.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/slashmenu-property.png" alt=""><figcaption></figcaption></figure></div>

### Code blocks

Code blocks support:

* **Syntax highlighting** — pick the language from the dropdown in the block's top-right corner
* **Multi-line indentation** — select multiple lines and press Tab to indent them all, Shift + Tab to outdent
* **Copy** — a copy button appears on hover to copy the entire block to your clipboard
* **Wrap toggle** — long lines can wrap or scroll horizontally

Type ` ``` ` (three backticks) followed by space at the start of a line to convert it to a code block instantly. After creation, click the language dropdown to switch syntax highlighting.

### Embed blocks

See [Embeds](../../advanced/feature-list-by-platform/embeds.md) for the full list — LaTeX, YouTube, Miro, Mermaid, Figma, Excalidraw, and more.
