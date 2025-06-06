# Raycast Extension (macOS)

Our long-awaited API is beginning to take shape! The first step is Raycast integration, allowing you to create, read, and delete Spaces, Objects, and Types, as well as search across them, all from Raycast on macOS.

[Install the Raycast Extension here](https://www.raycast.com/any/anytype)

<figure><img src="../../.gitbook/assets/raycast_2x.png" alt=""><figcaption></figcaption></figure>

### Update - AI

We've introduced several enhancements based on your requests and feedback, plus Anytype for Raycast is now an AI Extension – search through spaces and objects using natural language or create new ones just by instructing <kbd>@anytype</kbd>.

* Improved Pinning & Navigation: Pin objects, types, members and spaces for quicker access. Objects of a certain Type now appear below their templates for better organization.
* Better Collection Management: Create objects directly within collections and browse collection items with ease.
* Customization & Visibility: Choose <kbd>Open Object in Anytype</kbd> as the default action, show custom properties in the Detail sidebar, toggle metadata in object details and apply templates when creating new objects.

<figure><img src="../../.gitbook/assets/Screenshot 2025-03-17 at 11.43.00 AM.png" alt="" width="563"><figcaption></figcaption></figure>

### Update - Local API

As a companion to our Local API, we’ve just shipped great improvements for our Raycast extension.

Here’s what’s new:

* **Quickly create** new spaces, objects, types, properties, or tags with the shortcut `CMD+N` while browsing your spaces.
* **Easily edit** your selected items (spaces, objects, types, properties or tags) using `CMD+E`.
* **Conveniently add objects** to lists either through the new `Add object to list` command or directly from the context menu `CMD+K`.

<figure><img src="../../.gitbook/assets/image (213).png" alt=""><figcaption></figcaption></figure>

### Privacy

Our API runs locally on your machine, works without internet connection and requires authentication for a client (eg. raycast extension) to retrieve & access data.

To accomplish this, Raycast initially pairs with the app through the 4 digit pop-up. This notifies you about giving the extension limited access to your account.

The API key is stored in encrypted local storage of the extension and will be used to fetch data from the app (to display spaces, objects etc.).

Therefore, no other applications than the authorized ones can access your data through the API.
