# AMKO Engineering Website

A single-page marketing site for **AMKO Engineering Services**, an electro-mechanical engineering company based in Alexandria, Egypt. The page presents the company's services, background, mission and contact details. Everything lives in one self-contained `index.html` file.

## Page sections

The navigation bar links to Home, Services, Projects, About, Mission, Chairman, Clients and Contact. The page itself contains these sections, in this order:

| Section | Anchor | Content |
|---|---|---|
| Hero | `#home` | Company name, tagline, short introduction and headline figures |
| About | `#about` | Company overview, industries served and summary statistics |
| Mission & Values | `#mission` | Mission, strategy and values cards |
| Chairman's Message | `#chairman` | Message from the company chairman |
| Clients | `#clients` | Grid of client names |
| Contact | `#contact` | Address, phone, email and website, plus a "Get In Touch" form |
| Services | `#services` | Nine service cards (for example electro-mechanical maintenance, condition monitoring, piping installation, project management) |
| Footer | — | Summary, service links, social handles, contact info and copyright |

## Tech stack

- **HTML5 and CSS3**, with all styles in an inline `<style>` block (flexbox/grid layout and one responsive breakpoint at 768px)
- **Vanilla JavaScript** in an inline `<script>` block: smooth scrolling to anchors, a navbar style change on scroll, and a hover animation on service cards
- **Google Fonts** for the Inter typeface
- **Unsplash** for two hotlinked images (hero and About sections)
- Icons are Unicode emoji. No icon library, framework or build step is used.

## Viewing locally

Open `index.html` directly in a browser, or serve the folder:

```bash
git clone https://github.com/Rewanooo22/amko-engineering-website.git
cd amko-engineering-website
python -m http.server 8000
# then open http://localhost:8000
```

Fonts and images load from external CDNs, so an internet connection is needed for the page to render fully.

## Known limitations

- **The contact form does not send anything.** The `<form>` has no `action` attribute and no submit handler, so it only runs the browser's built-in field validation.
- **Broken anchors:** the "Projects" nav link and the "View Projects" button point to `#projects`, and the footer's "Download Brochure" button points to `#brochure`. Neither section exists on the page, and no brochure file is included.
- **Section order differs from the nav order:** Services is listed second in the navigation but is the last section on the page.
- **Social links are placeholders:** the Facebook, LinkedIn and Instagram entries point to `#`.
- **No mobile menu:** below 768px the navigation links are hidden and nothing replaces them.
- **Malformed footer markup:** a stray fragment (`="#services">Project Management</a></p></div>`) after the "Follow Us" column renders as visible text.
- The statistics on the page (years of experience, project count, team size, client satisfaction) are static marketing copy.
