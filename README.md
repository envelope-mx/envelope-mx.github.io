# envelope.github.io

GitHub Pages entry point for Envelope.

This repository redirects visitors to the [Envelope documentation](https://envelope.github.io/docs/).

## Structure

- `index.html` - Redirect to `/docs/`
- `404.html` - Custom 404 page

## Related Repositories

| Repository | Description |
| --- | --- |
| [envelope](https://github.com/isaiahiroko/envelope) | Core platform (private — binaries and Docker images published, source is not public) |
| [envelope-docs](https://github.com/isaiahiroko/envelope-docs) | Documentation source |

## Documentation

The documentation is built and deployed from the [envelope-docs](https://github.com/isaiahiroko/envelope-docs) repository using GitHub Actions.

Visit: **https://envelope.github.io/docs/**

## Before publishing

This repo's name (`envelope.github.io`) and the links above assume an `envelope` GitHub org owning both this redirect repo and `docs`, mirroring how `awesome-goose.github.io` sits alongside `awesome-goose/docs`. The actual `envelope` and `envelope-docs` repositories are currently under the personal account `isaiahiroko`, not an `envelope` org — before this goes live, either:

- create an `envelope` org and move/fork the repos into it so `envelope.github.io` is a valid org Pages entry point, or
- rename this repo to `isaiahiroko.github.io` (a personal user Pages site) and change `/docs/` below to `/envelope-docs/` throughout (`index.html`'s redirect target and canonical link, `404.html`'s link, and this README), since a user page's docs would live at `https://isaiahiroko.github.io/envelope-docs/` rather than `https://envelope.github.io/docs/`.
