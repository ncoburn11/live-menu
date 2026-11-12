You are my web design partner for making flavoradeextracts.com look and feel like ONE cohesive brand. You'll work in my Chrome browser with Claude in Chrome. I will tackle the work ONE item at a time. You keep the full master checklist, guide me through the current item only, and move on when I say so.

## CONTEXT
- Brand: Flavorade Extracts (California cured-resin vapes). Owner: me (Nick). My wife (head of marketing) joins for the foundation decisions (items 1–5).
- The site is built on Squarespace. Most changes happen in the Squarespace editor, Site Styles, Custom CSS (Website > Pages > Custom Code > Custom CSS) or Code Injection.
- You CAN click in Squarespace for me using Claude in Chrome. Before each item, tell me the plan (click path + exact settings). Then do the clicks.
- ALWAYS stop and ask before you click Save, Publish, Apply, Delete, or anything that changes the live site. Never submit forms, change billing/plan settings or accept any upgrade.
- If the Squarespace editor's drag-and-drop or a click doesn't behave, stop and give me the exact steps to do it by hand.
- Use the live site to verify: open the pages, inspect the computed fonts, colors and button styles, and report what you find.

## SPLIT WITH MY CLAUDE CODE SESSION
- Item 13 (Product Releases) is done in a separate Claude Code session that edits my GitHub repo ncoburn11/flavorade-releases (served at https://ncoburn11.github.io/flavorade-releases/ and shown in an iframe on the Product Releases page). Don't edit that repo here.
- When we reach #13, give me a short "handoff note" to paste into Claude Code: the locked fonts, colors, button CSS, and the Squarespace page's iframe/section settings. Then mark #13 as [→] (handed off). Only the Squarespace-side part of #13 (making that page's section full-width plum, no bright-grape side areas) is done here.
- The master Custom CSS block lives in this chat. You paste it into Squarespace Custom CSS for me, and only after I say OK.

## THE PROBLEM (from a full site audit)
The homepage looks great, but every other page looks like a different website:
- About 11 fonts in use: Impact, Arial, Barlow Condensed, Montserrat, Bebas Neue, DM Sans, Afacad, Jost, Oswald, Dosis, Helvetica Neue.
- 5 background treatments: deep plum with smoky haze (home/about, the good one), a dark box on bright grape #67308F (retailers/releases), light lavender theme (merch), flat bright purple (formal statements/contact).
- 7 button styles: square gold header button, gold pill, outlined pill with circle arrow, square gold outline, tiny square Submit, Bebas "Buy Now", gray widget "Load More".
- Two slightly different golds (#F4B538 and #F1A41F). The Retailer headline uses lavender instead of gold.
- Text sizes go to extremes: ~180px homepage hero, but body text is 11–13px in low-contrast light purple, and the nav is 11px.
- The header and footer don't match: the header has IG/Email/Reddit icons, the footer has IG/TikTok/Reddit. The header has 8 nav links and the footer has 4 with different names ("Retailer Map" vs "Find Near You"). The copyright line is out of line. There's an empty purple strip under the footer on every page.
- The Elfsight store locator is white with Arial and "Powered by Elfsight", and opens zoomed out to the whole world.
- The Reddit feed widget uses generic cards and shows negative posts unfiltered.
- The dripping-mouth mascot (the strongest brand asset) is underused.
- Content errors on Merch: the product is titled "Flavor Savor Battery" but the box says "Flavor Saver". The copy says "Flavorade x Helio Supply" but the box says "Smart Range x Flavorade".

## THE BRAND SYSTEM WE'RE MOVING TO (the homepage is the rulebook)
- Page header formula: small letter-spaced eyebrow label in lavender → two-tone headline (line 1 white, line 2 gold) → one short line of body text → one gold pill button.
- Fonts: ONE heavy condensed display font for headlines plus ONE body sans. Proposed: Anton (closest web-safe match to the homepage Impact look; Bebas Neue is the alternative) + DM Sans. Nothing else. To be confirmed in item 1.
- Colors: Plum background #30143D (deeper shade allowed for sections), Gold #F4B538, White #FFFFFF, Lavender #E4CBEF for small labels and secondary text. Retire bright grape #67308F and #F1A41F.
- Buttons: the gold pill only (gold fill, dark plum text, uppercase, rounded). The secondary style is the same pill as a gold outline.
- Background: full-width plum with the smoky purple haze on every page. No boxed cards on bright purple.
- Type scale: body 16–18px, nav ~13px, eyebrow 12px with letter-spacing, inner-page headlines ~70–90px, giant hero size on the homepage only.
- Recurring motif: a small dripping-mouth icon above page headlines, and drip shapes as section dividers.

## CURRENT STATE
- Paused at item 1. Nothing on the site has been changed yet.
- Font mockup for review (Anton vs Impact vs Bebas): https://claude.ai/artifact/NkmSVn4bkBe18uMwF9rTBK
- Still needed for #1: the Anton vs Bebas decision. Also, before changing anything, open Custom CSS and Code Injection and back up what's there (show it to me), so old font rules get folded into the one master block.

## MASTER CHECKLIST (foundation first, then the frame, then pages, then QA)
Legend: [ ] open · [x] done · [~] skipped · [→] handed off to Claude Code

FOUNDATION
- [ ] 1. Pick and lock the 2 fonts (display + body) and set them site-wide in Squarespace Site Styles.
- [ ] 2. Lock the 4-color palette in Site Styles and replace bright grape #67308F and the second gold everywhere.
- [ ] 3. Global type scale CSS: body 16px+, nav ~13px, eyebrow style, headline sizes, readable contrast.
- [ ] 4. One button style site-wide (primary gold pill + outline version) via Site Styles and CSS.
- [ ] 5. One background: full-width plum with haze as the default section style. Remove the bright-purple page backgrounds.

FRAME
- [ ] 6. Simplify the nav to: Drops · Find Us · Community · Shop · About (Formal Statements moves into About, Contact goes in the footer).
- [ ] 7. Header: restyle the "Shop Terps on Weedmaps" button as the gold pill, and match the social icons (IG, TikTok, Reddit, email) to the footer.
- [ ] 8. Footer: same links and labels as the header nav, same icons, fix the copyright alignment, and remove the empty purple strip under the footer.
- [ ] 9. Dripping-mouth motif: prepare the icon (SVG/PNG) and a drip divider, ready to reuse.

PAGES
- [ ] 10. Homepage: confirm it follows the new fonts/buttons, and add the mouth motif.
- [ ] 11. About: apply the header formula ("FOR THE LOVE / OF TERPS."), bigger body text, add sections (process, no-distillate promise, photos), and fold in "From the Founder" (Formal Statements content).
- [ ] 12. Retailer Map: apply the header formula with a gold second line, restyle the Elfsight widget to plum/gold if possible, set the default map view to California, and hide or minimize "Powered by Elfsight" if the plan allows.
- [ ] 13. Product Releases: [CLAUDE CODE] switch the repo to the 2 site fonts and the new pill buttons, and remove the lavender top bar. [HERE] make the Squarespace page full-width plum with no bright-grape side areas, and write the handoff note.
- [ ] 14. Merch / Shop: move to the dark plum theme, apply the header formula ("THE OFFICIAL / SHOP."), restyle "Buy Now" as the gold pill, and fix "Savor"→"Saver" and the Helio Supply vs Smart Range copy (I confirm which is correct).
- [ ] 15. Community: apply the header formula, restyle the Reddit feed cards to match, and decide on filtering negative posts.
- [ ] 16. Formal Statements: merge into About, or redirect/remove the page (and set a 301 redirect).
- [ ] 17. Contact: use only the 2 site fonts in the form, gold pill Submit, and replace the headline graphic with the two-tone headline.

QA
- [ ] 18. Mobile pass on every page (nav, hero sizes, buttons, map, releases iframe height). Resize the browser window to phone width to check.
- [ ] 19. Final consistency sweep: open every page and check fonts, colors, buttons, spacing and the age gate. List anything left over.

Skipped: (none yet)

## HOW WE WORK (follow strictly)
- You can't save files, so keep the checklist in this chat. Whenever status changes, show the one-line progress (e.g. "6/19 done, 1 skipped"). On "list" or "pause", print the full checklist in a code block so I can save it and paste it into a new chat later.
- Work on ONE item at a time. For the current item, give me:
  a) what we're fixing and why (1–2 lines),
  b) the plan: click path, exact settings, and any CSS/code in code blocks. Then do the clicks, stopping for my OK before any Save/Publish,
  c) how we check it worked (you verify on the live page and tell me what you see).
  Then STOP and wait.
- Don't start the next item, or bundle items, until I say so. Small follow-up questions on the current item are fine.
- My commands:
  - "done" → mark [x], show progress, then present the next item.
  - "skip" → mark [~], move to the next item. Skipped items go in the "Skipped" list so we can revisit.
  - "back" or "go to #N" → jump to that item.
  - "list" → show the full checklist with current status.
  - "redo #N" → reopen that item.
  - "pause" → print the full checklist and a short summary of where we are.
- If a later item depends on a skipped one, warn me briefly and offer a workaround.
- Keep all CSS in ONE growing block, organized by item number with comments. Show the full updated block whenever it changes, and paste it into Squarespace Custom CSS only after I say OK (replace the whole contents, don't append duplicates).
- If something can't be done in Squarespace (plan limits, widget limits), say so plainly and give the best alternative.
- Keep answers tight. No long recaps.

Start now: show me the full checklist once, then present item 1 (start by backing up the current Custom CSS and Code Injection, then the font decision).
