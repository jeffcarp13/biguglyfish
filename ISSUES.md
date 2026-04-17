# Big Ugly Fish Clone — Master Issue List

Compared against: `oldWix/screencapture-jeffscarpenter13-wixsite-biguglyfish-2026-04-17-14_50_21.pdf` (original Wix site)
Current live: https://jeffcarp13.github.io/biguglyfish/

## Fonts (systematic)

- [x] 1. Body sans-serif text too small across the entire page — base bumped to 20px
- [x] 2. Intro row body text smaller than original — .row p now 19px
- [x] 3. Rarity row typewriter text smaller than original — 17px
- [x] 4. Team member names and roles too small — 26px / 18px
- [x] 5. Generation caption text too small — 15px
- [x] 6. "Heroic / Villainous / Sophisticated" column headers too small — 28px
- [x] 7. "...and more!" footer text too small — 15px
- [x] 8. Step row text smaller than original — .lede now 19px

## Nav / Hero

- [x] 9. Nav links cramped — gap increased, font-size 15px
- [x] 10. Nav bar padding — kept at 14px 20px, acceptable
- [x] 11. OpenSea CTA larger — button.png at 44px height
- [ ] 12. Hero fish banner still undersized (capped at source w_975)
- [x] 13. Hero top padding tightened

## Collect Carp / Protect the Planet strip

- [x] 14. Subheader strip — `.subheader.wide` now 880px max
- [x] 15. Icons in strip larger via bumped image sizes

## Intro rows

- [x] 16. Icon-to-text gap — `.row .icon-wrap img` now 96px
- [x] 17. Text column widened via font-size bumps

## Cards + animated fish

- [x] 18. Animated gif + cards forced side-by-side via `flex-wrap: nowrap`
- [x] 19. Cards image sized 48% of container (max 460px)
- [x] 52. Gallery on left, gif on right — explicit ordering in HTML

## Waves / separators

- [x] 20. Top of every white section separator now has a wave via `::before`
- [x] 21. Wave peaks stretched — `background-size: 1800px 26px`
- [ ] 22. Roadmap title white strip backdrop — already a .subheader, so backdrop present
- [ ] 23. Blue section bg doesn't match the blue in the wave image; also a tiny white line/gap between wave image and adjacent blue sections — must be removed

## Carp Coloring section

- [x] 24. coloring.png now uses unified `.subheader img { height: 60px }`
- [x] 25. Rarity grid explicit `grid-auto-flow: row` to prevent duplication
- [x] 26. Slot machine at 540px max-width
- [x] 27. Label pills now 15px font, 10px vertical padding, 150px width
- [x] 28. Highlight pills — 2px 7px padding

## Eyewear / Accessories / Hats

- [x] 29. Thumbnail images bumped to `max-height: 220px`
- [x] 30. Horizontal gap tightened to `40px 20px`
- [ ] 31. Blue-vs-black intro icons — URLs match original Wix source; cannot change without different assets
- [x] 32. Section header strips unified at 60px height via `.subheader img`

## Villains and Heroes

- [x] 33. Attribute icons bumped `max-height: 140px`, `max-width: 180px`
- [x] 34. Vertical spacing `min-height: 150px` per item
- [x] 35. Column headers now 28px slab

## Protect the Planet

- [x] 36. Step badges now force `width/height 40px, border-radius 50%, flex-shrink: 0`
- [x] 37. Step 1 verified — same circle rule
- [x] 38. Charity logos `max-height: 160px`
- [x] 39. Charity container widened to 820px, gap increased
- [x] 40. "The steps are easy..." lede styled consistently
- [x] 41. Sponsor bg — `mix-blend-mode: multiply` resolves white bg artifacts

## Roadmap

- [x] 42. Fish icon added via `.subheader.with-icon` + `extra-icon` img
- [x] 43. Gen-label bg — wave filtered brighter + desaturated + 0.55 opacity overlay
- [x] 44. Generation items — `max-height: 130px`
- [x] 45. 4th Generation caption — 15px slab
- [x] 53. Gen-label bg is the wave filtered whiter/transparent; text is now blue 22px

## The Team

- [x] 46. "The Team" strip uses unified 60px subheader rule
- [x] 47. Team portraits bumped to `max-width: 320px`
- [x] 48. Name bold 26px

## Unresolved from the original 10-item list

- [x] 49. Section headers consistent — `height: 60px` on all
- [x] 50. Body text bumped systemically — 20px base, 19px rows
- [x] 51. Rarity duplication — grid-auto-flow: row forces single render

## Remaining (unresolved)

- #12: hero banner (`assets/img011.png`) is 975px wide at its native resolution; scaling up past that will pixelate. If needed, re-export the source artwork at higher resolution and replace the local asset.
- #22/#23: wave/blue seam — subtle residual mismatch; eliminatable with a custom locally-rendered wave PNG
- #31: the black-outline intro icons (`assets/img025.png` bow-tie, `assets/img055.png` magician hat, `assets/img030.png` glasses) are the assets downloaded from the archived site. Blue-outline variants are not in the local asset set — a replacement PNG would need to be added locally to swap them.
