# AMKO Engineering Services Website

A single-page marketing website for **AMKO Engineering Services**, built with plain HTML, CSS and a little JavaScript. There is no build step.

## Sections

- **Home**: hero banner
- **About AMKO**
- **Mission & Values**: mission, strategy and values
- **Chairman's Message**
- **Our Services**: electro-mechanical maintenance, technical assistance and manpower, condition monitoring, spare parts supply and fabrication, upgrades and turnkey projects, alignment, piping installation, project management, and belt vulcanizing and maintenance
- **Our Trusted Clients**
- **Contact Us**: contact form (name, email, subject, message)

## View it

Open `index.html` in a browser, or serve the folder:

```bash
git clone https://github.com/Rewanooo22/amko-engineering-website.git
cd amko-engineering-website
python -m http.server 8080
```

Then go to http://127.0.0.1:8080.

To publish it, enable **GitHub Pages** (Settings → Pages → deploy from the `main` branch, root folder).

## Tech

- HTML5 and CSS3, with all styles inline in `index.html`
- [Inter](https://fonts.google.com/specimen/Inter) from Google Fonts
- A small vanilla JavaScript block at the end of the page

## Known limitations

The contact form has no backend, so messages aren't sent anywhere. Connect it to a form service (for example Formspree) or a server endpoint before relying on it.
