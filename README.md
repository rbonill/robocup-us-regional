RoboCup US @2026

This copy is published with GitHub Pages at **https://us.robocupamericas.org** (the `CNAME` file).
The official site, https://us.robocup.org, deploys from `robocup-org/robocup-us-regional`.
When syncing from that repo, keep this repo's `CNAME`: theirs says `us.robocup.org`, and GitHub
only lets one repository use a domain. Keep the `rel="canonical"` link to https://us.robocup.org/ in
`index.html` too, so search engines treat us.robocup.org as the original page.

### Pointing the domain (order matters)
1. Optional but recommended: verify `robocupamericas.org` in the GitHub account (Settings → Pages → Verified domains), so no
   other account can ever claim a subdomain of it.
2. Merge to `main` with this `CNAME`, then confirm GitHub Pages shows `us.robocupamericas.org` as the custom domain
   (`gh api repos/rbonill/robocup-us-regional/pages` → `"cname": "us.robocupamericas.org"`).
3. Only then create the DNS record in the robocupamericas.org zone at FastComet: `us` CNAME `rbonill.github.io.`
   A DNS record pointing at GitHub before the domain is bound here could be claimed by another Pages site.
4. When GitHub has issued the certificate, turn on **Enforce HTTPS**.
