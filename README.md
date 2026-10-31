# Jude Uche — Personal Portfolio

A responsive personal portfolio built with semantic HTML5 and modern CSS3 only.

## Project structure

```text
portfolio/
├── index.html
├── css/
│   └── style.css
├── assets/
│   ├── images/
│   └── icons/
└── README.md
```

The `assets/images/` and `assets/icons/` folders are intentionally included as locations for your own static assets. The current design uses a CSS-built portrait placeholder and decorative CSS artwork, so no image download is required to view the site.

## Open locally

1. Download and extract the `portfolio` folder.
2. Open `index.html` directly in a modern browser.
3. No server, package manager, build process, JavaScript, or external dependency is required.

## Personalise the website

### Replace the portrait placeholder
Add a professional portrait to `assets/images/` (for example, `jude-uche-portrait.webp`). In `index.html`, replace the `<div class="portrait-placeholder" ...>` block in the hero with:

```html
<img
  class="portrait-photo"
  src="assets/images/jude-uche-portrait.webp"
  alt="Portrait of Jude Uche"
  width="900"
  height="1100"
>
```

Then add this rule to `css/style.css`:

```css
.portrait-photo {
  display: block;
  width: 100%;
  height: 440px;
  object-fit: cover;
  object-position: center 35%;
}
```

Adjust the height in the mobile media query if needed. Use a compressed WebP or AVIF image to keep the page light.

### Update your professional profile
Review the text in `index.html`, especially:
- Professional title and hero introduction.
- About section and learning interests.
- Skills and capability descriptions.
- Focus areas and service availability.
- Education, experience and milestones.
- Project cards and testimonial placeholder.

Only publish skills, qualifications, projects, client names, testimonials and achievements that are accurate and that you have permission to share. The headline supplied for this first version has been reframed as an exploration of software development rather than a verified employment or company claim.

### Add projects
For each completed project, include:
- Project name and category.
- The real problem it addresses.
- Your contribution and process.
- Tools/technologies actually used.
- Screenshots with descriptive alt text.
- Working live-demo and source-code links, where available.

Do not leave `#` links for unfinished project buttons. Add links only when they work.

### Update social links
The current profile includes GitHub: `https://github.com/judextech`. Add other verified professional profiles in the contact area when ready.

## Contact form limitation

This version uses direct `mailto:` and `tel:` links. A static HTML/CSS page cannot receive, store, or send form submissions by itself. A working contact form requires a backend or a trusted form-processing service. No non-working form has been included.

## CSS-only mobile navigation

The mobile menu uses the native HTML `<details>` and `<summary>` disclosure elements. This works without JavaScript and supports keyboard interaction in modern browsers.

## SEO and sharing notes

- The page includes a descriptive title, meta description, viewport, author and Open Graph metadata.
- Replace the Open Graph image placeholder (`assets/images/og-placeholder.jpg`) with a real, publicly hosted social-sharing image before publishing.
- Add a canonical URL and custom domain metadata when your final website URL is known.
- Search preview and social-sharing behaviour can vary by platform.

## Deployment

You can host this static folder on GitHub Pages, Netlify, Cloudflare Pages or any static web host. Upload the contents of the `portfolio` folder while preserving the folder structure. For GitHub Pages, create a repository, add these files, and enable Pages from the repository settings.

## Accessibility and performance

The site includes semantic landmarks, a skip link, a logical heading structure, visible keyboard focus, descriptive link text, responsive layouts and reduced-motion support. The portrait placeholder has an accessible description. Images added later should have useful alt text and explicit dimensions.

No Lighthouse, screen-reader, cross-browser, or Core Web Vitals audit has been run as part of this deliverable. Test the deployed version with keyboard navigation, a screen reader, browser responsive tools and Lighthouse before treating it as production-verified.

## Known limitations

- HTML and CSS cannot implement client-side form submission, dynamic filtering, live project data, analytics, authentication or database features.
- There is no JavaScript, framework, external font, tracking script or animation library.
- The site is a strong first portfolio foundation; it should be updated as your real work and experience grow.
