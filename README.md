# BGdel — Background Remover

Erase image backgrounds **entirely in your browser**. Drop in one or many photos
and BGdel cuts out the subject automatically — perfect for profile pictures and
marketplace listings.

- 🔒 **100% private** — images never leave your device; all processing runs locally.
- 🧠 **AI cutout** powered by [Transformers.js](https://github.com/huggingface/transformers.js)
  with the **BiRefNet‑lite** model (MIT licensed).
- ⚡ Runs on **WebGPU** when available, with an automatic **WASM/CPU** fallback.
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

## License & credits

- App code: free to use.
- Background‑removal model: **BiRefNet‑lite** — MIT licensed, free for commercial use.
- Inference engine: **Transformers.js** (Apache‑2.0).
