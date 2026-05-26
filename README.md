# scotthynd.com

Static one-page website for Scott Hynd.

## Files

- `index.html` is the homepage.
- `CNAME` tells GitHub Pages to use `scotthynd.com`.
- `assets/scott-hynd-headshot.jpeg` is the profile image.

## Contact Form

The homepage uses a native styled contact form that posts to Zoho Forms using Zoho's generated HTML/CSS submit endpoint. This keeps the visual design clean on GitHub Pages while still capturing submissions in Zoho.

The Zoho Forms version remains available as a hosted fallback:

- Public form URL: `https://forms.zohopublic.com/scotthynd1/form/WebsiteReviewRequest/formperma/DGJZU9e6aar0Of3jRZgjOyrkkoTjEaJIyiHvfEWth9o`
- HTML/CSS submit endpoint: `https://forms.zohopublic.com/scotthynd1/form/WebsiteReviewRequest/formperma/mVRc0ufO6vCfTDREaseBcUxmRjD_kVl-9giawLStW9k/htmlRecords/submit`
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
