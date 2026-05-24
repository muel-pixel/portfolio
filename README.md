# Enwenye Samuel — Portfolio

Sammie (Enwenye Samuel) This is the portfolio for For Sammie.

## Structure

```
portfolio/
├── index.html          # Main portfolio page (single-file site)
├── images/             # All project images
│   ├── trip-trove-screens.png
│   ├── ridathabolt-mobile.jpg
│   ├── ridathabolt-persona.png
│   ├── ridathabolt-task-flow.png
│   ├── ridathabolt-annotated.png
│   ├── threadbound-hero.png
│   ├── threadbound-steps.png
│   ├── oracol-shirt.png
│   └── samior-shirt-pant.jpg
└── README.md
```

## Run locally

Just open `index.html` in your browser. No build step, no server needed.

For the cleanest local preview (some browsers block local images otherwise), serve it with any static server:

```bash
# If you have Python
python3 -m http.server 8000

# If you have Node
npx serve .
```

Then visit `http://localhost:8000`.

## Deploy to Vercel

### Option 1 — Drag & drop (fastest)
1. Go to https://vercel.com/new
2. Drag the entire `portfolio` folder onto the page
3. Done — Vercel will give you a `*.vercel.app` URL

### Option 2 — Via GitHub (recommended for ongoing updates)
1. Create a new GitHub repo
2. Push this folder to it
3. On Vercel, "New Project" → import the repo
4. Framework preset: **Other**
5. Build command: leave empty
6. Output directory: `.` (current folder)
7. Deploy

### Custom domain
After deploying, add your custom domain in Vercel's project settings under "Domains".

## Future: Next.js port

The HTML is structured so each `<section>` can become a React component:
- Hero → `<Hero />`
- Marquee strip → `<Marquee />`
- Work list → `<WorkList />` + `<WorkItem />`
- About → `<About />`
- Contact → `<Contact />`

Move CSS into `globals.css` (or Tailwind), images into `/public/images/`, swap `<img src="images/...">` for Next's `<Image src="/images/..." />`, and you're done.

## Fonts used
- **Fraunces** (variable serif, display) — Google Fonts
- **Inter** (sans, body) — Google Fonts
- **JetBrains Mono** (mono, labels) — Google Fonts

All loaded via Google Fonts CDN in the HTML head.

## Credits
Designed and built by Enwenye Samuel · 2026
