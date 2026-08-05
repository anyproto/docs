---
description: Publish Objects as static webpages on your personal subdomain.
---

# Publish

**Web Publishing** lets you turn any Object into a public webpage at a URL anyone can visit. Pick an Object, click Publish, and Anytype generates a static HTML page hosted on your personal subdomain at `<your-id>.any.org/<slug>`.

This is for content you want **publicly readable** — blog posts, public profiles, documentation, meeting briefs, or anything you'd otherwise put on a personal website.

With Web Publishing, the Object you've already written is the published page. Update the Object, republish, and the public page updates. No second platform to maintain.

## Publishing an Object

1. Open the Object you want to publish.
2. Click **Share** in the top-right corner.
3. Review the **URL slug**.
4. Click **Publish**.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Publish.jpg" alt=""/><figcaption></figcaption></figure></div>

Within a few seconds, your Object is live at `<your-any-id>.any.org/<slug>`. Copy the URL or share directly from the dialog.

## Updating a published page

Edit the Object normally. Your edits don't auto-publish — you have to republish to push changes:

1. Open the Object.
2. Click **Share**.
3. Choose **Unpublish** or **Update**.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Publish Update.jpg" alt=""/><figcaption></figcaption></figure></div>

## Managing your published pages

**Vault Settings > My Sites** is the central management screen for everything you've published:

* See a list of every published Object with title, URL, last published date
* Click any URL to open the live page in a browser

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Docs Publish My Sites.jpg" alt=""/><figcaption></figcaption></figure></div>

## What's supported and what isn't

Web Publishing is still in development.

#### Supported in published pages

* **All text formatting** — paragraphs, headings, lists, callouts, quotes
* **Images and image blocks** — included as part of the published page
* **Code blocks** with syntax highlighting
* **LaTeX math** — rendered as static MathML
* **Embeds** that work in static contexts — YouTube, Vimeo, Mermaid diagrams (rendered server-side), images
* **Custom Object icon and cover** — appears at the top of the page
* **Visible Properties** — chosen Properties appear in the page metadata or header
* **Toggle blocks** — collapsed by default in published view, expandable on click

#### Not yet supported

* **Linked Objects** — links to other Objects in your Channel point to a "page not published" placeholder unless those Objects are also published
* **Inline Queries and Collections** — these don't render in published pages
* **Chats and Discussions** — not exposed publicly
* **Multi-page sites** — you can publish many Objects but they're independent pages, not a connected site (multi-page is on the roadmap)
* **Custom themes or styling** — published pages use a default Anytype style
* **Custom domains** — published pages live on `<your-id>.any.org`; pointing a custom domain is on the roadmap

For multi-page sites, watch for updates in the Anytype changelog.

## Tips

{% hint style="warning" %} **Don't publish Objects with sensitive Properties.** Properties like internal status, private notes, and personal information are uploaded too unless you exclude them in the publish dialog. Review what's visible before clicking Publish. {% endhint %}

{% hint style="warning" %} **Anyone with the URL can see a published page** — including web archivers, search engines, and screenshot tools. Treat the URL as effectively public, even if you don't share it widely. {% endhint %}
