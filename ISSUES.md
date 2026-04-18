# Big Ugly Fish Clone — Visual Differences

Original (reference): `biguglyfish - orig.pdf` (the authoritative design, Wix chrome stripped)
Live (current): `screencapture-jeffcarp13-github-io-biguglyfish-2026-04-17-20_34_26.pdf`

## Hero (About)

- [ ] H1. Original hero is a **horizontal** composition: "Big. Ugly. Fish." stacked on the LEFT, 8-fish cluster on the RIGHT, filling the full blue section width edge-to-edge. Current centers a single image with excess left/right whitespace and stacks title above fish.
- [ ] H2. Original title font appears slab/serif ("Big." / "Ugly." / "Fish." on 3 lines left-aligned). Current is identical styling but wrongly centered and fish layout is different.

## Section header strips (all of them)

- [ ] S1. **No wave top/bottom borders** are visible on any white strip in the live render (Collect Carp, Carp Coloring, Eyewear, Accessories, Hats, Villains & Heroes, Protect the Planet, Roadmap, The Team). Original shows pale-blue wavy edge PNG on top and bottom of each white strip.
- [ ] S2. Strip height inconsistent in live render. Original: every strip is the same compact height (~60–70px of white between the two wave borders).
- [ ] S3. Collect Carp + Protect the Planet strip icons: original uses a small school-of-fish icon for "Collect Carp" and a globe-in-hands icon for "Protect the Planet". Current: same icons but render size + spacing differ; pairs do not sit on one compact row.

## Collect Carp. / Intro rows

- [ ] I1. Original intro icon sizes are smaller (~40px). Current icons render larger (~60–70px) making rows bulky.
- [ ] I2. Original positions "cards collage" + "animated rainbow fish" side-by-side UNDER the 4 intro bullet rows, similarly sized (~45% each). Live render: animated fish appears much wider than cards.

## Carp Coloring (Rarity)

- [ ] R1. Original shows **3 rows** only: SPECIAL, RARE, ENDANGERED — each row is `[label-pill] [small fish img] [text column]`.
- [ ] R2. Live render shows **6 rows** — the bottom 3 (Villainous / Heroic / Sophisticated) are leaking V&H content into the Rarity section with eyewear images (rainbow sunglasses, 3D glasses, blue+green fish). This is a serious bug.
- [ ] R3. Rarity label pills (SPECIAL/RARE/ENDANGERED) colors: green / light-blue / red-orange — original uses pre-made label PNGs; live render shows flat CSS pills with slight differences in color saturation.
- [ ] R4. Text highlight boxes (e.g. "3 Color Fish.", "2 Color Fish.") are black-bg/white-text inline chips — preserve this; live looks OK.

## Eyewear

- [ ] E1. Original: 2 rows × 3 items = 6 eyewear items (black glasses, blue sunglasses, plain eyes; heart glasses, monocle, pirate eyepatch). Live: same 6 but the 3rd row on live PDF accidentally shows eyewear in the rarity section above; the Eyewear section itself looks correct.
- [ ] E2. "Big Ugly Fish are randomly given 1 of 18 different sets of eyes..." intro icon (small glasses icon) appears smaller in original.

## Accessories

- [ ] A1. Original: 2 rows × 4 items = 8 accessories (MOM tattoo, tie, mirror, cigar / joint, bowtie, pipe, megaphone — plus one more, total 8 shown on page 3). Live: 3 rows × 3 items = 9 items (adds pink tongue, face mask which are actually from a different set).
- [ ] A2. Order: original row 1 = MOM tattoo / tie / mirror / cigar; row 2 = joint / bowtie / pipe / megaphone. Live rearranges.
- [ ] A3. Intro icon (feather/bowtie) is smaller in original.

## Hats

- [ ] Ha1. Original: 3 rows × 3 items = 9 hats (bowler / cowboy / rainbow, captain / rasta / devil-horns, crown / halo / viking). Live: matches 9 items but column widths / gaps differ.
- [ ] Ha2. Intro icon (top-hat) smaller in original.

## Villains & Heroes

- [ ] V1. Original: 3 columns (Heroic, Villainous, Sophisticated), each with ~9 items listed vertically with `+N` or `-N` badge to the right of each icon, then "...and more!" caption at bottom.
  - Heroic list (original, top to bottom): crown +1, halo +2, protect-planet sign +2, life-ring +2, face mask +1, stethoscope +2.
  - Villainous list: devil horns +2, viking helmet +1, pirate eyepatch +2, MOM tattoo +2, monocle +1, vampire mouth +2.
  - Sophisticated list: bowler +2, bowtie +2, monocle +2, pipe +1, tie +1, cigar +1, pink tongue −1.
- [ ] V2. Live render has 6 items per column (truncated or reordered) and the entry ordering differs from original.
- [ ] V3. Intro-row icons (bowtie, gauge) appear smaller in original.

## Protect the Planet

- [ ] P1. Original: 2 intro rows (sunrise icon / proceeds text; VOTE icon / owners text) — live has the same but at different icon sizes.
- [ ] P2. Step badges (1 green circle, 2 blue circle) — original and live both show circles; live may render slightly oval on some viewports.
- [ ] P3. Charity logos: original arranges **5 logos in 2 rows** with row 1 = Defenders of Wildlife + Wildlife Conservation Society (2 big), row 2 = Greenpeace + WWF stacked with Oceana to the left; the logos sizes in original are larger and centered under the Wildlife Conservation text block. Live: row 1 = Defenders, Wildlife Conservation, WWF (3); row 2 = Greenpeace, Oceana — logos smaller than original row 1.
- [ ] P4. Original appears to visually emphasize WWF + Wildlife Conservation as the two biggest logos; live has them uniform-sized.

## Roadmap

- [ ] Rm1. Original roadmap header strip uses a **single colorful school-of-fish icon** + "Roadmap" slab text. Live strip icon reads similarly but wave borders missing.
- [ ] Rm2. Generation-label bars ("2nd Generation", "3rd Generation", "4th Generation") in original are **wide rounded pills** with subtle wave texture; live renders them as flat white pills with no texture.
- [ ] Rm3. Gen items: captions ("Additional Accessories", "Sidekicks", "Breed Your Fish", etc.) in original render dark gray. Live renders captions blue (inheriting link color?).
- [ ] Rm4. Gen items 2nd Gen: 3 items; 3rd Gen: 2 items; 4th Gen: 1 item — structure matches.
- [ ] Rm5. Icon artwork for gen items renders smaller in original relative to caption.

## The Team

- [ ] T1. Original: 3 members in a row (Jeff / Scott / Is This You?) with fish portrait above bold name + role caption. Live matches.
- [ ] T2. Strip icon for "The Team" in original is a small trio of tiny fish + slab-serif "The Team". Live renders a cluster of fish too small; the strip wave borders are missing.
- [ ] T3. Between Villains & Heroes "...and more!" row and Protect the Planet strip, original has a tiny black fish-swirl ornament. Live omits it.

## Waves / background

- [ ] W1. Wave PNG `img028.png` is loaded in CSS (`::before`/`::after`) but appears invisible in live render. Likely the pseudo-elements are being clipped by the strip's `overflow: hidden` combined with an icon larger than the strip, OR the PNG has transparent fill so the `background-color: var(--bg-blue)` is covering it. Needs verification: waves should be clearly visible as a row of blue wavy peaks along top and bottom of every white strip.
- [ ] W2. Original wave scale: approx 8–10 peaks across the viewport width at desktop; live currently shows none.

## Typography

- [ ] Ty1. Section header text uses Special Elite (typewriter slab) — matches.
- [ ] Ty2. Body text uses sans-serif — matches, but original body copy is slightly smaller (14–15px) vs live 16px, making live intro rows feel larger.

## Nav

- [ ] N1. Original Wix wrapper has "About / Colors / Attributes / Conservation / Roadmap" + blue "Buy on OpenSea" pill on right. Live matches structurally. OK.
- [ ] N2. Live nav is sticky — acceptable modernization, not in original, but doesn't conflict visually.

## Priority summary

1. Fix waves on strips (W1).
2. Hero layout: title LEFT, fish cluster RIGHT, edge-to-edge (H1).
3. Rarity section rendering the extra 3 V&H rows (R2) — THIS IS A BUG.
4. Villains & Heroes list content accuracy (V1, V2).
5. Accessories count and order (A1, A2).
6. Gen label bars need wave texture (Rm2).
7. Gen captions color fix — dark gray, not blue (Rm3).
8. Charity logo sizing uniformity (P3, P4).
