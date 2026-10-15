# MetriGlow Analytics — public website

This repository hosts the public informational website for the **MetriGlow** brand, operated under the name **MetriGlow Analytics** in Calgary, Alberta, Canada.

## Public pages

- `index.html` — homepage
- `privacy.html` — privacy policy
- `terms.html` — EULA and terms of service
- `launch.html` — public client landing page (no public account login)
- `connect.html` — operator-assisted QuickBooks connect/reconnect instructions
- `disconnect.html` — disconnection guidance and support contact (not an automatic revoke API)
- `styles.css` — shared website styling

Business email: metriglow@outlook.com.

## Hosting

Use GitHub Pages from the `main` branch, `/(root)` directory. Expected site: https://metriglow.github.io/.

This **public website repository** is separate from the private `metriglow/metriglow` application source repository; never push client data, access tokens, passwords or Azure settings here.

## Updates

Edit pages in a development branch, review accuracy, and merge to `main` to publish (assuming Pages is configured for `main`). Update the displayed effective date when materially revising legal policies. Check links after publication.

**Compliance note:** The policy pages describe a small reporting business and developing production QuickBooks integration. Before authorizing access to live client financial records or submitting compliance claims to Intuit, verify your actual security controls, retention/deletion processes, legal business disclosures, provider terms and any required agreement with the client. Website publication is not Intuit production approval or legal certification.

## Intuit production setup — important

The public URL candidates are:
- Host domain: `metriglow.github.io`
- Launch: `https://metriglow.github.io/launch.html`
- Connect/Reconnect: `https://metriglow.github.io/connect.html`
- Disconnect landing page: `https://metriglow.github.io/disconnect.html`

These pages are **informational** and presently only send customers to a support email. There is no public customer login or authenticated self-service disconnect here. **Do not claim they are a completed OAuth, automatic disconnect or Intuit-approved integration.** Intuit may require a functional onboarding experience for review.

The production OAuth redirect URI is a DIFFERENT, exact-match HTTPS Azure Function callback URL (not GitHub Pages). Only register that URI once the endpoint and Intuit production keys are ready. Never embed Function keys, OAuth tokens, tenant secrets, unverified client identity or company RealmIds in public HTML.
