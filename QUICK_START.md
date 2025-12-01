# ⚡ LumoAI GitHub Pages - Quick Start

Get your LumoAI chat app live on GitHub Pages in **5 minutes**!

---

## 📦 What You Get

✅ **File:** `lumo-github-pages.html` - Standalone chat app
✅ **Features:** Dark/light theme, settings panel, connection status
✅ **Setup:** 2 minutes on GitHub Pages
✅ **Backend:** Connects to your Render API

---

## 🚀 The 5-Minute Setup

### Step 1: Create GitHub Repo (1 min)
```bash
# Go to github.com → New Repository → "lumo-frontend"
# (Keep it public for GitHub Pages)
```

### Step 2: Clone & Add Files (1 min)
```bash
git clone https://github.com/YOUR-USERNAME/lumo-frontend.git
cd lumo-frontend

# Copy the HTML file as index.html
cp lumo-github-pages.html index.html

# Create .gitignore (optional)
echo "node_modules/" > .gitignore

# Create README
echo "# LumoAI Chat" > README.md
```

### Step 3: Push to GitHub (1 min)
```bash
git add .
git commit -m "Deploy LumoAI to GitHub Pages"
git push -u origin main
```

### Step 4: Enable GitHub Pages (1 min)
1. Go to **Settings** → **Pages**
2. Source: `Deploy from a branch`
3. Branch: `main` → `/root`
4. Click **Save**
5. Wait 1-2 minutes

### Step 5: Connect Backend (1 min)
1. Open: `https://YOUR-USERNAME.github.io/lumo-frontend/`
2. Click **⚙️ Settings** (top-right)
3. Paste Render URL: `https://your-app.onrender.com`
4. Click **Test Connection** → Should be ✅ **Connected**
5. Click **Save**

**Done!** 🎉

---

## 🎯 Your URLs

**Chat App:**
```
https://YOUR-USERNAME.github.io/lumo-frontend/
```

**Render Backend (Example):**
```
https://lumo-api.onrender.com
```

---

## 🔧 Render Backend URL Format

When configuring in app settings, use:
```
https://your-backend-name.onrender.com
```

**NOT:**
- ❌ `https://your-backend-name.onrender.com/` (with slash)
- ❌ `https://your-backend-name.onrender.com/api` (with /api)
- ✅ Just the base URL

---

## ⚙️ If "Disconnected"

### Check 1: Is backend running?
```bash
curl https://your-backend-name.onrender.com/api/conversations
# Should return JSON, not 404 or error
```

### Check 2: Enable CORS on backend

**Express.js:**
```javascript
const cors = require('express-cors');
app.use(cors());
```

**Flask:**
```python
from flask_cors import CORS
CORS(app)
```

### Check 3: Render app asleep?
- Visit Render dashboard
- Click "Redeploy" to wake it up
- Or use paid tier for always-on

---

## 📝 Your Files Checklist

```
✅ lumo-github-pages.html  → Copy as index.html
✅ README.md              → Project description
✅ GITHUB_PAGES_SETUP.md  → Detailed guide
✅ .github/workflows/     → Auto-deployment (optional)
```

---

## 💬 Test It Out

After connecting backend:

1. Type: **"Hello Lumo!"**
2. Press Enter or click Send
3. Wait for response
4. AI should reply with Gen-Z personality
5. Click **📋 Copy** to copy response

---

## 🎨 Customize (Optional)

Edit `index.html`:

**Change theme color:**
```css
--primary: hsl(203.7736 87.6033% 52.5490%);
/* Use any HSL color */
```

**Change title:**
```html
<title>My AI Chat App</title>
```

**Change placeholder:**
```html
placeholder="Ask me anything..."
```

---

## 🚀 Update App

When you make changes:
```bash
git add index.html
git commit -m "Update UI"
git push
# Auto-deploys in 1-2 minutes
```

---

## 📚 Need More Help?

- **Full Setup:** See `GITHUB_PAGES_SETUP.md`
- **Troubleshooting:** See `README-GITHUB-PAGES.md`
- **Backend Info:** See `BACKEND_README.md`

---

## ✨ Features

| Feature | How |
|---------|-----|
| **Dark Mode** | Click 🌙 icon |
| **Change Backend** | Click ⚙️ Settings |
| **Copy Message** | Click 📋 Copy button |
| **Check Status** | Green/Red indicator (top) |
| **Mobile Support** | Opens on any device |

---

## 🎯 Common Issues

| Problem | Solution |
|---------|----------|
| "Disconnected" | Check backend URL in settings |
| 404 Error | Make sure `index.html` is in root |
| Messages not sending | Test connection in settings |
| Render asleep | Visit Render dashboard to wake |
| CORS error | Add CORS to backend |

---

## 💡 Pro Tips

- 💾 Settings saved in browser storage
- 🔒 No secrets in frontend code
- 🌍 Works offline (until you send a message)
- ⏱️ Render spins down after 15 mins inactive
- 🔄 Can switch backends anytime

---

## 🎉 Next Steps

1. ✅ Copy `lumo-github-pages.html` to your repo
2. ✅ Push to GitHub
3. ✅ Enable Pages
4. ✅ Get your Render backend URL
5. ✅ Configure in settings
6. ✅ Start chatting!

---

## 📞 Quick Links

- **GitHub Pages Docs:** https://docs.github.com/en/pages
- **Render Docs:** https://render.com/docs
- **Hugging Face API:** https://huggingface.co/docs/hub/api

---

**Ready?** Deploy now! 🚀🤭✨
