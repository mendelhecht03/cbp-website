# Chabad of Boro Park — Stripe Verification Site

## Purpose

Minimal single-page website to satisfy Stripe's business website requirements so the organization's Stripe account can be verified for donation processing. This is not a full marketing site. The goal is approval, not features.

## Organization Details

- **Operating name:** Chabad of Boro Park
- **Legal name:** Anshei Moshe Chabad Inc.
- **Type:** 501(c)(3) nonprofit
- **Phone:** [+1 (929) 406-8957]
- **Email:** [chabadboropark@gmail.com]
- **Address:** [1231 45th Street, 2nd Floor, Brooklyn, NY 11219]
- **Tagline:** "Spreading the wellsprings of Chassidus throughout Boro Park"  
- **Description:** "Your donation supports Chabad of Boro Park's mission of spreading Chassidus and serving the Chassidishe community of Boro Park through Torah learning, outreach, and community programs.”

## Tech Stack

- Plain HTML + Tailwind CSS via CDN
- No build step, no npm, no frameworks, no JS libraries
- Vanilla JS only if absolutely needed
- Deployment: Cloudflare Pages

## Stripe Requirements the Site Must Meet

1. Organization legal name visible (matching Stripe account)
2. Clear description of what the organization does
3. Clear statement of what donations support
4. Contact info: phone, email, address (all visible)
5. Donation refund policy (separate page, linked from footer)
6. Privacy policy (separate page, linked from footer)
7. Terms of service (separate page, linked from footer)
8. HTTPS (automatic via Cloudflare Pages)
9. No placeholder content, no "coming soon" sections
10. All links functional

## Site Structure

**`index.html`** — single page with:
- Organization name and brief tagline
- Short description of the organization and what donations support
- Contact info (phone, email, address)
- Footer with: legal name, 501(c)(3) statement, links to privacy/terms/refund pages

**Three separate legal pages:**
- `privacy.html`
- `terms.html`
- `refund-policy.html`

That's the entire site. No hero animations, no "what we do" grids, no fancy donate section, no suggested amount buttons. Just the required content, cleanly presented.

## Design

- Clean, simple, readable
- Mobile-responsive
- Doesn't have to look impressive — just has to look legitimate
- Skip animations, gradients, hover effects unless trivial

## What NOT to Build

- No multi-section homepage
- No "what we do" section
- No suggested donation amounts
- No donate button functionality yet (placeholder link is fine)
- No images unless trivially easy
- No JavaScript interactions
- No contact form
- No anything not on the Stripe requirements list above

## Working Style

- Build the whole homepage in one pass since it's so minimal
- Then generate the three legal pages using free templates adapted to a nonprofit
- Don't add features not in this spec