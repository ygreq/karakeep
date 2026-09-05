# Karakeep Browser Extension

Browser extension for Karakeep to quickly bookmark links, take notes, and assign tags and lists directly from your browser.

## Development

### Dev Mode (Watch / Hot Reload)
```bash
pnpm --filter @karakeep/browser-extension dev
```

### Production Build
```bash
pnpm --filter @karakeep/browser-extension build
```
Output files are written to `dist/`.

---

## Installing the Extension in Your Browser

### Chromium Browsers (Chrome, Brave, Edge, Opera, Arc)
1. Open your extensions page:
   - **Chrome**: `chrome://extensions`
   - **Brave**: `brave://extensions`
   - **Edge**: `edge://extensions`
2. Turn on **Developer mode** (toggle in the top-right corner).
3. Click **Load unpacked** (top-left corner).
4. Select the `dist/` folder inside this directory (`apps/browser-extension/dist`).
5. After rebuilding or editing code, click the **Reload** (🔄) icon on the Karakeep extension card in the extensions manager.

### Firefox
1. Go to `about:debugging#/runtime/this-firefox`.
2. Click **Load Temporary Add-on...**.
3. Select `dist/manifest.json`.

---

## Configuration
1. Pin the **Karakeep** extension to your browser toolbar.
2. Click the icon to open the popup.
3. Enter your Karakeep server URL (e.g. `http://localhost:3000` or your self-hosted URL) and API key.
