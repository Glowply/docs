# Glowply documentation — project instructions

## About this project

- Bilingual (Arabic + English) help center for **Glowply** (جلوبلي), an Arabic-first "website + online store as a service" for small businesses and online sellers.
- Built on [Mintlify](https://mintlify.com). Pages are MDX with YAML frontmatter; configuration lives in `docs.json`.
- Localized content lives under `ar/` (Arabic) and `en/` (English). Every page exists in **both** languages with matching slugs.
- Audience: non-technical business owners. Write for someone who has never built a website.
- Run `mint dev` to preview, `mint broken-links` to check links.

## The product, in one paragraph

A customer signs up at `glowply.com` → verifies their phone by code (WhatsApp first, SMS fallback) → Glowply automatically builds them a hosted website + store on a `<name>.myglowply.com` address (HTTPS is automatic). They sign in at `glowply.com` and land directly in **one place**:

**Their site dashboard** — a white-labeled admin (Arabic + English toggle) where they run everything: the **Home page** (setup checklist, store stats, recent orders), **Store** (payments, shipping), **Products** (categories, product options, reviews, discounts), **Customers**, **Analytics**, **Branding & contact buttons**, **Store design** (pages, templates, popups) built with the **Builder**, **Content** (blog, media), **Marketing**, the **Ask Glowply** assistant, and **Settings** — which now holds **Subscription & Billing**. Billing is a **prepaid wallet**: you top up (bank card or mobile wallet) and the monthly subscription renews itself from the wallet balance. A free trial starts automatically; after it, renewals are charged from the wallet.

The old **account portal** at `/my-account/` has been **retired** and now forwards into the site dashboard. There is one area, not two — document the dashboard and its sections, and make clear which section a task lives in.

The dashboard's setup checklist is 7 steps: **Your design → Your logo → Categories → Products → Delivery → Test order → Share link** (التصميم ← اللوجو ← الأقسام ← المنتجات ← التوصيل ← أوردر تجريبي ← شارك اللينك).

## Terminology (use these exact terms; never invent synonyms)

The site dashboard labels below are what the customer actually sees (confirmed against the live dashboard). Several changed from earlier terms — the old term is noted so you can catch stale copy.

| English | Arabic | Notes |
|---|---|---|
| Glowply | جلوبلي | Brand. Tagline: "Where ideas glow." |
| site dashboard / your dashboard | لوحة تحكم موقعك | The one place you work. White-labeled admin; Arabic ⇄ English toggle |
| Home page | الصفحة الرئيسية | Dashboard home: setup checklist, store stats, recent orders |
| account portal | — (retired) | Old `/my-account/` area — retired; the URL now forwards into the site dashboard |
| Subscription & Billing | الاشتراك والفواتير | Under **Settings**. Store owner only. Live and self-serve |
| Subscription | الاشتراك | Trial → active → past due → cancelled |
| free trial | الفترة التجريبية | Starts automatically when the site is created |
| Wallet / wallet balance | المحفظة / رصيد المحفظة | Prepaid balance |
| top up | شحن (المحفظة) | Self-serve in Subscription & Billing: cover next renewal, or 1 / 3 / 6 renewals, or a custom amount |
| renewal | التجديد | Monthly; charged from the wallet, not a card |
| past due | متأخر الدفع | Renewal failed (wallet too low) |
| payment methods | بطاقة بنكية / محفظة موبايل | Bank card (Visa/Mastercard, instant) or mobile wallet (Vodafone Cash, Orange Cash) |
| Plan | الباقة | One monthly plan |
| Account (settings) | الحساب | Name/phone editable; email change via support |
| Site management | إدارة الموقع | SSL, custom domain, open editor |
| custom domain | النطاق المخصص | Requested via support, not self-serve |
| Store | المتجر | Menu group → Payments (الدفع), Shipping (الشحن) |
| Payments | الدفع | Under Store |
| Shipping / delivery | الشحن / التوصيل | Under Store |
| Products | المنتجات | Menu group → Categories, Product options, Reviews, Discounts |
| Categories | الأقسام | Singular القسم. Was التصنيفات until 2026-10-26 |
| Tags | الوسوم | |
| Product options | خيارات المنتجات | **Was "Attributes" / الخصائص.** Size, color, etc. → product variations |
| Reviews | التقييمات | **Was المراجعات.** Ratings & feedback on products |
| Discounts | الخصومات | **Was "Coupons" / القسائم.** Discount codes (one quick-action is still "New Coupon") |
| Orders | الطلبات | |
| Customers | العملاء | Menu group → Customers, Customer messages |
| Customer messages | رسائل العملاء | **Was "Form submissions" / إرسالات النماذج.** Messages from your site's forms |
| Analytics | التحليلات | Sales / product / revenue reports (also "Store analytics") |
| Branding & contact buttons | الهوية وأزرار التواصل | Logo, store branding, and contact buttons (WhatsApp etc.) |
| Store design | تصميم المتجر | Menu group → Pages, Ready-made templates, Popups |
| Pages | الصفحات | Edited with the Builder |
| Ready-made templates | القوالب الجاهزة | Template library |
| Popups | النوافذ المنبثقة | |
| the Builder | البلدر | The page editor (white-label of Breakdance); reached via Store design → Pages |
| Builder library | مكتبة البلدر | |
| Elements manager | مدير العناصر | |
| Maintenance mode | وضع الصيانة | |
| Content | المحتوى | Menu group → Blog, Images & files |
| Blog | المدونة | Was "Posts" / المقالات |
| Images & files | الصور والملفات | Media library. Under Content |
| Marketing | التسويق | Menu group → SEO, Live Events, Journeys, Website Analytics, Connect your ads |
| SEO | الظهور في جوجل | Menu label = "Appear in Google" |
| Live events | اللي بيحصل دلوقتي | |
| Journeys | رحلة العميل | Customer journey |
| Website Analytics | زوار الموقع | Site visitors |
| Connect your ads | ربط الإعلانات | Ad pixels |
| Settings | الإعدادات | → General settings, Translate your site, Subscription & Billing |
| Ask Glowply (assistant) | اسأل glowply | In-dashboard AI assistant; answers from the Glowply guide (these docs) |

Product facts to keep accurate: address is always `<name>.myglowply.com`; currency is **EGP** (ج.م); HTTPS/SSL is automatic; billing is a **self-serve prepaid wallet** in **Settings → Subscription & Billing** (top up by **bank card** or **mobile wallet** — Vodafone Cash / Orange Cash); support is **support@myglowply.com**, live chat, and WhatsApp. The in-dashboard **Ask Glowply (اسأل glowply)** assistant answers store owners' questions from these docs.

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
- **Never expose internal vendor names** the customer doesn't see: Breakdance (it's "the Builder"), WordPress/WooCommerce (it's "your site"/"the Store"), Enhance, Akedly, Bosta (it's "shipping/delivery"). The current billing page names **no** payment provider — it shows a "certified provider" plus bank-card / mobile-wallet options — so don't name Kashier (or any provider) in customer docs; say "a certified payment provider".
- Don't document admin-only settings (wallet unit price, plan/trial configuration) — those are internal, not customer-facing.
- Don't reproduce the full WooCommerce or Breakdance manuals. Cover Glowply's UI and the common tasks thoroughly; keep deep third-party edge cases out.
- One trial signup per phone number; Egyptian phone numbers at signup; one site per account — reflect these limits where relevant.
