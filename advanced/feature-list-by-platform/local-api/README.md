# Local API

Release 0.46.X marks an exciting and long-awaited moment in Anytype’s evolution: **the first iteration of our Local API** is here! It opens up powerful new possibilities for an ecosystem of plugins, automations and third-party integrations.

### Anytype Local API (Developer Preview)

Our API is now available and directly included with the desktop app, running entirely on localhost. It operates fully offline, meaning you can build and use integrations without any cloud dependencies - even while flying!

This initial release targets developers, and we’re eager to see what the community creates with it!

{% hint style="danger" %}
I**mportant Security Notice:** By providing an API key or using extensions, you grant limited access to your Anytype vault, enabling operations such as editing or deleting objects. Ensure you **use only trusted extensions**.
{% endhint %}

### Key Highlights

* **Secure Authentication:** Authenticate once via a 4-digit challenge in the desktop app, generating an API key. This key acts as a bearer token to authenticate subsequent requests. Additionally, API keys can be managed and generated directly through the desktop client's settings, making it easy to share keys with third-party integrations.
* **Comprehensive Documentation:** The OpenAPI specification and full documentation are available on our new [Developer Portal](https://developers.anytype.io/).
* **Robust API Capabilities:** Endpoints offer core Anytype functionality: creating objects, editing, querying and much more.
* **Growing Developer Ecosystem:** Early SDKs and community-driven tools are already underway: Python and Go clients, MCP server and Raycast extension.
