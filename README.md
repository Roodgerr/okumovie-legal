# Okumovie public policies for GitHub Pages

This folder is a standalone static website. Publish the **contents of this folder**
as the root of a separate public GitHub repository, then open **Settings → Pages**
and select **Deploy from a branch → `main` → `/(root)`**. Do not publish the whole
Okumovie app repository just to host these pages.

The site contains English and Russian privacy policies, terms, and account-deletion
instructions. The policy pages are generated from `assets/i18n/policies.json` by
running `python tools/build_github_policy_site.py` from the app project root.

After GitHub Pages is enabled, URLs follow this pattern:

- `https://<owner>.github.io/<repository>/privacy-en.html`
- `https://<owner>.github.io/<repository>/delete-account-en.html`
- `https://<owner>.github.io/<repository>/terms-en.html`

Replace `<owner>` and `<repository>` with the actual GitHub account and repository.
Use the resulting live URLs in Play Console only after confirming the pages open
without signing in. The support address is copied from the current in-app policy.
