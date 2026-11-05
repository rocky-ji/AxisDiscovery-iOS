# AXIS Device Discovery support site

This folder is prepared for GitHub Pages deployment from the `/docs` folder on the default branch.

## Before publishing

1. Replace every `SUPPORT_EMAIL` placeholder in `docs/support.html` and `docs/privacy.html` with a monitored support email address.
2. Review the privacy statements against the final released app and any SDKs you add. The current text describes the present implementation: local Bonjour discovery and direct local anonymous VAPIX requests, with no developer backend or analytics SDK.
3. Keep the bundle ID and store metadata consistent with the app: `com.rockyji.axisdiscovery.mobile`.
4. In the GitHub repository, open Settings → Pages, choose Deploy from a branch, select the default branch and `/docs` folder.
5. After publishing, verify `https://<github-username>.github.io/<repository>/`, `/support.html`, and `/privacy.html` open without signing in. Use the Support and Privacy URLs in App Store Connect.

The app is an independent utility and is not affiliated with or endorsed by Axis Communications. Its iOS discovery uses Bonjour and may not find products that do not advertise a supported Bonjour service.

## Mac App Store pages

The Mac pages are independent of the existing iOS pages. Publish the entire `docs` folder, including `style.css`, `mac.css`, and `assets/app-icon.png`. No build tools or JavaScript are required. Keep GitHub Pages configured for the default branch's `/docs` folder.

| App Store Connect field | Published URL |
| --- | --- |
| Mac Marketing URL | `https://<github-username>.github.io/<repository>/mac.html` |
| Mac Support URL | `https://<github-username>.github.io/<repository>/mac-support.html` |
| Mac Privacy Policy URL | `https://<github-username>.github.io/<repository>/mac-privacy.html` |

Replace the GitHub username and repository placeholders with your public repository's values. Verify all three URLs work without signing in before entering them in App Store Connect. Do not upload the app's private source, signing certificates, or provisioning profiles to this website repository.

The Mac pages use `haichao_ji@163.com` as the public contact address. They describe the free Mac app separately from the iOS app's trial and purchase terms. Both the marketing and support pages document AXIS Camera Station server IP discovery through ONVIF WS-Discovery, with unavailable (NULL / Unknown) serial numbers as a known limitation. Discovery does not enumerate every camera managed by a Camera Station server.

Before submission, check the text against the final sandboxed Mac app and confirm minimum macOS and architecture support. Do not announce Mac App Store availability or add a download badge until the app has actually been published.
