---
description: Let AI assistants act on your Anytype data.
---

# Anytype Agents' Skill

The **Anytype Agents' Skill** is an open-source toolkit that gives AI assistants a safe way to read, search, and modify Objects in your Anytype Channels. Drop it into Claude Code, Cursor, Gemini CLI, GitHub Copilot, or any other agent-capable tool, and the agent can run scripts against your Anytype data — programmatically — to handle bulk edits, transformations, and repetitive tasks you'd rather not do by hand.

The repository is on GitHub: [github.com/anyproto/anytype-agents-skill](https://github.com/anyproto/anytype-agents-skill).

***

Anytype already exposes a [Local API](https://github.com/anyproto/docs-new/blob/main/advanced/feature-list-by-platform/feature-list-by-platform/local-api/README.md) for direct integration. The Skill is a layer above that — it bundles the API into ready-made functions an AI agent can use without you having to teach it the protocol.

If you've ever thought "I wish I could just describe what I want to do to my notes and have it happen," this is the bridge. You describe the task in plain language, the agent uses the Skill to translate that into the correct Anytype operations, and the work gets done.

Common use cases:

* **Bulk Property updates** — "Set all Tasks in the 'Q1 Planning' Collection to Status: In Progress"
* **Data transformations** — "Find all Notes tagged 'meeting' from last quarter and create a Collection summarizing them"
* **Migration and cleanup** — "Rename every Object containing 'TODO' in its title to remove that prefix"
* **Reporting** — "List all Objects modified by me this month, grouped by Type"
* **Cross-Channel operations** — "Copy this Type definition from my Personal Channel to my Team Channel"

## How it works

The Skill provides a **lightweight, isolated JavaScript runtime**. When the agent decides to do something to your Anytype data, it writes a short JavaScript script using the Skill's high-level methods, then runs it in the sandbox. The script reads or writes through your local Anytype Local API.

Around 30 high-level methods are exposed, covering:

* **Reading Objects** — get Object by ID, list Objects by Type, search across Channels
* **Creating Objects** — add a new Object with Type, Properties, and content
* **Updating Objects** — set Property values, change Type, edit content blocks
* **Searching** — full-text search, filter by Property, scope to a Channel
* **Working with Types and Properties** — list available Types, create new ones, manage Properties
* **Collections and Queries** — add/remove Objects from a Collection, query with filters

The runtime is **isolated** — the script only has access to the Anytype Skill's methods, not to your filesystem or network. This means you can run AI-generated scripts without worrying about them doing something destructive outside Anytype itself.

(Inside Anytype, of course, the script can change anything the API allows. See the **Safety** section below.)

## Setup

#### Prerequisites

* Anytype installed and running on the same device
* A [Local API key](https://github.com/anyproto/docs-new/blob/main/advanced/feature-list-by-platform/feature-list-by-platform/local-api/README.md) generated in **Vault Settings > API Keys**
* An AI agent that supports tool use (Claude Code, Cursor, Gemini CLI, GitHub Copilot, etc.)

#### Install the Skill

The exact installation steps depend on which agent you're using. Generally:

1. Clone or download the Skill from [github.com/anyproto/anytype-agents-skill](https://github.com/anyproto/anytype-agents-skill).
2. Configure your agent to load the Skill (each agent has its own way to register tools — see the agent's docs).
3. Provide your Anytype API key when prompted.

The Skill's repository includes per-agent setup guides for the most common tools.

#### Verify it's working

Ask the agent something simple, like:

> List all the Object Types in my Personal Channel.

If the Skill is connected, the agent runs a method like `listTypes()` against your Local API and reports back. If it isn't, you'll see an error or the agent will fall back to general-knowledge guesswork.

## Example workflows

#### Bulk update

> Set the Status of every Task in the "Sprint 14" Collection to "Done".

The agent writes a short script that:

1. Finds the Collection by name
2. Lists all Objects inside
3. Filters to Type: Task
4. Updates the Status Property of each one

You see the script before it runs (in most agents) and can approve or reject it.

#### Find and report

> How many Notes did I create this month, and which Tags do they use?

The agent:

1. Queries Objects of Type: Note
2. Filters by creation date
3. Aggregates Tag values
4. Returns a report

No data is changed.

#### Transform and migrate

> For every Book Object in my Reading channel, create a corresponding Review Object linked to it.

The agent:

1. Lists Books
2. For each, creates a new Review Object with a relation back to the Book
3. Reports what it did

## Safety

#### What the Skill can do

Anything the Local API can do. This includes creating, updating, and deleting Objects, modifying Types and Properties, and editing block content.

#### What the Skill can't do

* Access files on your computer outside Anytype
* Make network requests outside the Local API
* See or modify other Channels you haven't given the agent access to (more accurately: the agent can only act on Channels accessible through the API key you provided)
* Bypass Channel permissions — if your role in a Channel is Viewer, the Skill can only read

#### Recommendations

{% hint style="warning" %}
**Review scripts before running them.** Most agents show you what they're about to execute. Read it. A "delete all Objects matching X" script run by mistake is hard to recover from.
{% endhint %}

{% hint style="warning" %}
**Use a separate API key for agent work.** If you ever want to revoke the agent's access, you can delete the key in **Vault Settings > API Keys** without affecting your other integrations.
{% endhint %}

{% hint style="info" %}
**Test on a small scope first.** Before running a bulk operation on hundreds of Objects, ask the agent to do it on five and check the result.
{% endhint %}

### Where to learn more

* [Anytype Agents' Skill on GitHub](https://github.com/anyproto/anytype-agents-skill) — full method reference, examples, per-agent setup
* [Local API](https://github.com/anyproto/docs-new/blob/main/advanced/feature-list-by-platform/feature-list-by-platform/local-api/README.md) — the underlying interface
* [API Keys](https://github.com/anyproto/docs-new/blob/main/advanced/feature-list-by-platform/settings/account-and-data.md) — managing keys in Vault Settings
