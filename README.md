# Hanum Trade website

Static site for hanumtrade.org. Edit `index.html` and replace everything in [square brackets].

## Put it on GitHub
1. Create a new repository on github.com named `hanumtrade-website` (public, no README).
2. Upload `index.html`, `CNAME` and `README.md` (Add file > Upload files), then commit.

## Host free with GitHub Pages
1. Repo > Settings > Pages > Source: "Deploy from a branch", branch `main`, folder `/ (root)`.
2. Under Custom domain, enter `hanumtrade.org` and save.

## Point the domain (Squarespace > Domains > hanumtrade.org > DNS Settings)
Add four A records for host `@`: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
Add a CNAME for host `www` pointing to `<your-github-username>.github.io`
Remove the old Squarespace A records. Do not touch MX, SPF, DKIM or DMARC records.

Then tick "Enforce HTTPS" in GitHub Pages once the certificate is ready.
