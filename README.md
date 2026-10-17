# SharkGYM

A responsive website for a fictional gym, created as part of the **AI-Assisted Front End Development Practicum**. The project follows the supplied landing-page reference and extends its visual style across five pages.

## Technologies

- Semantic HTML5 and external vanilla CSS
- Flexbox layouts and responsive media queries
- Roboto imported from Google Fonts
- A keyboard-accessible, CSS-only hamburger menu

No JavaScript, CSS Grid, frameworks, or build dependencies are used.

## Pages

| Page | File | Description |
| --- | --- | --- |
| Home | `Pages/Index.HTML` | Gym introduction, benefits, quotation, and membership links |
| Programs | `Pages/Programs.HTML` | Training options and program cards |
| Trainers | `Pages/Trainers.html` | Illustrative trainer profiles |
| Subscriptions | `Pages/Subscriptions.HTML` | Example membership plans and contact links |
| Contact | `Pages/Contacts.HTML` | Fictional contact details and a clearly marked demo form |

In-page buttons use GET forms to navigate without JavaScript; the navigation bar uses links. Membership buttons open the subscription or contact page. There is no registration backend. The contact form does not send or store information, and its send button is disabled.

## Project structure

```text
GYM-website/
├── Pages/              # Five HTML pages
├── CSS/
│   ├── shared.css      # Palette, typography, navigation, footer, and shared layouts
│   ├── Index.css
│   ├── Programs.css
│   ├── Trainers.css
│   ├── Subscriptions.css
│   └── Contacts.css
├── Images/             # Local image assets
└── README.md
```

## Run locally

Open `Pages/Index.HTML` in a browser. No installation or build step is required. Alternatively, serve the repository root with an existing static-file server and open `/Pages/Index.HTML`.

Keep filenames and path capitalization unchanged when hosting on a case-sensitive server. An internet connection is needed to load Roboto; a sans-serif fallback is provided.

## Design and responsive behavior

The shared palette uses `#1F2937` for dark backgrounds, `#F9FAF8` for light text, `#E5E7EB` for secondary text and the quote background, and `#3882F6` for buttons and the main call to action. Hero headings use 48px extra-bold text on desktop, information headings use 36px extra-bold text, and the quotation uses 36px light italic text.

Flexbox reorganizes content at smaller widths. Images use fluid widths; the hero preserves its aspect ratio, while cards use `object-fit: cover` to fill consistent image areas without stretching. The portrait card has a custom crop position to keep the subject visible. These choices suit the different layout roles of hero and card images.

Before submission, check every page at 375px, 768px, and 1200px or wider. Verify image crops, horizontal overflow, menu opening and closing, keyboard focus, and navigation links. These checks require an actual browser; source validation alone does not establish visual correctness.
