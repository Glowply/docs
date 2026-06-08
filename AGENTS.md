# Glowply documentation — project instructions

## About this project

- Bilingual (Arabic + English) help center for **Glowply** (جلوبلي), an Arabic-first "website + online store as a service" for small businesses and online sellers.
- Built on [Mintlify](https://mintlify.com). Pages are MDX with YAML frontmatter; configuration lives in `docs.json`.
- Localized content lives under `ar/` (Arabic) and `en/` (English). Every page exists in **both** languages with matching slugs.
- Audience: non-technical business owners. Write for someone who has never built a website.
- Run `mint dev` to preview, `mint broken-links` to check links.

## The product, in one paragraph

A customer signs up at `glowply.com` → verifies their phone by code (WhatsApp first, SMS fallback) → Glowply automatically builds them a hosted website + store on a `<name>.myglowply.com` address (HTTPS is automatic). They then use **two areas**:

1. **The account portal** at `/my-account/` — Dashboard, Subscription, Wallet, Account, Site management. Billing is a **prepaid wallet**: you top up, and the monthly subscription renews itself from the wallet balance. A free trial starts automatically; after it, renewals are charged from the wallet.
2. **Their site's own dashboard** — Store, Pages, Media, Posts, Marketing, and the **Builder** — reached from the portal via a one-click "Glowply dashboard" button. This is where they build pages and run the store.

Document both areas. Make clear which area a task lives in.

## Terminology (use these exact terms; never invent synonyms)

| English | Arabic | Notes |
|---|---|---|
| Glowply | جلوبلي | Brand. Tagline: "Where ideas glow." |
| account portal / your account | لوحة حسابك | The `/my-account/` area |
| Dashboard | لوحة التحكم | Both the portal home and the site dashboard home |
| Subscription | الاشتراك | Trial → active → past due → cancelled |
| free trial | الفترة التجريبية | Starts automatically when the site is created |
| Wallet | المحفظة | Prepaid balance |
| wallet balance | رصيد المحفظة | |
| top up | شحن (المحفظة) | Add credit in 1 / 3 / 6 / 12-month bundles |
| renewal | التجديد | Charged from the wallet, not a card |
| past due | متأخر الدفع | Renewal failed (wallet too low) |
| Plan | الباقة | |
| Account (settings) | الحساب | Name/phone editable; email change via support |
| Site management | إدارة الموقع | SSL, custom domain, open editor |
| custom domain | النطاق المخصص | Requested via support, not self-serve |
| the Builder | البلدر | The page editor (white-label of Breakdance) |
| Template library | مكتبة القوالب | |
| Builder library | مكتبة البلدر | |
| Elements manager | مدير العناصر | |
| Maintenance mode | وضع الصيانة | |
| Store | المتجر | The online store |
| Products | المنتجات | |
| Orders | الطلبات | |
| Customers | العملاء | |
| Categories | التصنيفات | |
| Tags | الوسوم | |
| Attributes | الخصائص | |
| Reviews | المراجعات | |
| Coupons | القسائم | |
| Form submissions | إرسالات النماذج | |
| Pages | الصفحات | |
| Media library | مكتبة الوسائط | |
| Blog / Posts | المقالات | |
| Marketing | التسويق | |
| SEO | تحسين محركات البحث | |
| Site analytics | تحليلات الموقع | |
| Store analytics | تحليلات المتجر | |
| Journeys | الرحلات | |
| Live events | الأحداث المباشرة | |

Product facts to keep accurate: address is always `<name>.myglowply.com`; currency is **EGP** (ج.م); HTTPS/SSL is automatic; payments run through **Kashier** (the customer just sees a payment page — card or wallet); support is **support@myglowply.com**, live chat, and WhatsApp.

## Style preferences

- Mirror Arabic and English 1:1 — same structure, same examples, same screenshots. Arabic renders right-to-left automatically.
- Active voice, second person ("you" / "أنت" implied). One idea per sentence.
- Sentence case headings in English; natural phrasing in Arabic.
- Bold for UI you click: **Top up** / **شحن**. Always give both the visible label and (where helpful) the other language in parentheses on first mention.
- Use Mintlify components: `<Steps>` for procedures, `<Card>`/`<CardGroup>` for navigation, `<Note>`/`<Warning>`/`<Tip>` for callouts, `<Accordion>` for FAQs.
- Reference the area explicitly: "In your **account portal**…" vs. "In your **site dashboard**…".
- Don't hardcode prices/amounts that change — describe the model and link to the live pricing page.

## Content boundaries

- Document only what the customer actually sees: the portal and the white-labeled site dashboard. Customers never see raw `wp-admin` chrome.
- **Never expose internal vendor names** the customer doesn't see: Breakdance (it's "the Builder"), WordPress/WooCommerce (it's "your site"/"the Store"), Enhance, Akedly. Kashier is fine to name (it appears on the payment page).
- Don't document admin-only settings (wallet unit price, plan/trial configuration) — those are internal, not customer-facing.
- Don't reproduce the full WooCommerce or Breakdance manuals. Cover Glowply's UI and the common tasks thoroughly; keep deep third-party edge cases out.
- One trial signup per phone number; Egyptian phone numbers at signup; one site per account — reflect these limits where relevant.
