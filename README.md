# LSPU Heritage Navigator — Website

A 14-page website about Laguna State Polytechnic University (LSPU) and its four campuses,
with four interactive data-structure and algorithm modules. No server or internet connection
is needed to view it.

## How to open
1. Unzip the folder.
2. Double-click `index.html` (or any other page) to open it in Chrome, Edge, Safari or Firefox.
3. Use the top menu to move between pages.

Every page is a single self-contained file (styles, scripts, photos and data are all built
in), so any page also works on its own — for example in a chat preview or when emailed.

## Pages
| Page | File |
|---|---|
| Home | `index.html` |
| About LSPU (vision, mission, core values, pledge, seal) | `about.html` |
| History (1952 – today, by era) | `history.html` |
| Campuses overview | `campuses.html` |
| Siniloan Campus | `campus-siniloan.html` |
| Sta. Cruz Campus | `campus-sta-cruz.html` |
| Los Baños Campus | `campus-los-banos.html` |
| San Pablo Campus | `campus-san-pablo.html` |
| Contact | `contact.html` |
| Developers (team photos with name and role) | `developers.html` |
| Module A · History BST | `bst.html` |
| Module B · Campus Network (graph) | `network.html` |
| Module C · BFS vs DFS | `traversal.html` |
| Module D · Sorted Timeline | `timeline.html` |

## The four DSA modules
- **A · BST**: milestones keyed by year. Search (shows path + comparisons), insert,
  in/pre/post-order traversals, balanced vs chronological build (height 5 vs 17).
- **B · Graph**: 4 campuses as vertices, undirected edges, adjacency list + matrix.
- **C · BFS vs DFS**: choose a start campus, step or run both side by side; queue vs stack
  shown live; visit order and comparison table at the end.
- **D · Sorting**: shuffle, then Insertion / Bubble / Selection / Merge sort, ascending or
  descending. Each event card keeps its own photo while sorting (records move as a whole).

## Design notes
- **Style:** clean and organic. A white sticky header, a full-bleed photo hero, cream and white
  sections, rounded white cards with soft shadows, pill badges above headings, and a forest-green
  footer with a subtle wave pattern.
- **Colours:** leaf green `#4A7C2C` (buttons, links, icons), forest `#1A3D0F` (headings, footer),
  earth brown `#6B5744` (secondary button), cream `#F5F5F0` / `#FAFAF5` backgrounds, mint-to-cream
  gradient on the call-to-action, gold `#FFB800` stars. Every text colour meets the 4.5:1 contrast
  minimum (white on green 4.99:1, body text on cream 9.42:1, footer text 9.08:1).
- **Type:** Outfit for headings and body text (loaded from Google Fonts; falls back to system
  sans-serif fonts when offline).
- **Accessibility:** skip link, visible keyboard focus, SVG icons instead of emoji, 44px minimum
  touch targets, keyboard-operable tree and graph nodes and spotlight thumbnails (arrow keys,
  Home and End), an adjacency list/matrix as the accessible view of the graph, a contact form with
  inline errors and a linked error summary, and a photo viewer that traps and returns focus.
- **Layout:** 1280px maximum width. Breakpoints at 1180px (drawer menu), 1024px and 640px. Text
  keeps a comfortable margin from the screen edge (48px each side on desktop, 32px on tablets, 20px
  on phones).
- **Homepage order:**
  1. Hero: photo, badge, headline and two buttons.
  2. About split: checklist, floating "since 1952" stat card, plus vision and mission cards.
  3. The four campuses as service cards: photo, icon, title, text and Learn more.
  4. The four interactive modules.
  5. The five names of LSPU: a card with a round photo, a "Name 1 of 5" step label and five
     photo thumbnails.
  6. A mint-gradient call-to-action.
- **Inner pages:** a photo banner with the page title and a short intro, plus the same cards,
  buttons, chips and footer.
- **Footer:** brand and an email box that opens the Contact page with the LSPU address filled in,
  Explore, Modules, Contact details, and legal links.
- **Motion:** soft scroll reveals (fade + rise, staggered). Cards lift on hover and photos zoom
  gently inside their frames. Pages fade in, and the header gains a shadow when you scroll. Nothing
  autoplays. With reduced motion turned on, content appears in its final state and scrolling is
  instant.

Further design notes are in `design-system/lspu-heritage-navigator/MASTER.md`.

## Photos and the seal
The official LSPU seal and all campus, history and team photos supplied for this project are
built into the pages. The LSPU seal/logo is a registered trademark of the university; use it
with the university's permission.

Order used for any photo not supplied: an openly licensed web photo (credited on the page) →
a plain placeholder in the campus colour (team members show their initials until a portrait
is supplied).

## Sources
Content is based on the official LSPU website: Historical Development, University Seal,
Vision/Mission, Group Values & Performance Pledge, and each campus's program list
(lspu.edu.ph). Check contact details and program offerings against the latest official pages
before publishing.

## Contact form
The form checks the inputs and shows a confirmation. It does not store or send data — a
page viewed locally has no server to send it to.
