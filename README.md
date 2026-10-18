# Sonar

Scan the depths. Detect the signal. Launch the coin.

A static site: one `index.html` with no build step.

## Files

- `index.html`: the whole site (HTML, CSS and JavaScript)
- `favicon.svg`: browser tab icon, drawn from the logo's pixels
- `logo.png`: home-screen icon
- `og.png`: link preview image for X, Discord and Telegram
- `vercel.json`: Vercel settings

## Deploy on Vercel

1. Push these files to the root of a GitHub repo.
2. In Vercel, choose **Add New → Project** and import the repo.
3. Set **Framework Preset** to **Other**. Leave the build command and output directory empty.
4. Click **Deploy**.

## Settings in index.html

- `CFG.X`: your X profile URL, shown as the "Follow on X" button in the $SONAR panel. Currently `https://x.com/SonarDotRent`.
- `CFG.RPC`: your own Solana RPC URL (for example Helius or Triton). The public endpoint rate-limits browser traffic, so wallet balances may not load without your own.
- Link previews: some apps need an absolute URL for `og:image`. Once you have a domain, change `content="/og.png"` to `content="https://yourdomain.com/og.png"`.
