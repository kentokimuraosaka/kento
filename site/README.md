# Haiburi LLC Website

Static site (plain HTML/CSS, no build step).

| File | Page |
| --- | --- |
| `index.html` | トップ（日本語） |
| `en/index.html` | Top page (English, for bank / payment reviewers) |
| `tokushoho.html` | 特定商取引法に基づく表記 |
| `terms.html` | 利用規約 / Terms of Service |
| `refund.html` | 返金ポリシー / Refund Policy |
| `privacy.html` | プライバシーポリシー / Privacy Policy |

## Publish (Cloudflare Pages)

1. Buy a domain (e.g. `haiburi.com`) at Cloudflare Registrar.
2. Cloudflare dashboard → Workers & Pages → Create → Pages → Connect to Git → select `kentokimuraosaka/kento`.
3. Build settings: Framework preset **None**, build command empty, build output directory **`site`**.
4. After deploy: Custom domains → add `haiburi.com` and `www.haiburi.com`.

## Before publishing, confirm

- Program durations (3 months / 2 months) and what is included.
- Refund policy numbers (8-day full refund, cancellation fee cap JPY 50,000 or 20%).
- Payment deadline (7 days) and start timing (3 business days).
- Replace `haiburillc@gmail.com` with a domain email once available.
