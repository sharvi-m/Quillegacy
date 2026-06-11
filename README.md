# Quillegacy Website

A simple two-file website for **Quillegacy**, the senior memory booklet initiative.

## Files

| File         | What it does                                          |
| ------------ | ----------------------------------------------------- |
| `index.html` | All the text and content of the site.                 |
| `style.css`  | All the colors, fonts, and layout.                    |
| `README.md`  | This file. Instructions for editing.                  |

That's it — just two files to maintain.

## How to view the site

Double-click `index.html` and it will open in your web browser.
No installation, no build step, no server needed.

## How to edit the text

Open `index.html` in any text editor (TextEdit, VS Code, Notepad, etc.).

Look for the section you want to change — each one is clearly marked with a comment like:

```html
<!-- ===== ABOUT US ===== -->
```

Just change the words between the `<p>` (paragraph) or `<h2>` (heading) tags.
Save the file and refresh your browser.

### Example

To change the mission statement, find this in `index.html`:

```html
<p class="lead">
  Our mission is to help seniors pass their memories...
</p>
```

Change the text inside, save, and refresh.

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

## How to put it online (free options)

The easiest free hosting options:

1. **GitHub Pages** — push these files to a GitHub repo, enable Pages in settings.
2. **Netlify Drop** — drag the folder onto [app.netlify.com/drop](https://app.netlify.com/drop).
3. **Vercel** — connect a GitHub repo at [vercel.com](https://vercel.com).

All three are free and take less than 5 minutes.

## Sections on the site

1. **Hero** — the opening line and mission tagline
2. **About Us** — mission statement and project description
3. **Impact** — three cards: for Families, for Seniors, for Future Generations
4. **Who We Are** — the team of 8th graders

---

Built with care for Quillegacy.
