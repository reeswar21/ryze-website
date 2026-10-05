# RYZE Website

Deploy-ready static website for RYZE.

## Before publishing
Edit `assets/config.js` and replace:
- `REPLACE_WITH_YOUR_EMAIL`
- `https://REPLACE-WITH-YOUR-VERCEL-URL.vercel.app`

Use a real email you monitor. Do not submit the site to a payment provider while placeholders remain.

## Preview locally
```bash
python -m http.server 8080
```
Then open `http://localhost:8080`.

## GitHub
Create a new repository such as `ryze-website`, then:
```bash
git init
git add .
git commit -m "Launch RYZE website"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/ryze-website.git
git push -u origin main
```
Never add HitPay keys, database credentials, API secrets or `.env` files.

## Vercel
1. Sign in to Vercel with GitHub.
2. Add New → Project.
3. Import `ryze-website`.
4. Framework preset: Other.
5. Leave Build Command and Output Directory empty.
6. Deploy.
7. Copy the public `*.vercel.app` URL into `assets/config.js`, commit and push again.

## HitPay
Use the public Vercel website URL in the Website field. Do not use your Render API URL, localhost, or a private GitHub URL.

## Included
- responsive landing page
- Regular / Commitment / Daily Commitment explanations
- RM2.50 commitment-charge disclosure
- one-charge-per-occurrence rule
- private-beta disclosure
- FAQ and contact section
- Privacy Policy
- Terms of Use
- Payment & Commitment Policy
- 404 page
- Vercel security headers
- no frontend dependencies or payment secrets

Before merchant submission, verify every statement matches the current app and replace all placeholders.
