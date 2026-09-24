# Career Tiger — Homepage Redesign (v2)

**Find the job that's right for you. Or get fit for the job you want.**

A visual-first, product-led homepage for Career Tiger. It's positioned as a career-readiness platform rather than another job portal.

- **Live v2:** https://captanjacksparr0w.github.io/careertigers-redesign/
- **Earlier concept (v1):** https://captanjacksparr0w.github.io/careertigers-redesign/v1/

![Hero](images/hero.jpg)

## Core idea: two journeys, colour-coded throughout

| Journey | Colour | CTA | Section |
|---|---|---|---|
| **Find your fit**: match on skills, personality, work style and goals | Tiger orange | Find My Right-Fit Job | *Find Your Fit* |
| **Get fit**: close the gap to the job you want | Fresh green | Get Job-Ready | *Get Fit* + tools |

## Page flow

1. **Hero**: two-line headline, one short supporting line, two CTAs (one per journey), and a custom hero image of a candidate at the centre of a Discover → Assess → Improve → Prepare → Hired path. Floating UI chips show fit score, skill gap and progress.
2. **Differentiator**: "More than a job platform." A side-by-side comparison: *Job portals: Find → Apply → Hope* vs *Career Tiger: Discover → Assess → Prepare → Apply → Grow*.
3. **Personalisation**: "Your career path shouldn't be one-size-fits-all." Eight profile dimensions orbit around *You*.
4. **Find Your Fit**: Profile → Career Tiger AI → right-fit roles with match % and the reasons behind each match. A toggle shows how a keyword match would miss them.
5. **Get Fit**: an auto-playing, clickable stepper: Target Job → Resume Analysis → ATS Score (animated gauge) → Skill Gap → Interview Prep → Expert Guidance → Job Ready.
6. **Get Ready for the Job You Want**: a grid of the seven tools, with small "AI" and "Human expert" labels.
7. **Your Next Career Move**: tabs for Start / Switch / New Role / Promoted. Each tab redraws the path Current You → Assessment → Skill Gap → Preparation → Target Role.
8. **How it works**: Assess → Discover → Improve → Apply → Grow, with a progress bar that fills across the steps.
9. **Trust**: partner names, stats and career-move stories.
10. **Final CTA**: "Your next career move starts here." with both CTAs.

Navigation: Jobs · Career Tools · Assessments · Counselling · Resources | Login · Get Started

## Custom images (made with ChatGPT image generation)

All three images share one brand look: midnight navy, tiger orange and green accents, warm cinematic light, and realistic Indian professionals. None of them contain text.

| File | Used in | What it shows |
|---|---|---|
| `images/hero.jpg` | Hero | Candidate at the centre of a five-step career journey |
| `images/interview.jpg` | Get Fit stepper, Mock Interviews card | A mock video interview with AI feedback cards |
| `images/counselling.jpg` | Get Fit stepper, Counselling card | A one-on-one session with a career counsellor |

## Before launch
- [ ] **Verify every number.** "20+ hiring partners", "12 industries" and "11+ courses" come from the current site. Replace them with confirmed platform stats, or remove them.
- [ ] Replace the carried-over testimonials with real, consented learner stories (photo + LinkedIn).
- [ ] Swap partner names for official logos, with permission.
- [ ] The profile, match % and ATS numbers in the demo UI are illustrative. Keep them clearly as product demos.
- [ ] Wire CTAs to real sign-up flows: *Find My Fit* goes to the profile/assessment, *Get Job-Ready* goes to target role + resume scan.

## Tech
A single static `index.html` with no framework, so it's easy to port into the Laravel Blade templates. It includes a mobile layout, reduced-motion support and alt text on all images.
