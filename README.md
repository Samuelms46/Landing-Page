# CINEMADISE Landing Page

## Overview
CINEMADISE is a concept landing experience for a Ugandan cinema ticketing platform. The prototype highlights value propositions for moviegoers and cinema operators, showcases product mockups, and captures early-access leads.

## Live Sections
1. **Home (`index.html`)**: Hero, dual CTA forms, benefits, product showcase, booking flow overview, and primary conversion call-to-actions.
2. **About (`about.html`)**: Brand story, mission, vision, values, and traction highlights.
3. **Team (`team.html`)**: Leadership spotlight, culture pillars, and recruitment CTA.
4. **Contact (`contact.html`)**: Direct contact details, inquiry form, FAQs, and partnership invitation.

## Project Structure
```
Landing Page/
├── images/
│   ├── Homescreen.png
│   ├── SAMUEL.jpeg
│   ├── Screenshot 2025-10-31 103718.png
│   ├── Screenshot 2025-10-31 103753.png
│   ├── Screenshot 2025-10-31 103840.png
│   ├── e-ticket.png
│   └── seats.png
├── about.html
├── contact.html
├── index.html
├── style.css
└── team.html
```

## Tech Stack
- **HTML5** for static markup
- **CSS3** for layout and visual design (`style.css` plus inline page-specific styles)
- **Vanilla JavaScript** for CTA toggling and submission stubs (`index.html` footer script)

## Getting Started
1. Clone or download the repository.
2. Open `index.html` in a modern browser to explore the landing experience.
3. Navigate to `about.html`, `team.html`, or `contact.html` for the additional sections.

## Design System Highlights
- Color palette anchored on warm neutrals (`#6C4324`, `#974420`, `#EE481A`, `#FCFCFC`).
- Typography: Inter family with emphasis weights for headings and CTAs.
- Components: Responsive navigation, card grids, CTA forms, stat bands, and gradient hero banners.

## Assets
All imagery lives under `images/` and is optimized for static use in the prototype. Replace with production-ready assets before launch.

## Two-Day Action Plan
1. **Consolidate Styles**: Move the inline `<style>` blocks from `about.html`, `team.html`, and `contact.html` into `style.css`, then link the stylesheet on every page for consistency and easier maintenance.
2. **Fix Audience Toggle Bug**: Update `switchAudience` in `index.html` to accept the click event explicitly instead of relying on the global `event` object (`index.html:377-388`).
3. **Close Home Wrapper**: Add the missing closing `</div>` for the `#home-page` container before the footer to keep the DOM well-formed (`index.html:34-314`).
4. **Hook CTA Targets**: Align all "Get Early Access" anchors with an actual `id` on the CTA section or adjust the link target accordingly (`about.html:424`, `contact.html:74`, `team.html:74`).
5. **Mobile Navigation Parity**: Replicate the mobile menu button and toggle script from `index.html` across the secondary pages so navigation works on small screens (`style.css:67-123`, `index.html:372-374`).
6. **Form Handling Roadmap**: Replace the alert-based stub with either a backend endpoint or a service like Formspree, capturing the fields defined in each form.

Staying focused on the action plan above will bring the prototype to a polished, presentation-ready state within the remaining two days.
