# gradial-site

The marketing website for **Gradial**, a running training plan for iPhone and Apple Watch.

Live at <https://enalmar.github.io/gradial-site/>.

## This repository is the website only

The app source is not open. This repo contains three static HTML pages, some images, and
nothing else: no Swift, no build step, no dependencies, no tracking.

It exists because the App Store requires a reachable privacy policy URL and a reachable
support URL, and because a free app with no server should be able to say so somewhere
people can read it.

- `index.html`: the product page
- `privacy/`: the privacy policy, which mirrors the one shown inside the app
- `support/`: support, the FAQ and the known limitations
- `assets/`: the app icon, the App Store screenshots, and the Open Graph card

## Support

Questions and bug reports: [open an issue](https://github.com/enalmar/gradial-site/issues).

Please do not paste health data into an issue. Describe the shape of the problem instead.

## Adding a custom domain later

One step, whenever it is wanted:

1. Add a `CNAME` file at the repository root containing the bare domain, for example
   `gradial.app`.
2. At the DNS provider, point an `ALIAS`/`ANAME` or four `A` records at GitHub Pages, and a
   `CNAME` for `www` at `enalmar.github.io`.
3. In Settings, Pages, enter the domain and tick **Enforce HTTPS** once the certificate has
   been issued.

The absolute paths in `404.html` are the only thing that would need revisiting, since a
custom domain serves from the root rather than from `/gradial-site/`.

## Licence

The site content is under [CC BY 4.0](LICENSE). The Gradial name, wordmark and app icon are
not covered by it and remain reserved.
