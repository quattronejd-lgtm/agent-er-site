# agent-er-site

The coming-soon page for Agent ER, served at https://agent-er.ai with GitHub Pages.

## Files

- `index.html` is the coming-soon page with The Vitals signup form.
- `thanks.html` is an optional standalone thank-you page.
- `styles.css` holds the site styles in the house palette with Inter.
- `logo.svg`, `favicon.svg`, `favicon-32.png`, and `apple-touch-icon.png` are the purple house mark.
- `og-image.png` is the social share image.
- `CNAME` points GitHub Pages at agent-er.ai.
- `robots.txt` allows indexing.

## Connecting The Vitals signup form to Kit

1. In Kit, create an inline form for The Vitals and open its HTML embed code.
2. Copy the form's `action` URL, which looks like `https://app.kit.com/forms/1234567/subscriptions`.
3. In `index.html`, replace `KIT_FORM_ACTION_URL` with that URL. The email field is already named `email_address`, which is what Kit expects.
4. In the Kit form settings, set the after-subscribing behavior to redirect to an external page, and use `https://agent-er.ai/?subscribed=1#vitals`. The page then shows the thank-you message in place of the form. You can use `https://agent-er.ai/thanks.html` instead if you prefer a separate page.

Until the placeholder is replaced, the form stays on the page and tells visitors that sign-ups open soon, so nothing posts to a dead URL.
