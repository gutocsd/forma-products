# treste — FORMA 3D Viewer Export

**Product ID:** `treste-001`
**Exported:** 7/8/2026, 3:15:45 PM
**FORMA Version:** 4.0

## Files in this folder

| File | Description |
|------|-------------|
| `viewer.html` | The 3D viewer — open this in a browser or embed as iframe |
| `config.json` | Product settings: materials, lighting, camera, bounding box |
| `Stick.obj` | 3D model |
| `thumbnail.jpg` | Product thumbnail |
| `textures/` | Texture files (if any) |
| `README.md` | This file |

## How to deploy (GitHub Pages — free)

1. Go to **github.com** and create a free account
2. Click **New repository** — name it `forma-products` (public)
3. Upload this entire folder (`treste-001/`) into the repository
4. Go to **Settings → Pages → Source → main branch** → Save
5. Wait ~1 minute. Your viewer URL will be:

```
https://YOURUSERNAME.github.io/forma-products/treste-001/viewer.html
```

6. Test the URL in your browser — you should see the 3D viewer

## How to embed in Framer / Shopify / any website

Once deployed, copy this code and paste into an **Embed** component:

```html
<iframe
  src="https://YOURUSERNAME.github.io/forma-products/treste-001/viewer.html"
  width="100%"
  height="600"
  frameborder="0"
  style="border:none;border-radius:12px">
</iframe>
```

**In Framer:** Insert → Embed → paste the iframe above. Set width to Fill, height to 600px.

**In Shopify:** Pages → Add Section → Custom HTML → paste the iframe.

**In Webflow:** Add → HTML Embed → paste the iframe.

## Troubleshooting

- **Blank page:** Make sure `config.json` and the model file are in the same folder as `viewer.html`
- **CORS error:** GitHub Pages automatically handles CORS — other hosts may need configuration
- **Model not showing:** Check that the model filename in `config.json` matches the actual file name

## Updating the product

Edit the product in FORMA, then export again and replace the files on GitHub. The URL stays the same.
