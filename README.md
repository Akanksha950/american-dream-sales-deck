# American Dream — Interactive Sales Deck

A fully interactive, browser-based Digideck-format commercial sales presentation for American Dream, East Rutherford, NJ — the largest mall in the Western Hemisphere.

**Live URL:** [Deploy to GitHub Pages / Vercel / Netlify — see below]

---

## What This Is

A self-contained, single-file interactive sales deck built for American Dream's commercial team. It replaces fragmented pitching (YouTube videos + PDFs + spreadsheets) with one cinematic, non-linear experience that works equally well on a live sales call or as a standalone prospect link.

The format is modelled after Digideck: full-screen slides, chapter tab navigation, a thumbnail filmstrip, a non-linear hub, and immersive slide-level storytelling — all in a single `index.html` file with zero build dependencies.

---

## Tech Stack

| Layer | Choice | Why |
|---|---|---|
| Structure | Vanilla HTML5 | Zero deps, instant deploy |
| Styling | Pure CSS3 | CSS variables, keyframe animations, grid |
| Logic | Vanilla JS (ES6+) | No framework overhead |
| Fonts | Google Fonts (Cormorant Garamond + Barlow Condensed) | Luxury/editorial pairing |
| Images | Unsplash CDN | High-quality, fast, free |
| Map | Inline SVG | Interactive, scalable, no libraries |

---

## Deck Structure

```
Chapter 0: Introduction
  ├── Slide 1: Cinematic hero — "Not a Mall. A Platform."
  └── Slide 2: Hub — Choose your path (non-linear)

Chapter 1: The Property
  ├── Slide 3: Why American Dream is different (stats)
  └── Slide 4: Regional reach & access (catchment map)

Chapter 2: Retail Leasing
  ├── Slide 5: The leasing opportunity
  └── Slide 6: ★ INTERACTIVE FLOOR MAP — "I Need to Be Here" moment

Chapter 3: Events & Venues
  ├── Slide 7: The global stage
  └── Slide 8: Venue tabs (Arena / PAC / Activation / Corporate)

Chapter 4: Entertainment
  └── Slide 9: Six world-class attractions grid

Chapter 5: Brand Sponsorship
  ├── Slide 10: Audience data + animated bars
  └── Slide 11: Partnership tiers (Presenting / Premier / Title)

Chapter 6: Contact
  ├── Slide 12: Design rationale & "I Need to Be Here" write-up
  └── Slide 13: Contact & inquiry CTA
```

---

## The "I Need to Be Here" Moment — Explained

**The feature:** The Live Retail Floor Map (Chapter 2, Slide 2).

**The interaction:** The viewer sees a full-screen SVG floor plan of American Dream. Every zone — Luxury Wing, Core Retail, Pop-Up rows, Munchies Food Hall, Big SNOW, The Arena, the Dream Wheel — is individually clickable. Clicking any zone slides open a detail panel with the specific leasing pitch for that location: available spaces, foot-traffic intensity, dwell-time data, anchor neighbors, and a direct "Inquire About This Space" CTA.

**Why it earns the reaction:**

A luxury brand executive clicking the Luxury Wing sees: Hermès and Gucci as neighbors, $87K+ average household income, 0% NJ clothing tax, and two spaces available — all in one interaction. They don't need to be told the opportunity. They *see* their name on the map.

A pop-up streetwear label clicking Zone A sees: peak traffic position, 1-week minimum term, and a direct inquiry button. The decision window from curiosity to contact is under 60 seconds — with no salesperson present.

This is what a deck should do. It doesn't describe the opportunity — it puts the prospect inside it.
---

## Design Decisions

**Why a single file?**
A sales rep needs to be able to email a link. A prospect needs to explore it on their laptop at 11pm. One file means zero broken asset paths, zero CDN failures, instant deployment. The entire deck travels in one URL.

**Why no video?**
Autoplay video from external sources introduces latency and reliability risk on live calls. The Ken Burns CSS animation on background images creates motion and atmosphere without any network dependency. With more time, self-hosted MP4s would replace the still images.

**Why SVG for the floor map?**
D3.js or Mapbox would be overkill for a fixed floor plan. An inline SVG gives full interactivity, perfect scalability, and zero additional payload. The entire map is ~60 lines of markup.

**Typography pairing:**
Cormorant Garamond (serif, 300 weight) for headlines — the same weight class used by luxury fashion brands. Barlow Condensed for all UI chrome — compressed, legible, high information density. Never Inter. Never Roboto.

---

## What I Would Build With More Time

1. **Autoplay video backgrounds** — Full-bleed MP4 on the hero and entertainment slides
2. **Live footfall charts** — Animated bar charts showing peak vs off-peak traffic by day/hour
3. **Deep-link chapter sharing** — `?chapter=leasing` URL parameter so a sales rep can send a prospect directly to the relevant chapter
4. **PDF export** — One-click export of the current chapter as a leave-behind PDF
5. **Analytics layer** — Track which slides a prospect spends the most time on; feed into CRM

---

## Contact

American Dream Commercial Team  
One American Dream Way · East Rutherford, NJ 07073  
americandream.com
