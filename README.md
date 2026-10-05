# Almost There

Static site for the band Almost There. Plain HTML/CSS, no build step.

## Local preview

```sh
python3 -m http.server 8000
```

## Hosting (GitHub Pages, free)

1. Push this repo to GitHub (public repo, or private with a paid plan).
2. Settings → Pages → Source: "Deploy from a branch", branch `main`, folder `/ (root)`.
3. Add the domain: create a `CNAME` file in the repo root containing just the domain (e.g. `almostthereband.com`), or set it under Settings → Pages → Custom domain.
4. At the DNS provider:
   - Apex domain: four `A` records pointing to `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `www`: `CNAME` to `<github-username>.github.io`
5. Once DNS resolves, tick "Enforce HTTPS".

## Content still to fill in

- Spotify and Amazon Music links in `index.html` are search URLs. Replace with the direct album URLs once they show up.
- Placeholder images in `assets/` (`cover.svg`, `band.svg`, `photo.svg`). Drop in real images and update the `src` attributes.
- Bio, contact email, show dates.
