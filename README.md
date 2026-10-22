# Clynera — Interactive Digital Brochure

A complete, self-contained animated brochure for modern clinics and therapy practices.

## Open locally

Open `dist/index.html` in a modern browser. All fonts, artwork, styles and scripts work without a third-party CDN or installation. For a local HTTP preview, run `python -m http.server 8000 --directory dist` from this folder, then open `http://localhost:8000`.

## Deploy to Vercel

1. Extract this ZIP.
2. Upload this folder's contents to your own GitHub repository, retaining the `dist` directory and `vercel.json` at the repository root.
3. In Vercel, import that repository as a new project, or use the source repository of your intended existing project.
4. Select Framework Preset **Other**, leave the Build Command empty, and use **dist** as the Output Directory. The included `vercel.json` provides those settings. No install command or environment variables are needed.
5. Deploy, and open the deployment URL returned by Vercel.

Alternative: if the Vercel CLI is already installed, run `vercel` in this folder for a preview deployment; run `vercel --prod` when ready to publish.

Official deployment configuration: https://vercel.com/docs/builds/configure-a-build
Official CLI deployment guide: https://vercel.com/docs/deployments

The website CTA is configured to **https://clynera.vercel.com**, exactly as supplied. This address could not be verified during preparation. Setting this CTA does not reserve, configure or deploy that domain. Vercel ordinarily assigns project addresses under `vercel.app`; confirm the actual destination in your Vercel project before sharing. If this brochure is deployed at the same URL as the CTA, replace it with your product, contact or demo-booking URL to avoid linking back to the brochure itself.

## What is included

- Six animated chapters with arrows, keyboard navigation, swipe gestures and a contents dialog.
- Responsive desktop and mobile layouts, plus fullscreen presentation where supported.
- Desktop overview/calendar toggle and CSS device mockups inspired by your screenshots.
- Patient delay/reschedule simulation with selectable appointment times.
- Clinical notes, prescription and queue preview tabs.
- Roster, attendance and payroll preview tabs.
- Collections and cash reconciliation previews.
- Full feature directory and downloadable brochure/poster artwork.
- Reduced-motion support, keyboard focus styles and labelled controls.

## Edit

- `dist/app.js`: chapter content, fictional demo data and the `SITE_URL` constant.
- `dist/styles.css`: palette, typography, layout and animations.
- `dist/index.html`: title, description, header and dialogs.
- `dist/assets`: Clynera logo and the four generated campaign artworks.
- `vercel.json`: hosting configuration.

No backend, analytics, database, paid dependencies or API keys are used. Interactions are clearly labelled local simulations, not live clinic functionality. No messages are sent, real appointments made, or financial records accessed. Original screenshots informed the HTML device previews; the campaign artwork also presents those screens with fictional names. The illustrations are design assets, not production print files.

## Validation

JavaScript syntax checked. Desktop navigation, patient slot selection, clinical tabs, team tabs, cash reconciliation and artwork preview were exercised in a browser. A 390 px phone-width preview was inspected. Hosting on Vercel is the remaining deployment step.
