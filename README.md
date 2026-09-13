# grimaldisound.com

Portfolio site for Marcus Grimaldi — mixing engineer and sound designer.

## Deploying with GitHub Pages

1. Create a new repository on GitHub (public).
2. Upload everything in this folder to the repo root — `index.html`, `support.js`, and the `assets/` folder. Keep the folder structure exactly as-is.
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment", set Source to **Deploy from a branch**, branch **main**, folder **/ (root)**. Save.
5. After a minute the site is live at `https://<your-username>.github.io/<repo-name>/`.

## Pointing grimaldisound.com at it

1. In **Settings → Pages → Custom domain**, enter `grimaldisound.com` and save.
2. At your domain registrar, add these DNS records:

   - Four `A` records for `@` → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - One `CNAME` record for `www` → `<your-username>.github.io`

3. Back in Settings → Pages, tick **Enforce HTTPS** once the certificate is issued.

## Notes

- The album cover images still load from the old Squarespace CDN. If that site is taken down, those images break — re-upload them into `assets/art/` and update the `<img src>` values in `index.html`.
- The contact form posts to Web3Forms. Emails go to the address on that account.
- Audio files total about 25 MB, which is fine for GitHub Pages (1 GB limit).
