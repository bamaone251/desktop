# Iframe Grid Dashboard

This is a single-page dashboard that displays 4 links in iframes laid out like your screenshot:

- Left column: Frame 1 on top, Frame 2 on bottom (Frame 2 is **20% taller**)
- Middle column: Frame 3 (**20% wider** than Frame 4)
- Right column: Frame 4

## Run locally (quick)

### Option A (Python)
1. Open a terminal in this folder
2. Run:
   python -m http.server 8000
3. Open:
   http://localhost:8000

### Option B (Node)
npx serve .

## Set the iframe URLs

### Option A: querystring
Open the page like this:

http://localhost:8000/?f1=https://example.com&f2=https://example.com&f3=https://example.com&f4=https://example.com

### Option B: edit defaults
Open `index.html` and change the `DEFAULTS` object.

## Note about embedding
Some sites block iframing using security headers (X-Frame-Options / CSP). If a site won't load, you may need a different URL or an app you control that allows embedding.
