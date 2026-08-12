# Anytype Docs

Source for the official **Anytype** documentation, published at **https://doc.anytype.io**.

Anytype is a local-first, end-to-end encrypted everything app — your thoughts, plans,
and private conversations belong to you, and only you.

Built with [Astro Starlight](https://starlight.astro.build/). Documentation content lives
in `src/content/docs/` (English at the root, translations under `es/` and `fr/`), and
navigation is defined in `sidebar.mjs`. Images live in `public/assets/`.

## Local development

```sh
npm install
npm run dev      # local preview
npm run build    # static build → ./dist
```

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). Fixes and improvements are welcome via pull request.
