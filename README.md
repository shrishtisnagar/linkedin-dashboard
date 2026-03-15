# 📊 LinkedIn Analytics Dashboard

A free, privacy-first analytics dashboard for LinkedIn. Upload your LinkedIn exports and instantly get charts, demographics, follower trends, post previews, and a clean printable PDF report. 

---

## ✨ Features

- **Company Page & Personal Profile** support
- **Interactive charts** — daily impressions, engagement trends, follower gains
- **Demographic breakdowns** — locations, seniority, job functions, industries
- **Post preview cards** — thumbnails and titles via LinkPreview API
- **Printable PDF report** — clean, branded, client-ready
- **Custom branding** — set your own primary and accent colours
- **Multi-client support** — manage multiple LinkedIn accounts in one place
- **100% local** — all data stored in your browser's localStorage, nothing sent to any server

---

## 🚀 Getting Started

### 1. Visit
Visit https://shrishtisnagar.github.io/linkedin-dashboard/

### 2. Export your LinkedIn data
**For a Company Page**, go to LinkedIn Admin → Analytics → export two files:
- **Content** (contains Metrics + All Posts sheets)
- **Followers** (contains New Followers, Location, Seniority, etc.)

**For a Personal Profile**, go to LinkedIn → Analytics → export one file:
- Personal analytics file (contains Discovery, Engagement, Top Posts, Followers, Demographics sheets)

### 3. Upload
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

## 📄 License

MIT — free to use, modify, and distribute.

---

*Built with ❤️ as a zero-dependency, privacy-first tool for LinkedIn managers and agencies.*

---

## 👤 Creator

Made by **Shrishti Nagar** — [linkedin.com/in/shrishtisnagar](https://www.linkedin.com/in/shrishtisnagar/)
