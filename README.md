# DoBu Martial Arts — HTML & CSS website

Open dist/index.html in any modern browser. No installation or build step is needed.
Keep the HTML files, styles.css and assets folder together. The downloadable ZIP places these at the top level.

## Pages
- index.html — homepage
- training.html — martial arts, junior training, self-defence and fitness
- timetable.html — weekly timetable; expandable daily schedules on smaller screens
- membership.html — all membership and training prices
- about.html — gym facilities and all six instructors
- community.html — expandable sample forum discussions
- account.html — demonstration registration form
- login.html — demonstration sign-in form
- member.html — sample membership dashboard
- contact.html — demonstration enquiry form

## What works
Page navigation, responsive layouts, keyboard focus, a skip link, expandable mobile navigation, daily schedules and community threads, and browser-native form validation. There is no JavaScript, framework or package dependency.

## What needs a backend
Real registration, login, secure password handling, stored memberships, plan changes, payments, enquiries and forum posting. Forms are marked demonstrations. Inputs intentionally have no name attributes, so their contents are not included in form submissions or URLs. The member area is a public sample page, not a protected account.

## Content notes
Prices, weekly class times, facilities and instructor names/qualifications come from pages 3–5 of the supplied DoBu Martial Arts assignment. Promotional descriptions and forum examples are proposed copy.

The assignment explicitly calls Basic, Intermediate and Advanced monthly plans. It does not explicitly state the billing period for Elite or Junior, so the website flags those periods for confirmation. The gym address, email, phone, course dates, membership terms and official social-media accounts were not supplied and have not been invented.

## Editing and assets
Edit page text in the relevant HTML file. Change shared design in dist/styles.css; the --db-* properties control the palette. Barlow Condensed headings and DM Sans body text load from Google Fonts, with local fallback fonts when offline.

The grayscale training image is AI-generated and depicts fictional adults, not the named instructors. It is included at dist/assets/martial-arts-training.jpg. Generation used the built-in image tool with this prompt:

Editorial black-and-white sports photograph of two fictional adult martial artists in white cotton gis and black belts practising a standing judo grip on dark training mats. Simple charcoal gym, strong side-window light, realistic anatomy and cloth, respectful training mood. Square composition with breathing room; no text, logos or watermarks.

This is the HTML/CSS website portion of the assignment. It does not replace the required technology report, formal design documents, testing records or evaluation report.

## Professional design upgrade

The upgraded site uses a full-width training photograph, image-led programme cards, an editorial gym section, stronger typography, a charcoal-and-vermilion palette, and consistent navigation, forms and footers across all ten pages.

All four images are AI-generated concept photography. They do not depict the actual named instructors or a verified physical gym. Images are stored locally in the assets folder and require no image-hosting service. The original grayscale image is retained; three new images add Muay Thai, karate and a gym interior. The new photographs were produced with the built-in image generation tool. Exact prompts:

{
  "mode": "built-in image_gen",
  "assets": [
    {
      "name": "hero-muay-thai",
      "prompt": "Use case: photorealistic-natural\nAsset type: original website hero photograph, 1536x1024 landscape.\nPrimary request: Two fictional adult athletes, one woman practising a controlled Muay Thai pad strike with an adult male pad holder in a premium charcoal industrial martial arts gym.\nScene/backdrop: Spacious charcoal gym, slate training mats, authentic training equipment kept visually quiet.\nStyle/medium: Premium editorial sports photography, documentary realism, believable skin and fabric detail, natural colour.\nComposition/framing: Subjects on the right half, with the left 45% darker clean negative space for a website headline. Frame both athletes' anatomy, pads, and gloves convincingly, a focused controlled training moment.\nLighting/mood: Subtle warm side lighting and soft daylight, composed and disciplined.\nColor palette: Muted charcoal, graphite, slate, restrained warm highlights, coherent premium sports campaign treatment.\nConstraints: Realistic anatomy, pads and gloves. Fictional adults only. No violence or injury. No logos, lettering, watermarks or identifiable named instructors. Photograph only, never a website screenshot."
    },
    {
      "name": "karate-training",
      "prompt": "Use case: photorealistic-natural\nAsset type: original website programme photograph, 1024x1024 square.\nPrimary request: A fictional adult woman in a crisp white karate gi practising a precise forward punch in a spacious dark dojo.\nStyle/medium: Premium editorial sports campaign photograph with documentary realism, natural colour, believable skin and fabric texture.\nComposition/framing: Authentic training posture, complete punching arm and hand in frame, enough room around the athlete for clean composition.\nLighting/mood: Natural side window light, focused disciplined atmosphere.\nColor palette: Muted charcoal, graphite and slate environment, restrained warm highlights, crisp natural white gi, coherent premium sports campaign treatment.\nConstraints: Realistic anatomy and hands. Fictional adult only. No logos, lettering, watermarks or identifiable named instructors. No violence or injury. Photograph only, never a website screenshot."
    },
    {
      "name": "gym-interior",
      "prompt": "Use case: photorealistic-natural\nAsset type: original website facilities photograph, 1536x1024 landscape.\nPrimary request: Architectural photograph concept for a premium martial arts and fitness gym, showing a broad clean matted training area in the foreground with weight racks and fitness equipment in a separate background zone.\nScene/backdrop: Spacious industrial gym with dark graphite finishes, slate training mats, warm wood accent, organised realistic equipment layout.\nStyle/medium: Premium architectural photography, realistic materials and perspective, documentary natural colour, coherent premium sports campaign treatment.\nComposition/framing: Wide landscape, broad open training floor foreground and clear separation of equipment zone at the back.\nLighting/mood: Soft daylight, subtle warm highlights, calm and disciplined.\nColor palette: Muted charcoal, graphite and slate with restrained warm wood.\nConstraints: No people. No logos, lettering, watermarks or identifiable named instructors. Photograph only, never a website screenshot."
    }
  ]
}

## Background consistency
All nine interior pages use the homepage's charcoal colour (#111718), with light text, muted green-grey secondary text and lighter charcoal cards. The homepage retains its existing sections and imagery.

## Code formatting

All HTML and CSS use consistent two-space indentation, LF line endings and readable line wrapping. HTML comments identify the shared header, main content and footer. CSS is divided into numbered sections, with each declaration on its own line. The favicon lives in assets/favicon.svg.

The .editorconfig and .prettierrc.json files preserve these conventions in compatible editors. Prettier 3.6.2 was used to format the source; it is optional for editing, and the website runs without it.


## Demonstration flow repairs on 6 October 2026

Sign in now uses required HTML patterns for the published sample credentials:
email `demo@dobu.example`, password `DoBuDemo2026`.
This is a browser-only demonstration check, not secure authentication. The
sample member page remains public and the constraints can be bypassed.

The four main Choose links use `account.html#plan-basic`, `#plan-intermediate`,
`#plan-advanced` and `#plan-elite`. CSS `:target` reveals the matching preselected
native dropdown and hides the default dropdown. The selection remains editable.
Keep all five option lists consistent when editing plans. No JavaScript, storage,
backend or additional HTML page is required or included. The fixed sample account
does not change its stored membership because no such storage exists.

See VALIDATION_NOTES.txt for test scope, validation results and limitations.
