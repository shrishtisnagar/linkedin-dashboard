# 📊 LinkedIn Analytics Dashboard

A free, privacy-first analytics dashboard for LinkedIn — built as a single HTML file. Upload your LinkedIn exports and instantly get charts, demographics, follower trends, post previews, and a clean printable PDF report. No server, no account, no data leaves your computer.

---

## ✨ Features

- **Company Page & Personal Profile** support
- **Interactive charts** — daily impressions, engagement trends, follower gains
- **Demographic breakdowns** — locations, seniority, job functions, industries
- **Post preview cards** — thumbnails and titles via LinkPreview API
- **Printable PDF report** — clean, branded, client-ready
- **365-Day View** — multi-month trend charts across all your uploads
- **Custom branding** — set your own primary and accent colours
- **Multi-client support** — manage multiple LinkedIn accounts in one place
- **100% local** — all data stored in your browser's localStorage, nothing sent to any server

---

## 🚀 Getting Started

### 1. Download
Just download `linkedin-analytics.html` — that's the entire app, one file.

### 2. Open in browser
Open the file in Chrome, Edge, or Firefox. No install, no build step.

### 3. Export your LinkedIn data
**For a Company Page**, go to LinkedIn Admin → Analytics → export two files:
- **Content** (contains Metrics + All Posts sheets)
- **Followers** (contains New Followers, Location, Seniority, etc.)

**For a Personal Profile**, go to LinkedIn → Analytics → export one file:
- Personal analytics file (contains Discovery, Engagement, Top Posts, Followers, Demographics sheets)

### 4. Upload
Click **+ Upload Report** in the sidebar, fill in the client name, select the month, choose Company or Personal, attach your file(s), and hit **Upload & Analyse**.

---

## 🖼 Post Previews (Optional)

Post cards can show real thumbnails and titles fetched via the [LinkPreview API](https://www.linkpreview.net).

1. Sign up free at [linkpreview.net](https://www.linkpreview.net) — no credit card needed
2. Copy your API key
3. In the dashboard go to **Settings → Post Preview API** → paste your key → Save
4. Post cards will now load thumbnails automatically. Results are cached locally so repeat views are instant.

> **Why a third-party API?** LinkedIn blocks browsers from fetching their pages directly (CORS). LinkPreview's server acts as a middleman — the same way WhatsApp or Notion generate link previews.

---

## 💾 Data & Privacy

| Question | Answer |
|---|---|
| Where is data stored? | Your browser's `localStorage` — on your own machine only |
| Is anything sent to a server? | No. Zero. Unless you use the LinkPreview API for post thumbnails |
| Does data persist between sessions? | Yes — close the tab, come back later, your data is still there |
| What clears my data? | Clearing browser cache ("Clear browsing data" → Site data) |
| Does it work across devices? | No — data lives in the specific browser on the specific machine you used |

**Tip:** If you're worried about losing data, use your browser's developer tools to export localStorage, or we recommend adding an Export/Import button (see Roadmap below).

---

## 📁 File Structure

```
linkedin-analytics.html   ← The entire app (HTML + CSS + JS, single file)
README.md
```

No dependencies to install. External libraries are loaded via CDN:
- [SheetJS (xlsx)](https://sheetjs.com) — parses Excel files
- [PapaParse](https://www.papaparse.com) — CSV parsing
- [Google Fonts (Poppins)](https://fonts.google.com)

---

## 🗺 Roadmap

- [ ] Export / Import data backup (JSON)
- [ ] 🤖 AI monthly commentary (OpenAI, Anthropic, Gemini)
- [ ] Engagement rate benchmarking across months
- [ ] Dark mode
- [ ] CSV export of parsed data

---

## 🤝 Contributing

PRs welcome. Since this is a single-file app, all changes go into `linkedin-analytics.html`.

Please test against both Company Page and Personal Profile exports before submitting.

---

## 📄 License

MIT — free to use, modify, and distribute.

---

*Built with ❤️ as a zero-dependency, privacy-first tool for LinkedIn managers and agencies.*

---

## 👤 Creator

Made by **Shrishti Nagar** — [linkedin.com/in/shrishtisnagar](https://www.linkedin.com/in/shrishtisnagar/)
