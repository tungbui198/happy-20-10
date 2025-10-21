# happy-20-10

Digital greeting card for Vietnamese Women's Day (20/10) with rose animation, confetti, and an order form.

## Highlights
- Static page powered by Tailwind CDN; open `index.html` locally or host on GitHub Pages.
- Floating petals, confetti burst, and interactive 3D rose toggle via tap/click.
- Rotating wish messages that can be personalized through URL parameters (`?to=...&from=...`).
- Drink order form integrates with Google Apps Script and gracefully falls back to Google Form.
- Suggested Highlands Coffee menu for quick selection and automatic form population.
- Respects reduced-motion preferences.

## Quick Start
- Open `index.html` in your browser to preview.
- Share a personalized link: `https://<domain>/happy-20-10/?to=Chi+Lan&from=Minh`.
- Update `og-image.jpg` if you want a custom social share preview.

## Customization
- Adjust form submission settings in the `CONFIG` object (Apps Script endpoint, Google Form fallback, `entry.*` mapping).
- Set `CONFIG.USE_GOOGLE_FORM` to `true` to force the Google Form workflow.
- Edit the drink list in the `MENU` array to match your menu or brand.
- Rewrite the wish messages in the `WISHES` array to suit your audience and tone.
- Tweak styles or effects in the `<style>` block and the script at the bottom of `index.html`.

## Deployment
- Host as a static site (GitHub Pages, Netlify, Vercel, etc.). For GitHub Pages, place the folder in your repo and enable Pages at `/happy-20-10/`.
- If using Apps Script, deploy it as a web app that accepts anonymous POST requests (Deploy > Web app > Anyone).
