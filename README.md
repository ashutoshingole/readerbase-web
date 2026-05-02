# readerbase-web

Static site for [Readerbase](https://readerbase.in), hosted on **GitHub Pages**.

| Path | Purpose |
|------|--------|
| `/` | Store redirect (mobile) + manual links (desktop) |
| `/privacy/` | Privacy policy |

## Before going live

1. In `index.html`, replace `YOUR_NUMERIC_APP_ID` with your real **App Store numeric ID** (App Store Connect). Until then, iOS auto-redirect is skipped if the placeholder is still present.
2. Confirm the Android `applicationId` in `index.html` matches `android/app/build.gradle.kts` in the app repo.
3. **GitHub:** Repo → **Settings** → **Pages** → deploy from branch `main`, folder `/ (root)`.
4. **Custom domain:** Add a `CNAME` file containing `readerbase.in` (or `www.readerbase.in`), then configure DNS per [GitHub Pages custom domain docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).

## Share URL

Use `https://readerbase.in/` (or your GitHub Pages URL until DNS is ready) in the app’s share message.
