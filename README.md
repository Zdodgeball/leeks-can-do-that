# Leeks Can Do That

A small static website about the amazing things leeks can do. Plain HTML and CSS, no build step, ready to host on Vercel.

## Files

- `index.html`: the whole page. Each leek fact is one `<section class="thing">`.
- `styles.css`: layout, type, and the green gradient that runs down the page.
- `favicon.svg`: the tab icon.
- `vercel.json`: Vercel settings (clean URLs).

## Preview locally

```sh
python3 -m http.server 3000
```

Then open http://localhost:3000.

## Deploy to Vercel

1. Create a repo on GitHub and push this one:
   ```sh
   git remote add origin https://github.com/<your-username>/leeks-can-do-that.git
   git push -u origin main
   ```
2. Go to https://vercel.com/new and import the repo.
3. Set the framework preset to **Other**. Leave the build command and output directory empty.
4. Click **Deploy**.

Or deploy straight from this folder with the Vercel CLI:

```sh
npx vercel
```

## Add a new leek fact

Copy a `<section class="thing">` block in `index.html` and edit the heading and paragraph. The background color for each section is set in `styles.css` with `main > .thing:nth-child(n)`, so add a matching line (or adjust the existing ones) if you add more than nine sections.
