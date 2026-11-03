# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

Mainly tourists from Spain on short city trips to Berlin. They are Spanish speakers who want a guided tour in their own language, and they choose and book shortly before or during the trip, usually on a phone.

## Product Purpose

berlines.es is the landing page for Carlos Maza, a Spanish-speaking local guide in Berlin. Visitors see the tour catalog (free tours, themed tours, premium day trips and experiences), check duration, schedule and price, and start a booking. Success means a visitor sends a WhatsApp message to book a specific tour.

## Positioning

A mix of three things the big Spanish free-tour operators can't honestly claim together:
- **One local guide, personal:** Carlos runs the tours and answers WhatsApp himself (reply within 24h).
- **Depth on history:** the Wall and Cold War, Nazism, Sachsenhausen and Potsdam told with rigor, at the places where things happened.
- **Niche experiences:** the Berlin beer tour, Berlín Alternativo (street art, squats, clubs), kayaking on the canals, and Sunday walks (Treptower Park, Tiergarten).

## Operating Context

- Booking runs through WhatsApp deep links (`wa.me/4915567304172`) with a message pre-filled per tour. The site has no booking engine and takes no payments.
- Social channels: Instagram and TikTok, both `@berlines.es`.
- Pricing types: free tours on a tip basis ("Propina"), paid tours with a discount-code price (for example 20€ · 18€ con código), and some tours priced on request ("A consultar").
- Per the Impressum, Carlos is a Reiseführer who runs guided tours for other providers. Do not present him as selling package tours.

## Capabilities and Constraints

- Static HTML/CSS with no framework and no build step, hosted on GitHub Pages (repo `mazapandi/berlinjoven-website`). Keep it that way.
- Pages: `index.html` (landing and catalog) and `impressum.html` (legal page; German legal text with Spanish glosses, currently marked provisional while the Gewerberegister entry is being changed).
- All site copy is in Spanish, except the Impressum, which stays in German as legally required.
- **Undecided:** what happens to `blog/` (older "Berlin Joven" branding, not linked from the landing page).

## Brand Commitments

- Name: **berlines.es**. It replaces the earlier "Berlin Joven" brand.
- Voice: first person, warm and direct, from a local guide ("Escríbeme por WhatsApp", "¿Nos vemos en Berlín?").

## Evidence on Hand

- Tour photos: `img/welcome.jpg`, `img/muro.webp`, `img/alternativo.jpg`, `img/cerveza.jpg`, `img/foto1–6.jpg`, `img/tours-abril-2025/*.webp`.
- Real tour facts (names, durations, schedules, prices) are in `index.html`.
- Real reviews exist on external platforms, but they are not yet collected in the repo and the source platform hasn't been confirmed. Do not invent review text, ratings or counts. Ask for the real ones.
- There are no press mentions, partner logos or visitor numbers on hand. Do not make them up.

## Product Principles

1. Every surface leads to a WhatsApp message about a specific tour.
2. The site should feel like one real person, not an agency: first person, a local view, direct contact.
3. Be precise and honest about logistics (duration, times, price, tip-based or not). That is what a trip planner needs.
4. Take history seriously. Tours about Nazism, Sachsenhausen and the Wall get a respectful, factual treatment, never playful.
