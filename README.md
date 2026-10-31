# AskWise: AI Chat Assistant — Official Website Package

**Product:** AskWise: AI Chat Assistant  
**Android package:** `com.chatpro.assistant`  
**Developer / public brand:** TechTornix Solutions  
**Support email (correct):** `chatpro@techtornix.com`  
**Legal effective date:** October 31, 2026

## Site pages

| Web route | Entry file |
|---|---|
| `/` | `index.html` |
| `/privacy/` | `privacy/index.html` |
| `/terms/` | `terms/index.html` |
| `/support/` | `support/index.html` |

## Tech stack

- Zero-build HTML5, modern CSS3, vanilla JavaScript (no React/npm/build required)
- Responsively crafted Android UI previews in HTML/CSS (not dead screenshot mockups)
- Generated AskWise glass / neon icon imagery, original scalable feature illustrations (SVG)
- Google Fonts DM Sans / Manrope with system fallbacks
- SVG icon sprite included inside each page, without external icon libraries
- Searchable support knowledge base, topic filters, accessible accordions, responsive menu, monthly/yearly Pro switcher
- Search engine meta tags, social sharing thumbnail, SoftwareApplication structured data, web manifest

## Preview locally

From the unzipped `AskWise_Website` directory:

```bash
python3 -m http.server 8080
```

Open <http://localhost:8080> in your browser.

## Deploy on Hostinger or any static host

Upload **all files and folders in `AskWise_Website/`** into your website's `public_html/` folder. Do not upload only `index.html`. The folders `privacy/`, `terms/`, and `support/` contain their own `index.html` for clean URLs.

Because the site uses relative links, it works at the root of a domain and also under many ordinary subfolders (assuming the host resolves folder `index.html`). HTTPS is recommended for public launch.

## Before publishing

1. **Google Play URL:** Buttons use `https://play.google.com/store/apps/details?id=com.chatpro.assistant`. This is the standard link pattern; it will work only when the Play listing is available to visitors.
2. **Pro pricing:** No unverified subscription prices are shown. The pricing switcher selects monthly/yearly copy; users see their real local price and renewal terms in Google Play or the app. Update marketing claims if your actual entitlements differ.
3. **Support form:** This is a static website. The validated form prepares a `mailto:` message in the visitor's email client; the visitor must press **Send**. It does **not** silently send email or pretend to submit to a server. For server-side delivery on Hostinger, connect a tested form handler (e.g. server-side PHP with authenticated SMTP, spam protection, and appropriate privacy disclosures).
4. **Privacy / Terms:** Text reflects the technical behavior and integrations provided in the brief but **must be reviewed against the shipped Android manifest, data flows, network calls, backup settings and subscription configuration** before publication and against your Google Play Data safety disclosure. Legal content is a launch-ready draft, not a guarantee of compliance or legal advice.
5. **Website address:** No final production domain was supplied, so canonical absolute URLs and production sitemap are intentionally omitted. Add canonical URLs and a sitemap when your domain is known.
6. **Data sharing:** The website does not run analytics/marketing trackers or set cookies in its own code. Remote Google Fonts are loaded unless you choose system-font-only mode; consider self-hosting font files with appropriate licenses if your legal review requires it.
7. **Real app UI:** Device previews are design mockups. Compare labels, screens, feature availability and widget actions to the production app and revise if needed.
8. **Verify your mail domain:** Ensure `chatpro@techtornix.com` is a functioning mailbox, with domain SPF/DKIM/DMARC configured.

## Privacy copy clarification

The policy correctly distinguishes *app-private local copies* from data sent to external AI providers when the user requests AI or transcription. It also distinguishes deletion of on-device data from processor retention. Google's Android microphone service policy restricts starting microphone capture from the background (already-started foreground recording may continue after the screen locks).

Relevant official references:

- [Android microphone foreground services](https://developer.android.com/develop/background-work/services/fgs/service-types)
- [Android background service restrictions](https://developer.android.com/develop/background-work/services/fgs/restrictions-bg-start)
- [OpenAI API data controls](https://developers.openai.com/api/docs/guides/your-data)
- [Google Play subscription management](https://play.google.com/store/account/subscriptions)

## Update the colors

All color tokens are near the top of `assets/css/styles.css`.

## Folder layout

```text
AskWise_Website/
├── index.html
├── privacy/index.html
├── terms/index.html
├── support/index.html
├── assets/css/styles.css
├── assets/js/main.js
├── assets/img/...
├── site.webmanifest
└── README.md
```
