# Mona privacy policy site

Static, zero-dependency privacy policy for Pizzeria Lidan AB's Mona application
and its Uber Eats Marketplace menu integration.

## Files

- `index.html` — policy content and semantic structure
- `styles.css` — responsive Lidan-branded presentation
- `favicon.svg` — lightweight Mona browser icon

The page contains no JavaScript, analytics, cookies, external fonts, or remote
assets.

## Preview locally

Open `index.html` directly in a browser, or serve this directory with any static
HTTP server. For example, if Node.js is available:

```powershell
npx --yes serve .
```

## Publish with GitHub Pages

The simplest deployment is a dedicated public repository:

1. Create a repository such as `mona-privacy-policy`.
2. Copy `index.html`, `styles.css`, and `favicon.svg` to the repository root.
3. Commit and push to the `main` branch.
4. In GitHub, open **Settings → Pages**.
5. Under **Build and deployment**, select **Deploy from a branch**.
6. Select the `main` branch and `/ (root)`, then save.
7. Wait for GitHub to publish the HTTPS URL.
8. Enter that exact URL as Mona's **Privacy Policy URL** in the Uber Developer
   Dashboard.

Typical URL:

```text
https://YOUR-GITHUB-USERNAME.github.io/mona-privacy-policy/
```

## Before publishing

- Confirm that Uber production access uses only the intended store/menu scopes.
- Confirm that Mona's implemented log and snapshot retention matches the stated
  90-day periods.
- Update the policy before enabling any Order API scope or processing eater,
  courier, delivery-address, payment, or order-history data.
- Keep the controller identity and contact details current.
- Have the final policy reviewed by the business's legal/privacy adviser.
