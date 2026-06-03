# CLAUDE.md — Hotel Hospitality Helper · Four Seasons deck (handoff)

Read this to resume without prior chat.

## What this is
A 14-section single-file animated HTML pitch deck for **Misión Digital · Hotel Hospitality Helper (XPRNZ for hotels)**, built in the **Four Seasons web aesthetic** (researched from fourseasons.com + Aman/Belmond/Ritz). This is a SEPARATE, simplified variant from the ornate original deck (`hotel-hospitality-helper-presentation`, live at hhh-mision-digital.netlify.app). Single file: `index.html` (inline CSS + JS).

## Live + repo
- **Live:** https://hhh-fourseasons.netlify.app
- **GitHub:** riverplateconsulting/hhh-fourseasons (private). NOTE: GitHub is under the `riverplateconsulting` account for now; Netlify currently under brian@riverplateconsulting.com. Brian's standing rule is that Misión Digital work should live on the **brian@mision-digital.com** accounts (GitHub `BrianMision`, Netlify slug `brianmision`); migration of this deck is a pending follow-up.

## Design system
Black-on-white editorial, color from full-bleed Unsplash photography (URLs are curl-verified), hairline rules, **gold `#B58E3F` as a RARE accent**. Fonts: **Cormorant Garamond** (display, weight 300), **EB Garamond** (body + italic eyebrow), **Archivo** (uppercase tracked labels). Rioplatense Spanish, **no em dashes**, restraint = luxury.

## Conventions / gotchas
- Single-file deck, no build step. Deploy: `cd` here, `source ~/.nvm/nvm.sh && nvm use 20`, `netlify deploy --prod --dir=.`.
- `?reveal` URL flag forces all reveal states AND collapses the `100vh` heroes so a tall headless capture shows the whole deck (hash anchors do not land reliably in headless on this body-scroll page). Capture then crop into bands to review.
- Passed a 14-agent bulletproofing audit. Notable past fix: slide 9 attestation quotes were black-on-black until `.sec.ink .q` joined the white-text override. Smooth scroll is class-gated (`html.smooth`) and off during `?reveal`.

## Status
Shipped, audited, live. Sections: cover, diagnóstico, el código, definición, dos mundos, el pase, ocho pestañas, demo, confirmaciones, arquitectura, evidencia (KPIs), arquetipos, servicio (precio/tiers), cierre. Interactions: QR role toggle, reveal-on-scroll, KPI count-ups.
