# envelope-mx.github.io

GitHub Pages root entry point for the [envelope-mx](https://github.com/envelope-mx) organization. Because this repository's name matches the org name exactly (`envelope-mx.github.io`), GitHub serves it at the bare root domain rather than as a project page.

This repo is just a redirect: it sends visitors straight to the [Envelope documentation](https://envelope-mx.github.io/docs/), which is built and deployed separately from [envelope-mx/docs](https://github.com/envelope-mx/docs).

Live: **https://envelope-mx.github.io/** → redirects to **https://envelope-mx.github.io/docs/**

## Structure

- `index.html` — meta-refresh + canonical-link redirect to `/docs/`
- `404.html` — custom 404 page with a link back to the docs

There is no build step; both files are served as-is via GitHub Pages (Settings → Pages → deploy from a branch, or GitHub Actions — whichever this repo has configured).

## Development

Edit `index.html` / `404.html` directly and preview locally with any static file server, e.g.:

```bash
python3 -m http.server 8000
# then open http://localhost:8000/index.html
```

## Related repositories

| Repository | Description |
| --- | --- |
| [envelope-mx/envelope](https://github.com/envelope-mx/envelope) | Core platform (private — binaries and Docker images published, source is not public) |
| [envelope-mx/docs](https://github.com/envelope-mx/docs) | Documentation site source, deployed to `/docs/` on this domain |
| [envelope-mx/index](https://github.com/envelope-mx/index) | Internal product/technical planning docs |
