# BGdel — Background Remover

Erase image backgrounds **entirely in your browser**. Drop in one or many photos
and BGdel cuts out the subject automatically — perfect for profile pictures and
marketplace listings.

🔗 **Live:** https://bgdel.vercel.app

- 🔒 **100% private** — images never leave your device; all processing runs locally.
- 🧠 **AI cutout** powered by [@imgly/background-removal](https://github.com/imgly/background-removal-js).
- 🖼️ Batch processing, background color presets + custom color, and PNG export
  (transparent or baked background).

## Usage

Just open the site and drop images in. The first run downloads the AI model once
(then it's cached for instant reuse).

## Run locally

This app must be served over **http** (the browser blocks model downloads on
`file://`):

```bash
python -m http.server 5500
# then open http://127.0.0.1:5500/index.html
```

## License

This project is licensed under the **GNU Affero General Public License v3.0
(AGPL-3.0)** — see [LICENSE](LICENSE).

It uses [@imgly/background-removal](https://github.com/imgly/background-removal-js),
which is also AGPL-3.0. In keeping with the AGPL, the complete source code of this
app is published here and linked from the running site. Commercial use (including
ads) is permitted **as long as the source stays available under the AGPL**. If you
need to use it in a closed-source product, obtain a commercial license for the
background-removal library from [IMG.LY](https://img.ly).
