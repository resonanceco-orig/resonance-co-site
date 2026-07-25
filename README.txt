RESONANCE CO. — static site (Netlify). Drag this whole folder onto Netlify to publish.

Pages: index.html (Home) · about.html (About) · for-event-communities.html (Speaking).
Home is fully static HTML (pre-rendered July 2026): all text is crawlable, animations are CSS
plus a small inline script. Fonts self-hosted in assets/fonts/.
SEO layer: sitemap.xml, robots.txt, 404.html, assets/favicon.svg, canonical tags, and JSON-LD
structured data (Organization + Person on Home, Person + Book on About, Service on Speaking).
Canonical domain: https://resonanceco.co (set as primary domain in Netlify).
about.html and for-event-communities.html share assets/site.css (tokens, nav, footer); their page-specific CSS stays inline.
Stay in Touch form is wired for Netlify Forms (form name "stay-in-touch").
Footer Instagram/TikTok links point to the live @resonancecoevents profiles.

Changelog (July 2026 cleanup):
- Home restored from Rayven's current working copy (self-contained bundle). It was missing
  from the GitHub repo; commit this file so repo and deploy match.
- Team load-in video removed intentionally (was a coming-soon item). Stay in Touch is form-only.
- Home carries its own inline styles (it does not use assets/site.css); fonts are self-hosted TTFs.
- Textbook cover renamed for SEO to Crisafulli-Event-Planning-Management-textbook-cover.jpg,
  compressed from 3.3MB. The old 2-byte PNG and the oversized PNG were removed.
- Press stills recompressed as JPGs.
- "Read the full story" link restored on Home (About page now exists).
- Credential rule: "PhD, CMP" in bylines and captions sitewide.
- Rose accent (#B01050) limited to one static use per page, per brand rule.

Outstanding (decisions for Rayven):
- "View the textbook" button on About stays hidden until the 2nd Edition publishes (Fall 2026).
- Hidden "On TikTok" block on About awaits the three pinned videos.
- When /speak ships: add noindex to it, and add nothing to sitemap.xml (it stays unlisted).
