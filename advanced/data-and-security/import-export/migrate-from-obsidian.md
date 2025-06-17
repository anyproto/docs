# Migrate from Obsidian

#### Step 1: Export from Obsidian

1. Locate your Obsidian Vault: go to Settings → Vault, then click the folder icon to open your vault location
2. Review your files: you’ll find:
   * `.md` (Markdown) files
   * Subfolders (if any)
   * Embedded files like `.png`, `.pdf`
   * Hidden system folder: `.obsidian/` (can be ignored)
3. Do a cleanup (recommended)
   * Convert embeds like `![[Note Title]]` into simple links `[[Note Title]]`
   * Remove or convert any plugin-specific syntax (Dataview queries, Templater fields)
   * Ensure your note content is in clean and standard Markdown format

#### Step 2: Import into Anytype

1. Drag and drop your entire Vault folder (or a subfolder) with `.md` files into Anytype or click Import Files and select it instead.
2. Anytype will process your files and automatically create objects for each Markdown file.

#### Step 3: Content mapping

1. `[[Internal Links]]` → become linked objects in Anytype, so the connections between your notes are preserved.
2. &#x20;`#tags` → become values in the Tag property. You can use them to filter, group or search across objects.
3. Frontmatter (the `---` metadata at the top) → becomes object properties.
