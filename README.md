# Quillegacy Website

A simple multi-page website for **Quillegacy**, the senior memory booklet initiative.

## Files

| File / Folder      | What it does                                          |
| ------------------ | ----------------------------------------------------- |
| `index.html`       | Landing page (hero + tiles to the inner pages).       |
| `about.html`       | About Us page.                                        |
| `services.html`    | Our Service page (with the four values).              |
| `product.html`     | Our Product page (booklet image + interview questions). |
| `impact.html`      | Impact page.                                          |
| `team.html`        | Who We Are page.                                      |
| `contact.html`     | Contact Us page (email).                              |
| `style.css`        | Shared colors, fonts, and layout for every page.      |
| `images/`          | Logo and any other images.                            |
| `README.md`        | This file. Instructions for editing.                  |

Every page shares the same nav bar and footer, so the site feels like one cohesive thing.

## How to view the site

Double-click `index.html` and it will open in your web browser.
Use the nav bar at the top to move between pages.

No installation, no build step, no server.

## How to edit text on a page

1. Open the page file you want to edit (e.g. `services.html`) in any text editor.
2. Look for the section you want to change — each one is clearly marked with a comment like `<!-- ===== … ===== -->`.
3. Change the words between the `<p>` (paragraph) or `<h2>` (heading) tags.
4. Save the file and refresh your browser.

## How to change the colors

Open `style.css` and look at the top:

```css
:root {
  --cream:      #faf6f0;   /* page background */
  --warm:       #f3ebdc;   /* alternating section background */
  --ink:        #2b2622;   /* main text color */
  --muted:      #6b6358;   /* secondary text */
  --accent:     #8a5a3b;   /* buttons & highlights */
  --accent-dk:  #6e4429;   /* hover color */
}
```

Change any color code (the `#xxxxxx` value) and the whole site updates.
Tip: use [coolors.co](https://coolors.co/) to pick new colors.

Change any color code (the `#xxxxxx` value) and the whole site updates.
Tip: use [coolors.co](https://coolors.co/) to pick new colors.

## About the font

The site uses **Outfit**, a free Google Font that closely matches Canva's "Now" font.
"Now" itself is a paid commercial font and is not available for free web embedding,
so Outfit is the closest free, web-safe alternative.

**If you want to use the real "Now" font on the website:**

1. Buy/download the `.ttf` or `.woff2` files (e.g. from Adobe Fonts or the foundry).
2. Put the font files in a new folder called `fonts/`.
3. In `style.css`, replace the Outfit setup with:

   ```css
   @font-face {
     font-family: 'Now';
     src: url('fonts/Now-Regular.woff2') format('woff2');
     font-weight: 400;
     font-style: normal;
   }
   /* repeat @font-face for each weight you have */

   :root {
     --font: 'Now', sans-serif;
   }
   ```

4. Remove the `<link href="…Outfit…">` line from the `<head>` of each HTML page.

## How to change the logo

The logo lives at `images/quillegacy-logo.png`.
It has a **transparent background** so it sits cleanly on any page color.

To swap it for a new version, just replace that file (keep the same filename).

## How to add a new page

1. Copy any existing inner page (e.g. `about.html`) and rename it (e.g. `gallery.html`).
2. Change the title, heading, and content for the new page.
3. In the new page's `<nav>` block, move `aria-current="page"` to the new page's link.
4. In **every other** HTML file, add a new link to the `<nav>` block:
   `<a href="gallery.html">Gallery</a>`
5. Save and refresh.

## How to put it online (free options)

1. **GitHub Pages** — push these files to a GitHub repo, enable Pages in Settings.
2. **Netlify Drop** — drag the folder onto [app.netlify.com/drop](https://app.netlify.com/drop).
3. **Vercel** — connect a GitHub repo at [vercel.com](https://vercel.com).

All three are free and take less than 5 minutes.

## Pages on the site

1. **Home** (`index.html`) — opening tagline + tiles linking to each inner page.
2. **About Us** (`about.html`) — mission and project description.
3. **Our Service** (`services.html`) — how the interview becomes a booklet, plus our four values.
4. **Our Product** (`product.html`) — what the finished booklet looks like and the full list of interview questions.
5. **Impact** (`impact.html`) — what this work means for families, seniors, and future generations.
6. **Who We Are** (`team.html`) — the team of three 8th graders.
7. **Contact Us** (`contact.html`) — email address for getting in touch.

## How to change the contact email

Open `contact.html`. Look for these two lines:

```html
<a href="mailto:info@quillegacy.com" class="contact-email">
  info@quillegacy.com
</a>
```

Replace **both** occurrences of `info@quillegacy.com` — the `mailto:` link and the displayed text. Save and refresh.

---

Built with care for Quillegacy.
