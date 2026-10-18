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

## The Vitals signup form (Kit)

The form posts the `email_address` field to Kit at `https://app.kit.com/forms/10062576/subscriptions`. Kit has double opt-in on and redirects to `https://agent-er.ai/?subscribed=1#vitals` after signup, where the page swaps the form for a thank-you message asking the subscriber to confirm from their inbox. `thanks.html` is an optional standalone version of that message.
