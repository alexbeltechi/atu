# Figma / Parabola mood-board content formats

*2026-11-19 · reusable system for fictional and real creator personas*

The purpose is to test a **general-use brand mood-board creator**: one person's visual identity, texts and assets should adapt across many editorial formats without hardcoded layouts or a single voice. ATU is the first test case, not the exclusive user.

## Twelve archetypes to compose

| # | Format | Copy density | Typical image/treatment | Example from [idea bank](idea-bank.md) |
| --- | --- | --- | --- | --- |
| 01 | Brand statement | 2–5 words | Wordmark over color field | „Mai departe.” |
| 02 | Portrait quote | One sentence | Close portrait, small high-contrast caption plaque | „Nu orice lucru frumos are stil.” |
| 03 | Question | One question | Direct-gaze or off-axis portrait; interactive story | „Tu când știi că e suficient?” |
| 04 | Personal story | Headline + caption | Documentary portrait or place | „Am crezut că asta îmi doresc.” |
| 05 | Mini essay | Title + 2–3 sentences | Photograph + editorial text | „Ai ajuns mai departe. Ce urmează?” |
| 06 | Carousel cover | Bold headline | Graphic layout, natural texture | „Diferența dintre stil și trend” |
| 07 | Talking head | Subtitles / 1–2 lines | Mid-sentence face, natural expression, phone-camera angle | „Mă gândeam azi la ceva…” |
| 08 | Photo diary | Minimal text / date | Several images, restrained caption | „În ultima vreme.” |
| 09 | Behind the scenes | Casual caption | Process images, hands, objects | „O idee care prinde contur.” |
| 10 | Opinion | Provocative statement | High-contrast editorial typography | „Să fii ocupat nu e o realizare.” |
| 11 | Project reveal | Title + description | Work, environment, detail photography | „Ce am schimbat și de ce.” |
| 12 | Invitation | One next step | Portrait, object or flat color | „Hai să facem ceva împreună.” |

## Content fields per component

```yaml
persona:             # fictional prototype or consenting real person
brand_name:          # "Atu" as a working example
format:              # 01..12
platform:            # story, post, reel, carousel
aspect_ratio:        # 9:16, 4:5, 1:1
headline:            # may be empty
body:                # may be empty
eyebrow:             # optional label/date/category
cta:                 # optional
image:               # supplied portrait, scene, or no image
image_focal_point:   # normalized x,y (for safe cropping)
font_display:        # font family/style/weight
font_body:
color_background:
color_text:
color_accent:
text_backplate:      # none / white / dark / translucent
text_align:          # left / center / right
logo_treatment:      # none / wordmark / minimal symbol
```

A component should work when `headline` is only two words, when body text is long, and when there is *no text*. Use a unified design system; don't create twelve unrelated styles.

## From the current Figma experiment

- Big close-up portrait; natural face, mid-word or thoughtful expression, rather than stock-fashion posing.
- Minimal black text on small white rounded plaques; sometimes one plaque per line.
- Dark navy / cream / white as **explorations**, not finalized colors.
- A wordmark-only tile can anchor the collection.
- Photo is the hero; typography should feel placed with intent, not like a generic quote template.
- Avoid heavy gradients, AI-looking stock imagery, noisy branding, inflated luxury signals and needless ornament.
- For text, test Instrument Sans, Onest and similar restrained sans serifs; font choice isn't fixed.
- Keep Romanian diacritics and measure wrapping in the actual font.
- Don't put text over eyes or important facial expressions by default; breaking this can be an intentional artistic choice.

## Test matrix

Test at least:
- Person with long hair / short hair; dark / light backgrounds; indoor / outdoor scenes.
- Three-word headline / one-sentence headline / two-line paragraph.
- Short and long Romanian words with diacritics.
- Portrait crops with space above, below and beside the face.
- Reels with burned-in subtitles and safe zones.
- Story CTA or poll overlay; carousel with multiple pages.

## Working with actual people

Only use approved image assets and real statements. A fictional line like „Am avut nevoie de ani să înțeleg asta” must not be attributed to a photographed real person without consent. The brand system should not force an artificial persona on the subject.
