# sefinek-i18n
Translation (i18n) files for [sefinek.net](https://sefinek.net). Used as a Git submodule in the main repository, mounted under the `locales/` directory.

## Structure
Each language has its own directory (`en/`, `pl/`), containing JSON files split into namespaces (e.g. `common.json`, `docs.json`, `error.json`, `projects.json`, `verification.json`). File names must match across all languages - namespaces are discovered from the JSON files in the default language directory.

## Usage
Translations are loaded via `i18next` in `services/i18n.js` in the main repository. Adding a new language or namespace also requires changes on the main project's side (see its `CLAUDE.md`).

## Reporting issues
If you notice a typo, mistake, or inaccuracy in a translation - fixes via PR are welcome.
