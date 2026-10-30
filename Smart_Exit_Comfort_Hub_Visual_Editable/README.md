# Smart Exit Comfort Hub — Visual Website + Editable Cost Estimator

This is a static, responsive website based on the provided visual concept. It includes transit-themed image panels, package cards, six location examples, how-it-works section, contact enquiry draft and a working editable cost calculator.

## Files
- `index.html` — page structure
- `styles.css` — responsive styling
- `app.js` — editable default package rates and estimator logic
- `assets/` — local image assets, including the visual reference mockup
- `data/cost-estimates.csv` — editable starter price breakdown
- `vercel.json` — static deployment configuration

## Edit prices in the live page
1. Open the website and scroll to **Build Your Own Cost Estimate**.
2. Select a package and change the area, number of locations, contingency, or any individual item rate.
3. Add or remove cost lines as required. Totals update automatically.
4. Download a detailed CSV or choose Print / Save PDF.

## Change default package prices
Edit `app.js` and find `const PACKAGES`. Each item has the form `["Cost item name", "fixed" or "area", rate]`.
- `fixed`: rate is charged per location.
- `area`: rate is multiplied by the area in m² and number of locations.
The currency selector changes only the displayed currency symbol; it does not convert exchange rates.

## Deploy on GitHub + Vercel
1. Extract this ZIP.
2. Upload the **contents** of `Smart_Exit_Comfort_Hub_Visual` into a GitHub repository.
3. Import that repository in Vercel. Choose **Other** as framework preset. No build command is required; static files are served directly.
4. Deploy. No database, API key, or environment variables are required.

## Privacy
The estimator runs in the browser and does not upload costs to a server. Refreshing resets the estimator to default values. Export a CSV if you want to keep a particular quote. The contact form only prepares an email draft and does not transmit data itself.

## Important
The supplied imagery is cropped from the generated visual concept mockup to provide local visual assets. Some panels may include tiny design details from the reference image. Replace images in `assets/` with approved project photography/renderings for a production site. Costs are illustrative planning estimates, not contractor quotations. Confirm site conditions, taxes, permissions, safety/accessibility requirements and supplier prices before budgeting.
