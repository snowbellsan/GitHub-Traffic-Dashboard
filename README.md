# 🌟 GitHub Traffic Dashboard 🌟

![Dashboard preview](https://via.placeholder.com/1200x600/667eea/764ba2?text=GitHub+Traffic+Dashboard+Preview)  
*Neon-styled, animated traffic analyzer for every repository under your GitHub account.*

---

## 🚀 Features

| Feature | Description |
|---------|-------------|
| **All-in-one view** | Fetches **Views**, **Unique Visitors**, **Clones**, and **Unique Cloners** for **up to 100** repos in a single click. |
| **Interactive table** | Sort any column (asc / desc) with a single button. |
| **Responsive bar chart** | Powered by **Chart.js** with smooth bounce animations and custom neon colors. |
| **Futuristic UI** | Gradient backgrounds, glowing text, floating titles, pulsing effects, and glass-morphism cards. |
| **Secure token handling** | Uses GitHub **Classic Personal Access Token** (never stored). |
| **Zero backend** | Pure client-side HTML + CSS + JS – works locally or hosted on GitHub Pages. |

---

## 🎨 Demo

Open the live demo on GitHub Pages:  
👉 **[your-username.github.io/github-traffic-dashboard](https://snowbellsan.github.io/Github-Traffic-Dashboard)**  

*(Replace `your-username` with your actual GitHub username after enabling Pages.)*

---

## 🛠️ How to Use

1. **Clone or download** the repository.
2. Open `index.html` in any modern browser.
3. Enter:
   - **GitHub username**
   - **Classic Personal Access Token** (`repo` scope required)
4. Click **🚀 データ取得！** – the dashboard will populate instantly.
5. Use the **Sort** controls to reorder the table and chart.

> **Tip:** Keep your token private. Never commit it to the repo.

---

## 🔒 Creating a Classic Token

1. Go to **Settings → Developer settings → Personal access tokens → Tokens (classic)**.
2. Click **Generate new token (classic)**.
3. Give it a name, select the **`repo`** scope, and generate.
4. Copy the token and paste it into the dashboard.

---

## 📊 Data Sources (GitHub API)

| Endpoint | Data |
|----------|------|
| `GET /user/repos` | List of repositories (max 100) |
| `GET /repos/:owner/:repo/traffic/views` | Views + Unique visitors |
| `GET /repos/:owner/:repo/traffic/clones` | Clones + Unique cloners |

*Rate-limit aware – works with the default 5000 requests/hour for authenticated users.*

---

## 🎨 Tech Stack

- **HTML5** – Structure
- **CSS3** – Gradient animations, glass-morphism, neon glow, Orbitron font
- **Vanilla JavaScript (ES6+)** – API calls, sorting, chart rendering
- **Chart.js** – Interactive bar chart
- **Google Fonts** – `Orbitron` for sci-fi vibe

---

## 🚧 Deployment on GitHub Pages

```bash
git clone https://github.com/your-username/github-traffic-dashboard.git
cd github-traffic-dashboard
# (optional) git remote set-url origin <your-repo>
git push origin main
