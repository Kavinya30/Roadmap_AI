# 🚀 RoadmapAI — Deployment Guide (Using FREE Gemini API)

## STEP 1 — Get Your FREE Gemini API Key

1. Go to → **https://aistudio.google.com/apikey**
2. Sign in with your Google account (any Gmail works!)
3. Click **"Create API Key"**
4. Copy the key (it looks like: `AIzaSy...`)

✅ That's it — Gemini is completely FREE with generous limits!

---

## STEP 2 — Push to GitHub

### Create the repo:
1. Go to **https://github.com/new**
2. Name it: `roadmapai`
3. Set to **Public**
4. Do NOT add README or .gitignore
5. Click **"Create repository"**

### Push your code (run in your terminal):
```bash
# Unzip roadmapai.zip first, then cd into it:
cd roadmapai

# Replace YOUR_USERNAME with your GitHub username:
git remote add origin https://github.com/YOUR_USERNAME/roadmapai.git
git branch -M main
git push -u origin main
```

✅ Code is on GitHub!

---

## STEP 3 — Deploy on Vercel (FREE)

1. Go to → **https://vercel.com**
2. Click **"Sign up"** → continue with GitHub
3. Click **"New Project"** → Import your `roadmapai` repo
4. **Before clicking Deploy** → open **"Environment Variables"**
5. Add:
   - **Name**: `GEMINI_API_KEY`
   - **Value**: your key from Step 1
6. Click **"Deploy"**

⏳ Wait ~2 minutes → Your app is LIVE! 🎉

---

## STEP 4 — Test It

1. Open your Vercel URL (e.g. `roadmapai.vercel.app`)
2. Type `Backend Developer` and click Generate
3. Watch the AI build your roadmap in ~15 seconds!

---

## Troubleshooting

**"GEMINI_API_KEY is not configured" error?**
→ Make sure the env variable name is exactly `GEMINI_API_KEY` in Vercel
→ Go to Vercel → Settings → Environment Variables → add it → Redeploy

**Build errors locally?**
→ Run `npm install` first
→ Need Node.js 18+

---

## Making Changes Later

```bash
git add .
git commit -m "my change"
git push
```
Vercel auto-redeploys on every push!
