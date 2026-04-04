# Olivia & Miguel — Wedding Website

Single-page wedding website. Plain HTML/CSS/JS, no build step.

## Deploy to GitHub Pages in under 5 minutes

### 1. Create a GitHub repository

Go to [github.com/new](https://github.com/new) and create a **public** repository.
Name it anything — e.g. `boda-olivia-miguel`.

### 2. Push the files

```bash
git init
git add index.html README.md
git commit -m "Wedding website"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
git push -u origin main
```

### 3. Enable GitHub Pages

1. In your repo, go to **Settings → Pages**.
2. Under *Source*, select **Deploy from a branch**.
3. Choose branch `main`, folder `/ (root)`.
4. Click **Save**.

Your site will be live at `https://YOUR_USERNAME.github.io/YOUR_REPO/` within ~60 seconds.

---

## Adding real photos

1. Copy your photo files next to `index.html` — name them `photo1.jpg`, `photo2.jpg`, `photo3.jpg`, etc.
2. Open `index.html` and find this section near the bottom:

```js
const photos = [
  // 'photo1.jpg',
  // 'photo2.jpg',
  // 'photo3.jpg',
];
```

3. Uncomment the filenames (and add more as needed):

```js
const photos = [
  'photo1.jpg',
  'photo2.jpg',
  'photo3.jpg',
];
```

4. Save and push. Done — the carousel will use your photos instead of the placeholders.

---

## Customising

| What | Where in index.html |
|---|---|
| Carousel interval | `setInterval(next, 4000)` — change `4000` (ms) |
| Colours | `:root` CSS variables at the top |
| Fonts | Google Fonts `<link>` tag + `--font-serif` variable |
| All text content | directly in the HTML sections |
