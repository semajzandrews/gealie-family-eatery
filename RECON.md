# RECON · Gealie Family Eatery

## Verified facts (used in the build)
- **Business:** Gealie Family Eatery (also seen as "Gealie's Family Eatery")
- **Category:** Authentic Jamaican home cooking (the kit's "Caribbean / American family eatery" reads, in reality, as a Jamaican eatery; copy and imagery anchored to Jamaican to make the category unmistakable).
- **Address:** 183A Main St, City of Orange, NJ 07050 (this is the Main St / City of Orange location; note there is a related/second listing at 624 Central Ave, East Orange. All copy is anchored to 183A Main St, City of Orange.)
- **Phone:** (973) 677-4214 — CONFIRMED across multiple directories.
- **PIN (last 6 of phone):** 774214 — CONFIRMED.
- **Google rating context:** 4.0 (Restaurantji shows 3.9/98 reviews; pill in hero shows 4.0 per the brief facts).
- **Existing website:** NONE found. Multiple directory listings (Yelp, Restaurantji, EatOkra, Jamaican Food Map, East Orange Eats, Wheree) but no official site. Confirms the BWYW premise.

## Hours (the part with conflicting sources, resolved)
Sources disagreed at the margins:
- Restaurantji / Yelp pattern: **Mon–Sat 9 AM – 9 PM, Sun Closed**.
- Jamaican Food Map: Tue–Wed 11 AM – 9 PM, Thu–Sat 9 AM – 9 PM, Sun–Mon Closed.
- A general search summary: open 11 AM – 9 PM Mon–Sat, Sun Closed.

**Decision:** Used **Tuesday–Saturday 9 AM – 9 PM, Sunday & Monday Closed** as the safest, most-supported reading (9 AM open aligns with serving Jamaican breakfast like ackee & saltfish; Sun closed is unanimous; Mon closed appears in the most detailed per-day source). 12-hour time everywhere. The owner can correct a day in one line before LIVE. Live Open/Closed pill computes from these hours in America/New_York (verified: at Wed 10:56 PM ET the pill correctly read "Closed now. Opens tomorrow at 9 AM").

## Services
- Dine in, take out, call-ahead ordering. Wheelchair accessible entrance/seating (per Yelp).

## Signature dishes (verified, used in menu + flip cards)
Brown stew oxtail (~$14, the repeat-order favorite), curry goat (~$14), jerk chicken (~$12), brown stew chicken, curry chicken, escovitch fish, ackee & saltfish (breakfast), beef patties (~$3), coco bread, rice & peas, fried plantain, steamed cabbage. Prices are directional (one verified data point: large oxtail $14); menu notes prices are a guide and the counter has the final word.

## Social (verified)
- Instagram **@gealiesrestaurantnj** — appears in two independent sources tagged "Orange, NJ" for this business, so shown. No other handle verified.

## Upsell intel (one line, for admin / Notion)
No online-ordering presence found (no Uber Eats / Grubhub / DoorDash / Toast link surfaced) and no website — a "Order ahead online / menu + delivery wiring" upsell is wide open on top of the base site.

## Art-direction notes (locked kit honored)
- Accent **#2C8C7D** teal, base **#FBF6EC** cream, **Sentient** display (italic teal accent word in hero + signature lines), **General Sans** body.
- Layout: warm magazine columns / stacked alternating bands (cream → cream-2 story → cream specials → dark ink menu → cream-2 story/reviews → visit). Mood: warm-classic family table.
- Deliberately breaks the soul-food/restaurant cliché ban: NOT brown-on-cream rustic, NO fork-and-knife icon, NO faux-chalkboard, NO generic food carousel. Teal+gold on cream is the differentiator.
- **Signature interaction (mine alone):** daily-special **flip cards** (click / hover / keyboard to flip; `aria-pressed` toggled; 3D rotateY verified as matrix3d 180°) with a subtle **CSS steam micro-animation** rising off the hot dish on the front face (20 particles; pauses on flip; reduced-motion safe). A matching steam wisp rises off the hero oxtail plate. Both states are legible at a glance (front = photo + day + dish name on a dark veil; back = teal card with description + price).
- Reveals are pure-CSS, visible-by-default, with a `reveal-done` force-visible safety net at 2.6s (per the "never gate visibility on JS" lesson). Verified computed opacity 1 on specials head + cards.
- Real nav (brand mark + 4 section links + persistent call CTA; CTA collapses to a 46px icon on mobile, plus a floating call button). Keyless Google Maps embed on the real address (verified iframe present, output=embed Ramos pattern). bysemaj.com footer credit styled to brand (teal pin + gold link).

## Verification done
- Opened at http://localhost:8080/gealie-family-eatery/.
- All 8 images load (naturalWidth > 0), zero broken.
- Map iframe present with correct src.
- Flip signature verified flipping (matrix3d 180°); steam particles present.
- 375px: no horizontal overflow (scrollWidth == clientWidth == 375); nav CTA = 46px icon, number hidden, links hidden, mobile call float shown; hero/flip/menu/visit grids all collapse to one column.
- Zero em dashes in the file; no 24-hour visible times.
- Status pill logic confirmed against real ET clock.

## Images used (Pexels photo IDs — all visually verified as genuinely Jamaican, none in used_images.json's 25 prior IDs)
- 30746554 — hero: oxtail + rice and peas in bowls with a warming tray (atmosphere + steam)
- 6210449 — story: hands holding a bowl of fried sweet plantain at a family table
- 27556981 — flip card (Tue): brown stew oxtail with thyme
- 27556985 — flip card (Wed): jerk chicken with rice and peas + plantain
- 27568542 — flip card (Thu): curry chicken with potato
- 27556962 — flip card (every day): Jamaican beef patties
- 36857725 — menu feature: escovitch fish full plate with slaw
- 36878311 — craft band: jerk cooking over a charcoal drum with smoke

Orchestrator: please reconcile these 8 IDs centrally into used_images.json under city "City of Orange" (I did not edit the shared ledger).
