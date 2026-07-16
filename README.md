# scotthynd.com

Static website for Scott Hynd.

## Files

- `index.html` is the homepage.
- `website-check/index.html` is the Website Check landing page.
- `CNAME` tells GitHub Pages to use `scotthynd.com`.
- `assets/scott-hynd-headshot.jpeg` is the profile image.

## Contact Form

The homepage and Website Check page use native styled contact forms that post to Zoho Forms using Zoho's generated HTML/CSS submit endpoint after the page-level validation passes. This keeps the visual design clean on GitHub Pages while still capturing submissions in Zoho.

The live pages keep the custom-designed forms rather than using Zoho's iframe embed. Spam protection is therefore handled with lightweight front-end checks before the Zoho submit: a hidden honeypot field, a minimum time-on-form check, stronger website URL validation, basic disposable-email blocking, obvious spam phrase blocking, duplicate-submit protection, inline failure messages, and setting the Zoho submit URL only after validation succeeds. These checks reduce page-driven bot spam while preserving the custom design and Zoho Forms backend capture.

Important limitation: because the page still posts directly to Zoho's public HTML/CSS endpoint, these checks cannot stop a bot that already has the endpoint or bypasses the page and posts directly to Zoho. If spam continues, the next step is Zoho Forms server-side spam control/CAPTCHA or a small backend/serverless form proxy that validates requests before forwarding clean leads to Zoho.

The Zoho Forms version remains available as a hosted fallback:

- Public form URL: `https://forms.zohopublic.com/scotthynd1/form/WebsiteReviewRequest/formperma/DGJZU9e6aar0Of3jRZgjOyrkkoTjEaJIyiHvfEWth9o`
- Notification recipient: `scott@scotthynd.com`
- Fields: Name, Email, Phone, Website URL, Type of business, and notes.

Before publishing site changes, submit one local test enquiry and confirm the entry appears in Zoho Forms and the notification email arrives.

## GitHub Pages Settings

Use:

```text
Source: Deploy from a branch
Branch: main
Folder: / root
Custom domain: scotthynd.com
Enforce HTTPS: enabled after certificate is ready
```
