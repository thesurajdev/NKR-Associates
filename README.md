# NKR & Associates

Marketing website for NKR & Associates, an accounting and compliance firm in New Delhi. Built to rank for local searches and turn visitors into WhatsApp enquiries.

**Live site:** [nkrandassociates.com](https://nkrandassociates.com)

Built by [Suraj Dev](https://www.surajdev.com) for NKR & Associates, shown here with the client's permission.

<!-- Add 2-3 screenshots here: hero section, services modal, mobile view -->

## What the site covers

The firm offers bookkeeping, GST registration and compliance, ITR filing, accounting and finalisation, payroll and TDS, business registration and ROC work, NGO registration, intellectual property, government licences, audit and assurance, advisory, and legal agreements. The site groups these into service categories, each opening a modal with the details.

## What's on the page

- Mobile-first layout that works from phones to desktops
- Custom cursor on desktop, plus scroll animations and a text marquee
- Floating WhatsApp button for instant enquiries
- Service categories with modals
- FAQ accordion
- Scrolling client logos and a testimonials section
- Contact section, and a preloader for first paint

## SEO work

This is the part I'd point a client to.

**Structured data (JSON-LD):** `ProfessionalService`, `WebSite`, `FAQPage`, `BreadcrumbList` and a catalogue of the six main services, so Google can read what the firm does and show FAQ rich results.

**Technical setup:** title and meta description, Open Graph and Twitter cards, canonical URLs, geo tags for Delhi, `sitemap.xml`, `robots.txt` and a Google Search Console verification file.

**Speed:** WebP images with lazy loading and explicit dimensions, preconnect and DNS prefetch for external resources, and GZIP compression and browser caching through `.htaccess`.

<!-- Add measured results here once you've run them: Lighthouse scores for mobile and desktop, Core Web Vitals from Search Console, ranking or traffic change since launch. Use real numbers or leave this out. -->

## Stack

Plain HTML5, Tailwind CSS (via CDN) and vanilla JavaScript. No build step, no framework, no database.

```
NKR-Associates/
├── index.html           main site
├── coming-soon.html     coming-soon page
├── sitemap.xml
├── robots.txt
├── .htaccess            compression, caching, security headers
├── google*.html         Search Console verification
└── media/
    ├── logo.webp
    ├── client-logo/     client logos
    └── ...              hero images, team photos
```

## Run it locally

```bash
git clone https://github.com/thesurajdev/NKR-Associates.git
cd NKR-Associates
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploying

Upload the files to any Apache host. The `.htaccess` file needs Apache, so on other servers, set up compression and caching in the server config instead. After going live: turn on HTTPS, confirm the canonical URLs use the live domain, submit `sitemap.xml` in Google Search Console, and check the structured data with Google's [Rich Results Test](https://search.google.com/test/rich-results).

## License

© 2026 NKR & Associates. All rights reserved. The code and content are published here as a portfolio piece and are not licensed for reuse.
