# Subdomain setup

Intended address: https://rameshnayaka.ans-siti.com

GitHub Pages publishing source: main branch, / (root).
Custom domain: rameshnayaka.ans-siti.com

At the DNS provider managing ans-siti.com, add:

| Type | Name / Host | Target / Value | TTL |
| --- | --- | --- | --- |
| CNAME | rameshnayaka | pranilpatiltech-cloud.github.io | Default / Auto |

Do not include https://, a path, or the repository name in the target. Do not change the existing @, www, MX, or other main-site records. If a conflicting record already exists for exactly rameshnayaka, resolve only that hostname's conflict.

After DNS propagates, open Settings > Pages > Check again. When the certificate is ready, enable Enforce HTTPS. DNS propagation can take up to 24 hours.

For another independent subdomain, create another repository/site, set its full custom domain in Pages, and add a CNAME for that host. No new domain purchase is required when using an existing domain you control.

Official guidance: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site
