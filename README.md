# GitHub Pages deployment copy

This folder contains the Calendly-free version of La Boîte à Je prepared for GitHub Pages. It is a static HTML/CSS site; no build step or package installation is required.

## Push this folder to the requested repository

The target repository is `https://github.com/jifu8756-droid/La-boite-a-je-test.git` (default branch `main`). It was checked and is currently empty. From a terminal where you are authenticated to GitHub, run:

```sh
git clone https://github.com/jifu8756-droid/La-boite-a-je-test.git
cd La-boite-a-je-test
cp -R /path/to/site/github-pages/. .
git add .
git commit -m "Prepare site for GitHub Pages"
git push -u origin main
```

Replace `/path/to/site` with the local path to the folder containing `github-pages/`. The `cp` command copies the deployment folder contents into the repository root, including `index.html` and `assets/`.

## Enable GitHub Pages

1. In the repository, open **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select `main` and `/ (root)`, then save.
4. Wait for the Pages deployment to complete and open the URL shown in Pages settings.
5. Test navigation, the mobile layout, and the contact/appointment flow before sharing the URL.

The root `index.html` is an exact copy of the approved `index_test2.html` homepage and is the entry page GitHub Pages expects.

For a custom domain, configure it in GitHub Pages and follow GitHub's DNS instructions. Enable **Enforce HTTPS** after the certificate is provisioned. Update the legal notice to reflect GitHub Pages hosting and complete the remaining legal placeholders before public launch.

Review [`BEFORE_SHIPPING.md`](BEFORE_SHIPPING.md) for outstanding launch items. This deployment copy intentionally excludes project archives, reference websites, source-only documents, and temporary drafts.
