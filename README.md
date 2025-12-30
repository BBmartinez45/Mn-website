# Calm Nerve — Landing Page Prototype

This folder contains a clean, editable landing page prototype for Calm Nerve (early access). Use it as a starting point for your page builder (Shopify, ClickFunnels, Leadpages), or host the static HTML on Netlify/Vercel.

Files added:
- `index.html` — Landing page with hero, features, ingredients, FAQ, signup form (posts to `thankyou.html` placeholder).
- `styles.css` — Simple responsive styles.
- `thankyou.html` — Thank-you/confirmation placeholder after signup.
- `email-welcome.txt` — Draft welcome email and optional beta tester variant.

How to preview locally:
1. Open `index.html` in your browser (double-click the file).

Or serve with a simple static server (PowerShell example using Python if installed):

```powershell
python -m http.server 8000; Start-Process http://localhost:8000/index.html
```

Before public launch, update the following:
- `assets/logo-placeholder.png` and `assets/bottle-mockup.png`  add your real logo and product images.
- Update brand colors in `styles.css` (`--accent` variable).
- Add verified testimonial content where appropriate.
- Configure the signup form action to point to your email provider or page-builder integration.

Integrating with an email provider (high-level steps):
- Klaviyo: create a Signup Form or API list and replace the form action with Klaviyo's form endpoint or use their embedded form code. Map fields to `email`, `firstName`, `beta`.
- MailerLite: create a form and copy/paste the HTML form code or use their API to add subscribers.
- Zapier / Make: post the form to a small serverless endpoint (Netlify Functions/Azure Functions) which forwards to your email provider.

Beta program and follow-ups:
- Capture a `beta` checkbox on your signup form and tag subscribers who checked it.
- Prepare a short onboarding email sequence (welcome, what to expect, beta instructions).

Next recommended steps I can help with:
- Create a Klaviyo/MailerLite-ready form snippet.
- Design a bottle mockup or export transparent PNG for the product image.
- Draft an automated 3-email welcome sequence for early access + beta testers.

If you'd like, I can now:
- Generate the Klaviyo form HTML (tell me which provider), or
- Draft the 3-email welcome/engagement sequence, or
- Replace placeholder images with a base64 placeholder for quick testing.
