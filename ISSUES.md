# Big Ugly Fish Clone — Master Issue List

Reference: `oldWix/screencapture-jeffscarpenter13-wixsite-biguglyfish-2026-04-17-14_50_21.pdf`
Live: https://jeffcarp13.github.io/biguglyfish/

## Hard bugs in the latest render (after rewrite)

- [ ] A1. NO waves rendered on ANY white section strip (Collect Carp, Carp Coloring, Eyewear, Accessories, Hats, Villains and Heroes, Protect the Planet, Roadmap, The Team). `::before`/`::after` pseudo-elements are not producing the wave PNG.
- [ ] A2. Generation label bars (2nd/3rd/4th Generation) have NO wave background — they are plain white pills. Original has wave-textured bars.
- [ ] A3. Rarity section STILL shows 6 rows instead of 3. Second set of rows pulls wrong images (eyewear: rainbow sunglasses, 3D-glasses). Replace CSS-drawn pills with the pre-made `labels.png` composite image — this is the user's hint.
- [ ] A4. Section header strips render at different widths — Carp Coloring narrow, Hats short, Roadmap wider, The Team wider. Not uniform despite `height: 50px`. Fix requires fixed strip dimensions AND bg-fill so the container is always the same.

## Section headers

- [ ] B1. Roadmap strip: I stacked a cluster of multiple small fish icons + Roadmap text instead of a single clean fish icon. Fix: use only ONE small fish icon.
- [ ] B2. The Team strip: same issue — cluster of tiny fish + text, not a single fish-trio icon.
- [ ] B3. Every strip must have uniform total height (content + top/bottom wave = same pixel height)

## Rarity section (Carp Coloring)

- [ ] C1. STOP rendering three separate label pills via CSS. Use pre-made `labels.png` composite.
- [ ] C2. Fish images (img047, img035, img050) should still render in rarity but NOT as a grid that can duplicate.
- [ ] C3. Text column ("No Matching Parts / 3 Color Fish" etc.) must NOT be in a grid that reflows.

## Protect the Planet

- [ ] D1. Step-2 badge renders as circle now ✓ (resolved in last pass)
- [ ] D2. Charity logos row 2 (Greenpeace, Oceana) are smaller than row 1 — make uniform max-height.
- [ ] D3. "Proceeds go to..." and "Owners of..." rows are cramped against the section boundary above. Add top padding.

## Roadmap

- [ ] E1. Gen-labels must use wave.png as background (lost during rewrite). Text should be visible over it — either darker text or the wave filtered lighter.
- [ ] E2. 4th Generation caption "Breed Your Fish" is currently blue — should be regular gray like other captions.
- [ ] E3. Gen items (Additional Accessories, Sidekicks, etc) captions are blue — should be dark gray.

## Hero

- [ ] F1. Hero banner has excessive left/right whitespace — original fills closer to edge.

## Content accuracy

- [ ] G1. The fish icon used for "Roadmap" strip should be the single `otherfish.png` (grey fish silhouettes) or a single colorful fish, NOT the multi-fish school icon which cascades.

## Charity layout

- [ ] H1. Currently: 3 top row + 2 bottom row. Original has 5 in mixed layout that fits tighter.

## Wave texture

- [ ] I1. Waves background must be stretched (fewer, taller peaks) to match original scale.
- [ ] I2. Wave must have top edge AND bottom edge on every white strip.
- [ ] I3. Wave color must match `#e5f0fe` (sampled from PNG blue areas).
