# llm-router-extensions

Plugin marketplace manifest for [llm-router](https://github.com/jrmatherly/llm-router).

The app fetches `marketplace/plugins.json` from this repository's `main` branch. The manifest is a JSON object with a `plugins` array. Each entry carries `id`, `name`, `description`, `module` (an HTTPS URL to a `.js`, `.cjs` or `.mjs` file, 8 MB max), `integrity` (sha256 of the module), `apps`, `permissions`, `surfaces`, `dependencies` and `capabilities`. The format reference is the `plugin.json` of each bundled plugin under `packages/electron/bundled-plugins/` in llm-router.

The list is empty for now: the plugins llm-router ships are bundled with the app, so nothing needs to be hosted here yet.

Point the app at another manifest with `CCR_PLUGIN_MARKETPLACE_URL`.
