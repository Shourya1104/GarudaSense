GarudaSense

**Pause before you click.** GarudaSense is a browser-based cybersecurity awareness prototype from Garuda Wings AI. It helps people inspect suspicious messages, QR codes, and media context before taking action.

## Run locally

1. Download or clone this repository.
2. Keep `index.html` and `garuda_wings_ai_logo.png` in the same folder.
3. Open `index.html` in a modern web browser.

No build step, package installation, or server is required for the basic demo. Some browser features, such as QR image decoding, may require a supported browser and a secure context (HTTPS).

## Features

- Message and link checks using visible rule-based warning signals.
- QR image decoding in supported browsers; the decoded destination is displayed without opening it.
- HawkEye phishing-awareness mini-game with a local scoreboard and leaderboard.
- Deepfake/media screening guidance for awareness. It is not a trained deepfake classifier.
- Contextual help chatbot, FAQs, and safety/recovery guidance.
- Light and dark themes, responsive layout, and the Garuda Wings AI logo.
- Architecture overview, use cases, browser-local performance timings, and code samples.
- Feedback form that prepares a local text draft until a team email or server endpoint is configured.

## Privacy and limitations

The prototype runs its message checks in the browser and does not connect to a backend. The QR feature decodes an image locally when supported. No external reputation service, validated threat-intelligence feed, trained detection model, or public REST API is currently connected.

A result that shows no warning signs does **not** prove a message or link is safe. The displayed timing metrics describe local performance, not detection accuracy. Do not paste passwords, one-time codes, payment data, or other secrets into the site.

The feedback form does not send submissions to the team by default. To configure a team email for a mail-app draft, edit the `garudasense-contact` meta tag near the top of `index.html` and set its `content` value to your team's email address. For automatic collection, connect a trusted form endpoint and update the form handler; no server endpoint is included in this repository.

## Publish with GitHub Pages

1. Upload `index.html`, `garuda_wings_ai_logo.png`, and this README to the root of your GitHub repository.
2. In the repository, open **Settings → Pages**.
3. Under the build and deployment settings, choose **Deploy from a branch**, select your branch (usually `main`) and the **/(root)** folder, then save.
4. Wait for GitHub Pages to publish the site, then open the URL shown in the Pages settings.

The logo file must stay beside `index.html` so the page can load it.

## Project files

- `index.html` — the complete single-page website, styles, and browser-side JavaScript.
- `garuda_wings_ai_logo.png` — logo used in the header and page background.
- `README.md` — project overview and publishing instructions.

## Credits

Created for the Garuda Wings AI hackathon project. Add your contributors, links, and any real evaluation results before presenting the project publicly.
