# Kamra Ta Muse LoL Worlds Tracker — GitHub Pages

This folder is ready to publish as a static GitHub Pages site.

## First deployment

1. Create a new GitHub repository, for example `kamra-ta-muse-worlds`.
2. Upload **index.html** and **.nojekyll** from this folder to the repository root.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
5. Select the **main** branch and **/(root)** folder, then save.
6. GitHub will publish the site at a URL similar to `https://YOUR-USERNAME.github.io/kamra-ta-muse-worlds/`.

## Public vs admin view

- Public: open the normal GitHub Pages URL.
- Admin: add `?admin=1` to the end of the URL.
  Example: `https://YOUR-USERNAME.github.io/kamra-ta-muse-worlds/?admin=1`

The admin URL is **not password-protected**. It only exposes editing controls in your browser. Visitors who know the URL can also see the controls, but they cannot change the published GitHub Pages site unless they can commit to your GitHub repository.

## Publishing tournament updates

1. Open the live site with `?admin=1`.
2. Make your team, seed, Play-In, Swiss, and Knockout changes.
3. Click **Export index.html** in the top navigation.
4. GitHub: open the repository, upload/replace the existing `index.html`, and commit the change.
5. GitHub Pages will redeploy. Your friends then see the new published state on the normal public URL.

Admin edits are saved as a browser draft using localStorage until you export. Public visitors ignore localStorage and always read the state embedded in the published `index.html`, so redeployments reliably update what they see.

## Updating with Git instead of the browser uploader

If you use Git locally, replace `index.html` with the newly exported file and run:

```bash
git add index.html
git commit -m "Update Worlds tracker"
git push
```

## Custom domain (optional)

You can later configure a custom domain in **Settings → Pages → Custom domain**. Follow GitHub's Pages DNS instructions for your domain provider.
