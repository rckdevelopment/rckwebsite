# RCK Development — DESIGN.md

## Purpose
This design system is based on the structural logic of the All Reno Framer site, adapted for **RCK Development** with a focus on **lead generation for calls and estimate requests**.

The source site uses a simple conversion funnel:
- hero with one primary CTA
- service overview
- portfolio/work samples
- educational content
- testimonials
- warranty/protection section
- FAQ section
- final request-a-quote CTA

RCK should keep that flow, but the tone should feel more credible, more local, and more premium for Bay Area homeowners.

---

## Product Goal
Generate:
- estimate requests
- phone calls
- consultation bookings

The site is not meant to be artistic or experimental.
It is meant to make homeowners feel:
- this company is legitimate
- this team is organized
- this contractor can be trusted inside my house
- I should request an estimate now

---

## Brand Positioning
RCK Development should feel:
- professional
- licensed
- reliable
- clean
- practical
- premium but not flashy

Avoid looking:
- cheap
- overly corporate
- futuristic tech startup
- generic handyman marketplace

Tone:
- calm
- direct
- trustworthy
- local
- experienced

---

## Design Principles
1. **Trust before beauty**  
   Every section should increase confidence.

2. **One action per screen**  
   The user should always know the next step.

3. **Real proof beats clever design**  
   Use real project photos, real locations, real testimonials.

4. **Clarity wins**  
   Short copy, clean spacing, obvious hierarchy.

5. **Repetition converts**  
   Repeat the estimate CTA throughout the page.

---

## Audience
Primary audience:
- homeowners in the Bay Area
- people considering kitchen remodels, bathroom remodels, ADUs, additions, and full-home renovations
- homeowners comparing 2 to 5 contractors

What they worry about:
- cost surprises
- delays
- poor communication
- messy job sites
- permit issues
- hiring the wrong contractor

What they want to feel:
- this team is responsive
- this team knows process
- this team does quality work
- this team is worth contacting

---

## Visual Direction
The overall visual language should be:
- modern contractor
- premium local service business
- clean editorial layout
- image-led but not image-dependent

This is not a luxury fashion aesthetic.
This is not startup minimalism.
This is **high-trust residential construction marketing**.

---

## Color System

### Core Palette
```yaml
color:
  brand:
    primary: "#2F6FED"
    primary_hover: "#2459C7"
    primary_soft: "#EAF1FF"
  neutral:
    black: "#111111"
    text: "#1A1A1A"
    text_muted: "#6B7280"
    border: "#E5E7EB"
    surface: "#F7F7F7"
    white: "#FFFFFF"
  semantic:
    success: "#1F7A4D"
    warning: "#C98900"
    danger: "#C23B3B"
```

### Usage Rules
- Use **blue** as the primary action color.
- Use black and deep neutral colors for headings.
- Use light gray backgrounds to separate sections.
- Keep color count low.
- Never use more than one strong accent color on the same page.

### Ratio
- 70% white
- 20% black / dark gray
- 10% blue accent

---

## Typography

### Font Stack
```yaml
typography:
  family:
    heading: "Inter, ui-sans-serif, system-ui, sans-serif"
    body: "Inter, ui-sans-serif, system-ui, sans-serif"
```

### Scale
```yaml
type_scale:
  hero: "56px / 1.05 / 700"
  h1: "48px / 1.1 / 700"
  h2: "36px / 1.15 / 700"
  h3: "28px / 1.2 / 600"
  h4: "22px / 1.3 / 600"
  body_lg: "18px / 1.7 / 400"
  body: "16px / 1.65 / 400"
  small: "14px / 1.5 / 400"
  label: "13px / 1.4 / 600"
  button: "16px / 1 / 600"
```

### Typography Rules
- Headlines should be short and bold.
- Body text should never feel dense.
- Use sentence case, not all caps.
- Avoid decorative font pairings.
- Keep paragraphs to 2–4 lines when possible.

---

## Spacing System
```yaml
spacing:
  4: "4px"
  8: "8px"
  12: "12px"
  16: "16px"
  20: "20px"
  24: "24px"
  32: "32px"
  40: "40px"
  48: "48px"
  64: "64px"
  80: "80px"
  96: "96px"
  120: "120px"
```

### Layout Spacing Rules
- Section padding: `96px` desktop, `72px` tablet, `56px` mobile
- Card padding: `24px` or `32px`
- Vertical rhythm should feel generous
- Keep more spacing around CTAs and form blocks

---

## Grid and Layout
```yaml
layout:
  container_max: "1200px"
  container_reading: "760px"
  grid_columns_desktop: 12
  grid_gap: "24px"
  radius_sm: "8px"
  radius_md: "12px"
  radius_lg: "16px"
  radius_xl: "24px"
  shadow_sm: "0 1px 2px rgba(0,0,0,0.04)"
  shadow_md: "0 8px 24px rgba(0,0,0,0.08)"
```

### Structure Rules
- Use 2-column layouts for hero and proof sections.
- Use 3-column grids for service cards and trust features.
- Use wide image blocks for project showcases.
- Keep all content left-aligned.
- Avoid center-aligning long paragraphs.

---

## Components

### 1. Header
Purpose: navigation + immediate CTA

Structure:
- left: logo
- center/right: Services, Projects, About, FAQ, Contact
- far right: primary button

Behavior:
- sticky on scroll
- white or slightly translucent background
- compact height

Primary CTA labels:
- Get Free Estimate
- Request Quote
- Book Consultation

---

### 2. Hero
Purpose: immediate positioning + action

Structure:
- short eyebrow text
- strong headline
- one supporting paragraph
- primary CTA + optional secondary CTA
- trust microproof row
- large renovation photo or split image

Recommended content shape:
```yaml
hero:
  eyebrow: "Licensed Bay Area General Contractor"
  headline: "High-Quality Home Remodeling Built Around Clear Process"
  subtext: "Kitchen remodels, bathrooms, ADUs, and full-home renovations with honest communication and dependable execution."
  primary_cta: "Get Free Estimate"
  secondary_cta: "View Projects"
  trust_items:
    - "Licensed & insured"
    - "Bay Area based"
    - "Clear estimates"
```

Rules:
- Keep headline under 12 words if possible.
- Do not overload hero with badges.
- Use one main image, not a busy collage.

---

### 3. Trust Bar
Purpose: instant credibility

Use directly below hero.

Items:
- Licensed & insured
- Transparent estimates
- Quality workmanship
- Bay Area service

Optional metrics:
- Years of experience
- Projects completed
- Avg review score

---

### 4. Service Cards
Purpose: clarify what RCK does

Structure:
- service image or icon
- service title
- one short description
- optional link

Recommended service set:
- Kitchen Remodeling
- Bathroom Remodeling
- ADU / Garage Conversion
- Full Home Renovation
- Room Additions
- Interior Upgrades

Rules:
- Keep descriptions practical, not poetic.
- Use outcomes homeowners care about.
- Each card should make it easy to self-identify.

Example:
```yaml
service_card:
  title: "Kitchen Remodeling"
  body: "Functional, modern kitchens designed for daily use, better storage, and long-term value."
  cta: "Learn more"
```

---

### 5. Project Showcase
Purpose: visual proof

Structure:
- large image
- project title
- city/location
- short summary
- optional tags

Recommended tags:
- Kitchen
- Bathroom
- ADU
- Full Remodel
- Addition

Rules:
- Always show location if possible.
- Use real photography only.
- Prefer before/after when available.
- Avoid mockups or stock interiors.

Example caption:
```yaml
project:
  title: "Modern Kitchen Remodel"
  location: "Sunnyvale, CA"
  summary: "Opened the layout, improved storage, and upgraded finishes for a cleaner and brighter family kitchen."
```

---

### 6. Why Choose RCK Section
Purpose: differentiate without fluff

Recommended bullets:
- Clear communication from estimate to completion
- Clean, organized job sites
- Quality-focused workmanship
- Transparent scope and process
- Local knowledge and permit awareness
- Professional scheduling and follow-through

Design:
- 2-column layout
- left: copy
- right: checklist cards or supporting image

---

### 7. Process Section
Purpose: remove uncertainty

Structure:
```yaml
process:
  - step: "01"
    title: "Consultation"
    body: "We learn your goals, timeline, and budget."
  - step: "02"
    title: "Estimate & Scope"
    body: "We define the work clearly so expectations are aligned."
  - step: "03"
    title: "Planning & Permits"
    body: "We organize the next steps and handle requirements where needed."
  - step: "04"
    title: "Construction"
    body: "We execute with communication, quality control, and professionalism."
  - step: "05"
    title: "Final Walkthrough"
    body: "We review the result together and close out cleanly."
```

Rules:
- Keep it simple.
- Homeowners should understand the process in under 15 seconds.
- Use this section to reduce fear of the unknown.

---

### 8. Testimonials
Purpose: social proof

Structure:
- quote
- customer name
- city
- project type
- optional avatar or star row

Rules:
- Prioritize believable specificity.
- Add city/location when possible.
- Keep cards clean.
- Do not use generic praise with no context.

Example:
```yaml
testimonial:
  quote: "RCK kept the process clear, the crew was respectful, and the final kitchen came out better than we expected."
  name: "Sarah M."
  city: "San Jose, CA"
  project: "Kitchen Remodel"
```

---

### 9. Protection / Warranty Section
Purpose: de-risk the contact decision

Structure:
- strong section heading
- 2 or 3 trust cards
- supporting photo

Suggested trust cards:
- Clear communication
- Quality workmanship
- Support after completion

Important note:
Only claim warranty terms that RCK can actually honor.
Do not copy the source site's 24-month warranty language unless it is true for RCK.

---

### 10. FAQ Section
Purpose: resolve objections before contact

Priority FAQs:
- What types of projects do you take on?
- Do you provide free estimates?
- Do you help with permits?
- How long does a remodel usually take?
- How do you handle changes during the project?
- Are you licensed and insured?
- Which areas do you serve?

Rules:
- Answer directly.
- Avoid legal-sounding language.
- Use FAQs to reduce friction, not to sound impressive.

---

### 11. CTA Banner
Purpose: convert after trust has been built

Structure:
- bold headline
- one sentence support text
- one prominent button

Examples:
- Ready to Start Your Remodel?
- Get a Clear Estimate for Your Project
- Talk to a Bay Area Contractor You Can Trust

Button labels:
- Request Quote
- Get Free Estimate
- Schedule Consultation

---

### 12. Contact / Lead Form
Purpose: capture intent with minimum friction

Recommended fields:
- full name
- phone
- email
- city
- project type
- short message

Best practice:
- keep it short
- place form above the fold on the contact page
- optionally repeat phone CTA for users who prefer calling

Microcopy examples:
- "Tell us a little about your project and we’ll get back to you shortly."
- "Prefer to talk now? Give us a call."

---

## Page Blueprint

### Homepage Order
```yaml
homepage:
  - Header
  - Hero
  - Trust Bar
  - Services
  - Featured Projects
  - Why Choose RCK
  - Process
  - Testimonials
  - FAQ
  - Final CTA
  - Footer
```

### Service Page Order
```yaml
service_page:
  - Header
  - Service Hero
  - Benefits
  - Project Examples
  - Process
  - FAQ
  - CTA
  - Footer
```

### Contact Page Order
```yaml
contact_page:
  - Header
  - Contact Hero
  - Lead Form
  - Service Area / Cities
  - FAQ
  - Footer
```

---

## Copy System

### Voice
- direct
- clear
- homeowner-friendly
- confident without hype

### Copy Rules
- Write like a professional contractor, not an ad agency.
- Use short sentences.
- Emphasize clarity, workmanship, and process.
- Prefer concrete words over abstract claims.

### Preferred phrases
- clear estimate
- quality workmanship
- reliable communication
- Bay Area homeowners
- built for daily living
- clean and organized process

### Avoid phrases
- world-class
- cutting-edge
- revolutionary
- luxury craftsmanship unless truly luxury-focused
- transforming dreams into reality
- your vision, our passion

---

## Imagery Rules
- Use real project photography.
- Prioritize bright, clean, finished spaces.
- Show kitchens, bathrooms, and remodeling details.
- Show the result, not just tools or workers.
- Use Bay Area-relevant project context where possible.

Avoid:
- obvious stock photos
- generic handshake images
- overly staged smiling-team photos
- low-resolution before images as hero assets

---

## Interaction Rules
- Keep animation subtle.
- Use fade, slight slide, and simple hover states.
- No parallax-heavy interactions.
- No spinning icons or flashy motion.
- Buttons should feel responsive, not playful.

Suggested motion:
```yaml
motion:
  hover_scale: "1.01"
  transition_fast: "150ms ease"
  transition_normal: "220ms ease"
  reveal_offset: "12px"
```

---

## Mobile Rules
- Keep CTA visible early.
- Stack hero content with image second.
- Use large tap targets.
- Reduce headline size, not hierarchy.
- Make service cards easy to scan vertically.
- Keep form fields full-width.

---

## SEO / Conversion Guidance
- Include service + location combinations naturally.
- Use headings that mention remodel types and Bay Area service.
- Put trust and local relevance above generic portfolio language.
- Repeat estimate intent in hero, middle CTA, and footer CTA.

Suggested title pattern:
- `Kitchen & Bathroom Remodeling in the Bay Area | RCK Development`

Suggested meta tone:
- clear, local, trustworthy, action-oriented

---

## Anti-Patterns
Do not do the following:
- too many colors
- dark-mode-only contractor site
- oversized animation
- long paragraphs in hero
- generic stock testimonial avatars
- weak CTA labels like "Submit"
- cluttered gallery grids with no context
- overclaiming timeline or warranty promises

---

## Prompt Block for AI Builders
Use this prompt in v0 / Bolt / Framer AI when generating pages:

```md
Build a lead-generation website for RCK Development, a Bay Area general contractor focused on kitchen remodeling, bathroom remodeling, ADUs, room additions, and full-home renovation.

Style:
- clean, premium, trustworthy
- modern contractor website
- lots of white space
- Inter font
- blue accent (#2F6FED)
- black headings, muted gray body text
- real-estate/editorial style layout
- subtle shadows, rounded corners, calm motion

Goal:
- generate estimate requests and phone calls
- make homeowners feel trust, professionalism, and clarity

Homepage sections:
- sticky header with CTA
- hero with strong headline, support text, estimate CTA, and trust microproof
- trust bar
- service cards
- featured projects with locations
- why choose us
- 5-step process
- testimonials with city and project type
- FAQ
- final CTA banner
- footer

Requirements:
- no flashy design
- no startup vibe
- no generic handyman feel
- use real renovation imagery placeholders
- optimize for conversion and local trust
```

---

## Summary
This system should help RCK look like:
- a real operator
- a reliable contractor
- a premium but approachable local business

The visual job is simple:
**earn trust fast, show proof, repeat the CTA, and make it easy to request an estimate.**
