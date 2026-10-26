# Electrify Christchurch website

A simple static website (plain HTML, CSS and images). No build step or coding tools are needed, and it can be hosted free on GitHub Pages.

## What is in this folder

| Path | What it is |
|---|---|
| `index.html` | Home page |
| `about.html` | About us |
| `why-electrify.html` | Why go electric? (Rewiring Aotearoa report figures) |
| `events.html` | Events |
| `get-involved.html` | Get involved |
| `contact.html` | Contact page and form |
| `404.html` | Page shown if a link is broken |
| `assets/css/styles.css` | All of the site's styling (colours, Rubik font, layout) |
| `assets/images/` | All illustrations, the logo and the favicon |
| `files/` | Put PDFs here (see below) |
| `.nojekyll` | Tells GitHub to publish the files exactly as they are |

## Putting it on GitHub Pages

1. Sign in to GitHub and create a new repository (for example `electrify-christchurch`). Make it **Public**.
2. Click **Add file > Upload files** and drag in everything from inside this folder, keeping the folder structure. Include the `.nojekyll` file if your computer shows hidden files. Click **Commit changes**.
3. Open the repository's **Settings > Pages**. Under "Build and deployment", choose **Deploy from a branch**, pick the `main` branch and the `/ (root)` folder, then Save.
4. After a minute or two the site appears at `https://YOUR-USERNAME.github.io/REPOSITORY-NAME/`.

### Using your own domain (for example electrifychristchurch.nz)

1. In **Settings > Pages**, type your domain into **Custom domain** and save. GitHub adds a file called `CNAME` for you.
2. At your domain registrar, add the DNS records GitHub lists on its "Managing a custom domain" help page.
3. Tick **Enforce HTTPS** once it becomes available.

## Before you go live

- **Contact form:** the form in `contact.html` needs a form service to send messages to your inbox. Create a free form at Formspree (formspree.io) or a similar service, then replace `YOUR_FORM_ID` in the `<form action="...">` line with your form's ID. Send yourself a test message. Until you do this, the form will not work.
- **Social sharing image:** to show a picture when the site is shared on Facebook, add a line like `<meta property="og:image" content="https://YOUR-DOMAIN/assets/images/electric-home.png">` near the other `og:` lines in each page, using your real web address.
- **Case study PDFs:** the three local stories on `why-electrify.html` currently link to PDFs hosted on the Rewiring Aotearoa website. You can leave them or download the PDFs, put them in `files/` and change each link to `files/your-file-name.pdf`.
- **Check every page** on your phone after publishing.

## Everyday changes

- **Change text:** open the page file on GitHub, click the pencil icon, edit the words between the tags, and commit the change. The site updates in a minute or two.
- **Add or replace a PDF:** upload it to `files/` (use lowercase names with hyphens), then link to it with `<a href="files/file-name.pdf" target="_blank" rel="noopener">Read the report (PDF)</a>`. To replace one, upload a new file with exactly the same name.
- **Change an image:** upload a new PNG to `assets/images/` with the same file name.
- **Colours and fonts:** these are at the top of `assets/css/styles.css`. The yellow is `#FFC754` and the cream background is `#FDFAF1`.

## Credits

Figures on the "Why go electric?" page are from Rewiring Aotearoa's Christchurch city regional report (v1.0, October 2026). Keep the credit and link to the report in place, and update the figures if a newer version is released.
