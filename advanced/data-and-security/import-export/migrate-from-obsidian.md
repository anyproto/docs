# Migrate from Obsidian

#### Step 1: Export from Obsidian

* Clean up your notes
  * Convert embeds like `![[Note Title]]` into simple links `[[Note Title]]`
  * Remove or convert plugin-specific syntax, such as Dataview queries, Templater fields, etc.
* Locate your vault
  * Open the Vault switcher (shown at launch or via `File → Open Vault`).
  * Right-click the vault you want to export and choose “Reveal in system explorer.”

#### Step 2: Import into Anytype

* Open `Space Settings → Import → Obsidian` and click on Import files.
* Select your vault folder (or a subfolder) for import.
  * On some platforms (like Linux and Windows), folder selection may not be supported.\
    In that case, compress the folder into a .zip archive and import the archive instead.
* Anytype will process the contents and automatically create a separate object for each Markdown file.

{% hint style="info" %}
#### Content mapping

* `[[Internal Links]]` → become linked objects in Anytype, so the connections between your notes are preserved.
* `#tags` → become values in the Tag property. You can use them to filter, group or search across objects.
* Frontmatter (the `---` metadata at the top) → becomes object properties.
{% endhint %}
