---
description: Collapse and expand sections of long Objects.
---

# Toggled Headings

## What is a Toggled Heading?

A **Toggled Heading** is a heading that can be collapsed to hide everything beneath it. Click the toggle arrow and the section folds up; click again and it expands. The heading itself stays visible — only the content below collapses.

This works on all three heading levels: Title (H1), Heading (H2), and Subheading (H3).

## How it works

A Toggled Heading captures everything below it (until the next heading of the same or higher level) as its children. When you collapse the toggle, all those child blocks are hidden.

The hierarchy works the same as regular block indentation:

```
# Project Overview      ← H1 toggle (children = everything below)
  ## Goals              ← H2 toggle (children = paragraphs in this section)
    paragraph
    paragraph
  ## Timeline           ← H2 toggle
    paragraph
    bullet list
# Resources             ← H1 (collapsing this hides everything until next H1)
  ## Reading            ← H2 toggle
```

When you collapse "Project Overview", the entire "Goals" and "Timeline" sections fold away with it.

## Creating a Toggled Heading

#### From the slash menu

1. Type `/` in the editor.
2. Search for **Toggle Heading 1**, **Toggle Heading 2**, or **Toggle Heading 3**.
3. Select the level you want.
4. Type the heading text.

#### Markdown shortcuts

Type these at the start of a line:

* `#>` + space → Toggled Heading 1
* `##>` + space → Toggled Heading 2
* `###>` + space → Toggled Heading 3

#### From a regular toggle

If you've already created a regular toggle block (`>` + space), you can convert it to a toggled heading:

1. Place your cursor in the toggle.
2. Type `#`, `##`, or `###` followed by space.
3. The toggle becomes a toggled heading at that level.

#### Converting an existing heading

To turn a regular heading into a toggled heading:

1. Hover over the heading and click the block handle (six dots) on the left.
2. Click **Turn into > Toggle Heading**.

When you convert, **everything beneath the heading** becomes a child of the toggle automatically — until the next heading of the same or higher level. You don't need to re-indent anything by hand.

## Working with Toggled Headings

#### Expand or collapse one

Click the triangle (▶ / ▼) to the left of the heading to toggle.

#### Expand or collapse all at once

Right-click anywhere inside the editor and choose:

* **Expand all toggles** — opens every toggle on the page
* **Collapse all toggles** — closes every toggle on the page

This works on regular toggles and Toggled Headings together.

#### Add or remove children

To add content under a Toggled Heading, place your cursor at the end of the heading and press Enter — the new block is automatically nested.

To move a block out of a toggle, decrease its indent with Shift + Tab (or drag it to a position above the heading).

#### Convert back to a regular heading

Click the block handle on the heading > **Turn into > Heading 1** (or 2, or 3, without "Toggle"). The toggle behavior is removed but the children stay where they are.

### Behavior in different views

* **In the editor** — toggles work as described above.
* **In Flow view** — toggle state is preserved per Object.
* **In PDF export** — collapsed sections are still exported. Choose **Expand all** before export if you want a tighter PDF.
* **In Markdown export** — toggle state is not preserved (Markdown has no native toggle syntax); all content is exported as standard headings.

### Tips

{% hint style="info" %}
**Use the Title-level toggle as a section divider.** A Toggled H1 named "Archive" or "Old notes" lets you stash content out of the way without deleting it.
{% endhint %}

{% hint style="info" %}
**Convert a heading to a toggle to organize quickly.** If a page is already structured with headings, converting them to toggles is a one-click way to add collapsible sections without restructuring.
{% endhint %}
