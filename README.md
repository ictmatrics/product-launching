<p align="center">
  <a href="https://github.com/ictmatrics"><img src="assets/ictmatrics-logo.png" alt="ICT Matrics" width="420"></a>
</p>

# Product Launching: Claude skills for launching products in Nepal

Free, skills-only Claude plugins by [ICT Matrics](https://github.com/ictmatrics) for planning, writing and running a product launch for Nepali buyers: from the first launch plan to Messenger replies, Daraz listings and Google Maps.

> नेपाली बजारमा नयाँ प्रोडक्ट लन्च गर्नका लागि Claude स्किलहरू — लन्च योजना, दशैं–तिहारको क्यालेन्डर, NPR मा मूल्य निर्धारण, नेपाली/अंग्रेजी/रोमन नेपालीमा कपी, फेसबुक–टिकटक पोस्ट र विज्ञापन, Messenger रिप्लाई, Daraz लिस्टिङ, र Google/AI मा देखिने बनाउने। सबै तपाईंकै तथ्यमा आधारित; नक्कली रिभ्यु, नक्कली अफर वा अतिरञ्जित दाबी कहिल्यै लेखिँदैन।

## Plugins

| Plugin | What it does | Skills |
|---|---|---|
| [Nepal Launch Strategy](plugins/launch-strategy-np) | Launch plan, readiness check, BS festival calendar, NPR pricing, post-launch review | launch-plan, launch-readiness-check, launch-calendar-np, launch-pricing-np, launch-retro |
| [Nepal Launch Copywriting](plugins/launch-copy-np) | Landing pages, edits, diagnosis, claims check, brand voice, English ↔ Nepali ↔ Romanized | launch-landing-page, copy-edit, copy-diagnose, copy-proof-check, brand-voice, bilingual-copy |
| [Nepal Launch Social & Ads](plugins/launch-social-ads-np) | Launch posts, Meta ads, TikTok/Reels scripts, influencer briefs with disclosure | social-launch-posts, meta-ad-copy, short-video-script, influencer-brief |
| [Nepal Launch Sales & Inquiries](plugins/launch-sales-np) | Messenger/Viber replies, sorting comments, SMS and email, marketplace listings | dm-sales-replies, comments-leads, launch-sms-viber, marketplace-listing |
| [Nepal Launch SEO & AI Visibility](plugins/launch-seo-np) | Launch page SEO, Nepali keyword map, Google Business Profile, AI answers | launch-page-seo, nepali-keyword-map, local-seo-check, ai-search-visibility |

## A launch, end to end

1. **Plan:** `launch-plan` → first buyers, positioning, channels, NPR budget, 90-day timeline.
2. **Time it:** `launch-calendar-np` → window around Dashain, Tihar, weddings or fiscal-year end, with courier cut-offs.
3. **Price it:** `launch-pricing-np` → unit economics with COD, courier and wallet costs; an offer you can honour.
4. **Check it:** `launch-readiness-check` → E-Commerce Act listing, payments, delivery, returns, trust, claims.
5. **Write it:** `launch-landing-page`, `bilingual-copy`, `copy-proof-check`.
6. **Announce it:** `social-launch-posts`, `meta-ad-copy`, `short-video-script`, `influencer-brief`.
7. **Sell it:** `dm-sales-replies`, `comments-leads`, `launch-sms-viber`, `marketplace-listing`.
8. **Get found:** `launch-page-seo`, `nepali-keyword-map`, `local-seo-check`, `ai-search-visibility`.
9. **Learn:** `launch-retro` → where buyers dropped off, and the next 30 days.

## What makes it Nepal-specific

- **Buyers:** Facebook and Messenger as storefront, "price?" comments, COD as the trust default, QR and wallets (eSewa, Khalti, Fonepay), inside-valley vs outside-valley delivery, diaspora gifting.
- **Language:** English, Nepali in Devanagari, and Romanized/code-mixed Nepali, each where it fits; "tapai/hajur" register; NPR and lakh formatting; BS and AD dates.
- **Calendar:** Bikram Sambat months, Dashain, Tihar, Teej, Chhath, Lhosar, New Year, wedding seasons, Asar fiscal-year end, SEE and admissions, monsoon.
- **Rules:** E-Commerce Act 2081 registration, Advertisement (Regulation) Act 2076, National Advertising Policy 2083 (mandatory sponsored disclosure, AI and deepfake rules), Consumer Protection Act 2075, Individual Privacy Act 2075, ad payments through the banking channel. Each with sources and read dates in the skills' `references/` folders.
- **Resilience:** every plan keeps an owned channel because platform access in Nepal has been cut suddenly before.

All example brands (Sathi Khata, Pahadi Maha, Dhaka Ghar, Himali Brew, Kheti Saathi, SikshaPath) are fictional. Synthetic sample inputs are in [samples/](samples).

## Install

Add this repository as a plugin marketplace in Claude Code:

```
/plugin marketplace add ictmatrics/product-launching
```

Then install the plugins you want, for example `/plugin install launch-strategy-np@product-launching`. Each skill folder can also be uploaded on its own as a custom skill in Claude.

## Principles

- Built only on your facts. Missing details are listed, never invented.
- No fake reviews, fake urgency, fake engagement, undisclosed sponsorship or AI "customers".
- Respect for every community; no stereotypes; national symbols not used to sell.
- Not legal, tax or financial advice; rules are flagged with sources so you can confirm them.
- Drafts only: nothing is posted, sent or spent without you.

## Repository layout

```
.claude-plugin/marketplace.json   marketplace listing
plugins/<plugin>/                 one folder per plugin (README, PRIVACY, LICENSE, manifests, icon)
plugins/<plugin>/skills/<skill>/  SKILL.md + references/
shared/                           source copies of the Nepal reference files used inside skills
samples/                          synthetic inputs for trying the skills
```

When you update a file in `shared/`, copy it into each skill's `references/` folder that uses it, so every skill stays self-contained.

## Credits

Derived in part from [marketing-skills](https://github.com/grayskripko/marketing-skills) by Sergey Skripko (MIT). See [NOTICE.md](NOTICE.md) for what was adapted and what is new.

## Feedback

Wrong fact, outdated rule, or a skill that did the wrong thing? Open an issue: https://github.com/ictmatrics/product-launching/issues

## License

MIT, see [LICENSE](LICENSE). Each plugin also carries its own LICENSE and PRIVACY.md.
