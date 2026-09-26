# Haiburi LLC Website

Static site in `site/` (plain HTML/CSS, no build step), served by Cloudflare Workers static assets (`wrangler.jsonc`).

| File | Page |
| --- | --- |
| `site/index.html` | トップ（日本語） |
| `site/en/index.html` | Top page (English, for bank / payment reviewers) |
| `site/tokushoho.html` | 特定商取引法に基づく表記 |
| `site/terms.html` | 利用規約 / Terms of Service |
| `site/refund.html` | 返金ポリシー / Refund Policy |
| `site/privacy.html` | プライバシーポリシー / Privacy Policy |

## Publish (Cloudflare Workers)

1. Domain: `haiburillc.com` (Cloudflare Registrar).
2. Cloudflare dashboard → Compute → Workers & Pages → Create → Import a repository → `kentokimuraosaka/kento`.
3. Branch: `claude/llc-payment-banking-setup-3k09kb`. Build command empty, deploy command `npx wrangler deploy` (default).
4. After deploy: Settings → Domains & Routes → add custom domains `haiburillc.com` and `www.haiburillc.com`.

## Before publishing, confirm

- Program durations (3 months / 2 months) and what is included.
- Refund policy numbers (8-day full refund, cancellation fee cap JPY 50,000 or 20%).
- Payment deadline (7 days) and start timing (3 business days).
- Replace `haiburillc@gmail.com` with a domain email once available.
