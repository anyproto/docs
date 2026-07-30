---
description: Save and organize web links as first-class Objects.
---

# Bookmarks

A **Bookmark** is a special kind of Object that stores a link to a webpage. Instead of just dropping a URL into a note, you create a Bookmark Object that captures the page's title, preview image, favicon, and a description — making it easy to recognize, link to, and organize like any other Object.

## Why it matters

Bookmarks turn ad-hoc URLs into structured information. You can tag them, filter them, link them to projects. If you're collecting research, building a reading list, saving inspiration, or maintaining a list of references, Bookmarks give them a proper home in your knowledge graph rather than scattering URLs across pages.

## How it works

A Bookmark is its own Object Type that is created by default (a System Type). When you create a bookmark, Anytype fetches metadata from the URL — title, description, preview image, and favicon — and stores them as Properties on the Object.

You can then:

* Add your own Properties (Tags, Status, Priority, Project links)
* Add notes or annotations in the editor
* Link the Bookmark to other Objects
* Include it in Queries, Collections, and Discussions

## Bookmark layout

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Bookmarks Layout.jpg" alt=""><figcaption></figcaption></figure></div>

Bookmarks have their own dedicated layout, separate from the standard [Page layout](objects/formats.md#page-layouts). Each Bookmark displays:

* The page's preview image at the top
* The page title (editable)
* A short URL with the site icon
* A prominent **Open Website** button

You can still add blocks below the bookmark layout if you want to write notes, link to related Objects, or build out additional context. To do this from the editor, right-click the bookmark and select 'Open as Object'.

## Creating a Bookmark

#### From the create menu

In the Channel Sidebar header, click the dropdown arrow and choose **Bookmark**, then paste the URL when prompted.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Bookmarks Create.jpg" alt=""><figcaption></figcaption></figure></div>

#### From the sidebar

In the Sidebar, you can mouse over 'Bookmarks' and click the '+' button. If the Types section is not revealed, then go to [Manage Sections](https://app.gitbook.com/s/uI82XLdf1100Q75OKbEQ/basics/sidebar/sidebar-sections#manage-sections). If the Bookmarks type is not visible, then you may not have any bookmarks yet. Once you have at least one Bookmark, it will display in the Sidebar.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Bookmarks Sidebar.jpg" alt=""><figcaption></figcaption></figure></div>

#### From the editor

If you want to add a bookmark to an existing object, paste the URL like you would any other text and a menu should reveal. Select the 'bookmark' option. This method will create a bookmark block in the object.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Bookmark Editor.jpg" alt=""><figcaption></figcaption></figure></div>

#### From the type

If you open your Bookmarks type from the Sidebar, then all of your bookmarks in the space will be collected there. Use the 'new' button on the right to add a new bookmark.

<div data-with-frame="true"><figure><img src="../.gitbook/assets/Docs Bookmarks Type.jpg" alt=""><figcaption></figcaption></figure></div>

#### From the browser extension

If you've installed the Anytype browser extension, click its icon on any page to save it as a Bookmark Object directly to a Channel of your choice. See your platform's installation guide for setup.

## Organizing Bookmarks

Because Bookmarks are Objects with their own Type, you can:

* **Filter by Tag** — create a "Reading List" tag, a "Research" tag, etc.
* **Pin a Bookmarks Query** to your sidebar to see all your saved links
* **Add an Object Property** linking each Bookmark to a Project or Topic
* **Use the Gallery layout** in a Query to see Bookmarks as visual cards

See [views.md](../organize/views.md "mention") for more details.

## Tips

{% hint style="info" %}
**Use Tags or a Status property to track reading state.** Add states like "To read", "Reading", "Read", "Reference" so a single Bookmarks Query can serve as your reading queue, your library, and your reference shelf.
{% endhint %}

{% hint style="info" %}
**Drag Bookmarks into Collections** when you want to group them by topic without setting up a tag system. A "Trip planning" Collection can hold flight bookings, AirBnB pages, and restaurant reviews side by side.
{% endhint %}
