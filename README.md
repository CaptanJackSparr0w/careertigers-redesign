# CareerTigers — Homepage Redesign Proposal

A redesign concept for [careertigers.com](https://careertigers.com) focused on looking **more appealing and more trustworthy** to students, parents and recruiters.

**▶ Live preview:** open `index.html` (or the GitHub Pages link in the repo's About section).

| Desktop | Mobile |
|---|---|
| ![Desktop](screenshots/after-desktop.png) | ![Mobile](screenshots/after-mobile.png) |

---

## Tagline — "Get your dream job"

**Recommended hero headline:** **From campus to your dream job.**

Alternatives:

| Tagline | Best used for |
|---|---|
| From campus to your dream job. | Hero headline (used in the redesign) |
| Your dream job is closer than you think. | Closing CTA section (used in the redesign) |
| Roar into your dream job. | Social media / ads (plays on the tiger brand) |
| Learn. Prepare. Get your dream job. | Brochures, posters, campus banners |
| Dream it. Prepare for it. Get hired. | Video / event backdrop |

---

## What's wrong with the current page (audit)

### Trust issues (highest priority)
1. **Browser tab says "Career Tigers - Laravel"** — the framework name looks unfinished. No meta description or social preview either.
2. **Testimonials look like placeholders** — generic employers ("Tech Solutions Inc.", "Global Tech Systems", "FinServe Corp"), no photos, no LinkedIn links. Visitors notice this quickly and it hurts credibility.
3. **Masterclass speakers have generic names and no photos** (e.g. "Sarah Johnson", "Michael Chen"). Use real coaches with photos and credentials.
4. **Hiring-partner strip has errors**: "Star Health Insurance" appears twice, typos like "AAJ Suplychain" and "nExt Educationight", and names are shown as grey text pills instead of real logos.
5. **Mixed messaging**: hero says "campus learners", footer says "online learners".
6. **No hard numbers anywhere** (learners placed, average package, partner count). Proof beats adjectives.
7. **Stock-looking hero image** plus a "D." / "a" artefact in the job-match card.

### Design / UX issues
8. **Purple + orange gradient mix** clashes with the orange/navy logo and looks like a generic template.
9. **The same journey appears twice**: "Learn → Practice → Get Ready → Get Hired" and "Assess → Build → Match → Convert". Pick one.
10. **Industries section is a 12-card wall** with around 36 chips. Very long, hard to scan.
11. **Mascot emoji after every heading** repeats and starts to look like clutter.
12. **Tool cards all say "View"**, which is a weak call to action. There's also no grouping or priority.
13. **FAQ shows numbered questions** with answers loaded late. Plain accordions are simpler.
14. **No secondary nav action** (Log in) for returning learners.

---

## What the redesign changes

| Area | Change | Why it helps |
|---|---|---|
| Brand palette | Tiger orange + deep navy on warm cream; purple removed | Matches the logo, and navy reads as reliable and established |
| Typography | Fraunces (serif display) + Figtree (body) | Serif headings feel established and credible, not "template" |
| Hero | New tagline, one clear primary CTA, social-proof row, live "career dashboard" card instead of stock photo | Shows the product and the outcome at a glance |
| Proof | Stats band (20+ partners, 12 industries, 8 tools, 11+ courses) — all from the current site | Concrete numbers build trust |
| Partners | Deduplicated, typos fixed, calm grey marquee (pauses on hover) | Looks polished (swap in real logos) |
| Journey | Two duplicate flows merged into 4 steps: Assess → Build → Practice → Get hired | One clear story |
| Tools | "Try it →" CTAs, "Most used" tag, Prepare/Apply filter tabs | Easier to scan and act on |
| Stories | Featured story layout with a clear "from → to" career move | Outcome-focused; ready for photos + LinkedIn |
| Industries | Interactive pills: pick an industry to see its roles | 12 cards become one compact block |
| Learning | Masterclasses and certifications merged into one section | Shorter page, less repetition |
| FAQ | Native accordion, support email beside it | Fast, accessible |
| Contact | Dark CTA band with callback form + privacy note ("We never share your details") | Reassurance at the moment of conversion |
| SEO | Proper `<title>`, meta description, Open Graph tags | Better search and share previews |
| Accessibility | Reduced-motion support, alt text, labelled inputs, strong contrast | Inclusive and more professional |

## Before launch — content checklist
- [ ] Replace testimonials with **real, verified** learners (photo, employer, LinkedIn link, consent)
- [ ] Add real photos + credentials for masterclass speakers
- [ ] Replace partner names with official logos (with permission)
- [ ] Add real outcome numbers if available (learners placed, avg. package, placement rate)
- [ ] Fill in the "Is my data safe?" FAQ answer + link the Privacy Policy
- [ ] Confirm the correct spelling of "nExt Educationight" (removed from the strip for now)

## Tech
Single static `index.html`, no build step, no framework. Styling uses CSS variables, so it can be ported into the existing Laravel Blade templates section by section.
