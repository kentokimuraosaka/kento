# Haiburi LLC Website

Static site in `site/` (plain HTML/CSS, no build step), served by Cloudflare Workers static assets (`wrangler.jsonc`).

| File | Page |
| --- | --- |
| `site/index.html` | トップ（日本語） |
| `site/en.html` | Top page (English, for bank / payment reviewers) |
| `site/tokushoho.html` | 特定商取引法に基づく表記 |
| `site/terms.html` | 利用規約 / Terms of Service |
| `site/refund.html` | 返金ポリシー / Refund Policy |
| `site/privacy.html` | プライバシーポリシー / Privacy Policy |

## Publish (automatic)

Every push to `claude/llc-payment-banking-setup-3k09kb` that touches `site/` deploys to the
`haiburillc` Worker (custom domains `haiburillc.com`, `www.haiburillc.com`) through
`.github/workflows/deploy.yml`.

One-time setup: add a Cloudflare API token (template "Edit Cloudflare Workers") as the
repository secret `CLOUDFLARE_API_TOKEN`. Until it exists, the workflow skips the deploy.

## Before publishing, confirm

- Program durations (3 months / 2 months) and what is included.
- Refund policy numbers (8-day full refund, cancellation fee cap JPY 50,000 or 20%).
- Payment deadline (7 days) and start timing (3 business days).
- Replace `haiburillc@gmail.com` with a domain email once available.
