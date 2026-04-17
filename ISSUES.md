# Big Ugly Fish Clone — Master Issue List

Compared against: `oldWix/screencapture-jeffscarpenter13-wixsite-biguglyfish-2026-04-17-14_50_21.pdf` (original Wix site)
Current live: https://jeffcarp13.github.io/biguglyfish/

## Fonts (systematic)

- [ ] 1. Body sans-serif text too small across the entire page
- [ ] 2. Intro row body text smaller than original
- [ ] 3. Rarity row typewriter text smaller than original
- [ ] 4. Team member names and roles too small
- [ ] 5. Generation caption text too small
- [ ] 6. "Heroic / Villainous / Sophisticated" column headers too small
- [ ] 7. "...and more!" footer text too small
- [ ] 8. Step row text smaller than original

## Nav / Hero

- [ ] 9. Nav links cramped against hero (no breathing room)
- [ ] 10. Nav bar needs more vertical padding
- [ ] 11. OpenSea CTA should be larger / higher contrast
- [ ] 12. Hero fish banner undersized; original fills near edge-to-edge
- [ ] 13. Hero has too much top padding above banner

## Collect Carp / Protect the Planet strip

- [ ] 14. Subheader strip narrower than hero band (inconsistent widths)
- [ ] 15. Icons in that strip smaller than original

## Intro rows (school / gem / globe / vote)

- [ ] 16. Icon-to-text gap too wide
- [ ] 17. Text column too narrow, causing different line breaks

## Cards + animated fish

- [ ] 18. Animated gif wraps below cards; original has them side-by-side
- [ ] 19. Cards image slightly smaller than original
- [ ] 52. Force side-by-side placement in Collect Carp: left = gallery cards, right = animated gif

## Waves / separators

- [ ] 20. Top of every white section separator missing its wave (only bottom has one)
- [ ] 21. Wave peaks too dense; original has fewer, larger, stretched peaks
- [ ] 22. Roadmap title has no white strip backdrop
- [ ] 23. Blue section bg does not match the blue baked into Waves.png

## Carp Coloring section

- [ ] 24. coloring.png header width inconsistent vs other section headers
- [ ] 25. **HARD BUG**: rarity rows duplicated, render 6x instead of 3x
- [ ] 26. Slot machine image slightly undersized
- [ ] 27. SPECIAL / RARE / ENDANGERED label pills thinner / less tall than original
- [ ] 28. "X Color Fish" black highlight pills narrower than original

## Eyewear / Accessories / Hats

- [ ] 29. Thumbnail images ~50 percent undersized
- [ ] 30. Horizontal gap between thumbnails too large
- [ ] 31. Intro icons (glasses / bowtie / top-hat) are black outline; original shows blue outline
- [ ] 32. Section header strips render at different widths (inconsistent heights)

## Villains and Heroes

- [ ] 33. Attribute icons beside +1 / +2 undersized (~80-100px vs ~150px)
- [ ] 34. Vertical spacing between list items too tight
- [ ] 35. Column headers undersized

## Protect the Planet

- [ ] 36. **HARD BUG**: step "2" badge renders as oval instead of a circle
- [ ] 37. Verify step "1" badge renders as consistent circle
- [ ] 38. Charity logos smaller than original (~80px vs ~150-180px)
- [ ] 39. Charity layout wraps awkwardly; Greenpeace / Oceana drop to separate lines
- [ ] 40. "The steps are easy..." line has different indentation
- [ ] 41. Sponsor-section bg color subtly off from rest of blue

## Roadmap

- [ ] 42. **Missing**: Roadmap title strip has no fish icon (original shows colorful fish beside text)
- [ ] 43. Gen-label bars look washed out with wave bg
- [ ] 44. Generation items (gray silhouettes) undersized
- [ ] 45. 4th Generation (Breed Your Fish) caption smaller than original
- [ ] 53. Gen-label bg should be the wave filtered whiter/transparent (only showing lower half). If impossible, make text blue and larger.

## The Team

- [ ] 46. "The Team" header fish-icon cluster rendering small / inconsistent
- [ ] 47. Team member portraits ~180-200px; original is ~280-300px
- [ ] 48. Team member name bold weight not strong enough

## Unresolved from the original 10-item list

- [ ] 49. Section headers still not consistent in size / placement
- [ ] 50. Body text systemic sizing (flagged multiple times)
- [ ] 51. Rarity duplication (flagged as "second row should be removed") — same as #25

## Systemic themes

- Body font undersizing (#1-8, #50) — likely CSS specificity issue where element-level sizes override base
- Section header inconsistency (#24, #32, #49) — `max-width` alone does not unify different aspect ratios
- Image undersizing across attribute grids / team / charities (#29, #33, #38, #44, #47)
