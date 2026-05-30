# Салон Рубин 2000 — QA

Status: PASS locally. Sheet was not updated per instruction.

## Gate 1 — source/fact audit: PASS
- Business name/category: Google Sheet row supplied by Dean + Google Maps mirrors.
- Address: ул. „Тирана“ 25, 1592 ж.к. Дружба 1, София — titul.bg and Polomap.
- Phone: +359 88 580 4169 — Google Sheet row, titul.bg, Polomap.
- Social/profile links: Facebook `https://www.facebook.com/SalonRubin2000`; Google Maps CID `16873097093533256076`.
- Hours: Mon–Sun 10:00–19:00 — titul.bg and Polomap.
- Legacy standalone domain `salonrubin2000.com` appeared in mirrors/search but DNS failed in `web_fetch`; not treated as active official site.
- No invented prices, awards, review counts, credentials, or guarantees.

## Gate 2 — visual-result image audit: PASS
- Hair salon / visual-result business.
- Checked Facebook saved extraction, Google Maps photo URLs via Polomap, Google/search mirrors, and legacy domain availability.
- Site uses real hair-result images near the top: Facebook hairstyle photos plus Google Maps red-hair result.
- Facebook cookie/login wall avoided by using saved public image extraction and mirrored research from `sites/rubin-2000/research/fb-images.json`.

## Gate 3 — testimonial audit: PASS
- Public written testimonials with real names/text found on titul.bg Google profile mirror.
- Used exact visible reviewer names and Bulgarian/original visible text excerpts.
- Removed review counts from public site. No fake/anonymous/rating-only cards.
- No visual star rows used because exact per-review star proof was not exposed in the fetched source.

## Gate 4 — copy audit: PASS
- Bulgarian copy pass completed: H1 clearly states profession + location; CTAs are natural; no audit/source-mechanics copy.
- No numbered service/feature boxes, no placeholder/TODO/Lorem text.

## Gate 5 — link/schema/SEO-head audit: PASS
- Exactly one H1.
- SEO: title, meta description, robots, canonical, OG tags, absolute og:image, twitter card present.
- Schema: HairSalon with NAP, address, hours, sameAs, hasMap, canonical URL.
- Hrefs checked locally: phone, anchors, Facebook, Google Maps, canonical, stylesheet.

## Gate 6 — image/layout audit: PASS after correction
- Image paths load locally after scroll/lazy-load check.
- Hero and gallery use portrait/square frames appropriate to source orientation; no forced landscape crop of vertical hair result.
- 2026-05-30 correction: exact visible image reuse was found (`rubin-fb-3.jpg` hero+gallery and `rubin-fb-8.jpg` services+gallery). This was a QA miss. The page now uses unique visible image files across hero, services, gallery, and contact.
- `rubin-google-2` was re-saved/renamed to `rubin-google-2-fixed.jpg` after Chrome decode issue.

## Gate 7 — map/local SEO audit: PASS after correction
- Bottom Google Maps/local SEO block is directly above footer.
- Map/contact block has exactly one visible navigation CTA.
- 2026-05-30 correction: old long text-query iframe rendered blank in live screenshot QA. Replaced with coordinate-based embed `42.661,23.4015&z=16&output=embed`, then re-tested visible map screenshots.

## Gate 8 — responsive visual QA: PASS
- Local screenshots generated:
  - `artifacts/desktop.png`
  - `artifacts/mobile-final2.png`
  - `artifacts/map-mobile.png`
- Sticky mobile call CTA present.
- Footer has unified SVG icon row for phone, Facebook, Google Maps.

## Gate 9 — final live QA: PASS
- Live URL confirmed HTTP 200: https://deanooooooooo.github.io/salon-rubin-2000-site/
- Live HTML contains business name, testimonial phrase, phone CTA, map/contact block, HairSalon schema, canonical, and OG tags.
