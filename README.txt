Textile Innovation Awards 2026 website

Upload the contents of this folder to the web root of innovation-awards.textiletoday.com.bd
(replacing the old 2024 WordPress site):

  index.html     main page (logo animation, categories, nomination form, jury, awards night, partners, contact)
  gallery.html   2024 photo gallery with slideshow and full-screen viewer
  gallery/       51 photos (large + thumbnail versions)

Nomination form: to receive submissions directly, open index.html, search for
  const FORM_ENDPOINT = '';
and put your form service URL between the quotes (e.g. a Formspree or Google Apps Script URL that accepts JSON POST).
Until then, nominees are given a ready-to-send email to info@textileinnovationexchange.com.

Old 2024 links keep working through small redirect pages included here:
  /photo-gallery/ -> gallery.html, /eligibility/ -> #apply,
  /categories-criteria/ -> #categories, /jury-board/ -> #jury

GITHUB PAGES
  1. Create a repository and upload EVERYTHING in this folder to its root
     (including the hidden files .nojekyll and CNAME).
  2. Settings > Pages > Source: "Deploy from a branch", branch main, folder / (root).
  3. CNAME already contains innovation-awards.textiletoday.com.bd.
     At your DNS provider, point that subdomain with a CNAME record to <your-github-username>.github.io
     (replace the record that currently points to the WordPress server).
     If you want to test on the github.io address first, delete CNAME until you switch over.
  4. After DNS updates, tick "Enforce HTTPS" in Settings > Pages.
