# PrysmLab
Transform photos into art with PrysmLab's curated AI style library. Browse tested prompts—anime, vintage, neon, cartoons—with before/after previews. Copy-paste to any AI generator. Save collections, search by mood, create stunning visuals in seconds. Free for creators. 🚀

## Features
- Curated AI art style library
- Before/after preview grid
- One-click prompt copying
- Search + filter themes
- "Liked" gallery (Supabase-backed)
- Login/Sign-Up
- Local playground mode
- Clean, responsive UI

## Getting Started
### Clone repository:
```bash
git clone https://github.com/ahamlabs/prysmlab.git
cd prysmlab
```

## Local Development Setup
PrysmLab is a static HTML/JS project. There is no build step or server required, but it must be served through HTTP (not opened as a raw file).

### Option A - Run with VS Code Live Server (recommended)
1. Install the Live Server extension in VS Code
2. Open the project folder
3. Right-click index.html
4. Select "Open with Live Server"

```bash
http://127.0.0.1:5500/index.html
```

You should see the PrysmLab UI load, including sidebar, gallery, search bar, etc.

### Option B - Run with Python's simple server
In your terminal:
```bash
python -m http.server 8000
```

Then open:
```bash
http://localhost:8000
```

## Authentication (Optional)
The app includes login, sign-up, and "liked" features powered by Supabase.

To use your own database:
1. Create a Supabase project
2. Copy your Project URL and anon key
3. Replace these values in index.html:
```js
const SUPABASE_URL = "https://<your-project>.supabase.co";
const SUPABASE_ANON_KEY = "<your-anon-key>";
```
4. Create the necessary tables (examples: users, liked_themes)
5. Enable RLS (row-level security) if using production mode

If you only want to preview UI components, Supabase is not required.

## Contributing
We welcome improvements and additions!

How to contribute:
1. Fork the repository
2. Create a new branch:
```bash
git checkout -b branch-name
```
3. Make edits (README, themes, UI, etc.)
4. Commit and push:
```bash
git commit -m "Add setup instructions to README"
git push origin branch-name
```
5. Open a Pull Request

For documentation tasks, follow the existing style and keep explanations simple, clear, and beginner-friendly.

## Reporting Issues
If you find bugs or missing documentation:
- Open an issue in the repository
- Include screenshots or console errors when possible



