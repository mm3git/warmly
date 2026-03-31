# Warmly — Production Setup Guide

**Goal:** Get your family using the app in the next 15-20 minutes.

**What you'll do:**
1. Create a free Supabase account (database + real-time sync)
2. Copy your credentials into the app
3. Deploy to Netlify (instant hosting)
4. Send one URL to all 6 family members
5. Everyone logs in with their name and starts using it

---

## Step 1: Create a Supabase Account (5 minutes)

1. Go to **https://supabase.com** and click "Sign Up"
2. Create a new account using your email
3. Create a new project:
   - Click "New Project"
   - Give it a name: `warmly-family`
   - Choose any region (choose closest to you)
   - Set a secure password (you'll need this)
   - Click "Create New Project"
4. Wait for the project to initialize (1-2 minutes)

---

## Step 2: Get Your Credentials (2 minutes)

Once your project loads:

1. Click **"Settings"** (gear icon) → **"API"**
2. You'll see two important values:
   - **Project URL** (looks like `https://xxxxx.supabase.co`)
   - **API Key (anon)** (a long string of characters)

**Copy both of these.** You'll paste them into the app in the next step.

> **Keep these private** — don't share them in public messages, but it's safe to share with trusted family in a private message.

---

## Step 3: Connect the App (3 minutes)

1. Open `warmly-app-production.html` in a web browser
2. You'll see the setup screen
3. Click **"Setup Supabase"**
4. Paste your credentials:
   - **Supabase URL:** (paste Project URL)
   - **Supabase API Key:** (paste API Key)
5. Click **"Save & Connect"**
6. You'll see "✅ Setup Complete!"
7. Select your name from the dropdown: **Mark (你)**

**You're in!** The app is now ready to use.

---

## Step 4: Deploy to Netlify for Free Hosting (5 minutes)

So far, the app only works on your computer. To let your family access it from anywhere, we need to host it online.

1. Go to **https://netlify.com** and click "Sign up"
2. Sign up with your email or GitHub (easiest)
3. Once logged in, you'll see the dashboard
4. Drag and drop `warmly-app-production.html` directly into the "Deploy" area
5. Netlify will give you a live URL (looks like `https://your-app-xxx.netlify.app`)
6. **Copy this URL** — this is what you'll send to your family

The app is now live and everyone can access it from that URL.

---

## Step 5: Send to Your Family (2 minutes)

Send this message to your group chat (in Chinese for Mom):

---

### Message for Mom (中文):
```
媽媽，我們做好了一個家庭應用程式給你！

👉 點這個鏈接: [YOUR_NETLIFY_URL]

然後：
1. 選擇你的名字: 媽媽
2. 按「進入」

就可以開始了！告訴我任何問題。
```

---

### Message for Sisters & Grandkids (English):
```
Hey everyone! The Warmly app is ready for testing.

👉 Go to: [YOUR_NETLIFY_URL]

Login with your name:
- Mark (if you're Mark)
- Sister 1 / Sister 2 (if you're a sister)
- Grandson / Granddaughter (if you're a grandkid)

Then start supporting Mom! Send her cheers, challenge her to games, and see her streaks grow.

Mom is using Chinese, so the app will show Chinese for her. Everyone else gets English with a toggle.
```

---

## What Each Person Can Do

**Mom:**
- Tap "I stretched today" or "I walked today" when she does those activities
- Tap "Play a brain game" to play 3 rotating games daily
- See family messages in her feed
- Watch her streak grow
- Try to earn rewards (coffee treats)

**Everyone Else (Mark, Sisters, Grandkids):**
- See Mom's activities in real-time
- Send her cheers (with AI-suggested messages coming soon)
- Challenge her to games
- View leaderboards
- See a weekly summary of her progress

---

## Testing the App (What to Try First)

1. **Open the app in two browser tabs** — one as Mom, one as Mark
2. **As Mom:** Tap "I stretched today"
3. **As Mark:** You should see the activity appear instantly
4. **As Mark:** Send her a reaction or message
5. **As Mom:** See Mark's message appear in her feed

This proves the real-time sync is working. The whole family will see the same data.

---

## Important Notes

- **The app stores data in Supabase** — everyone's activities, messages, and game scores are shared
- **Language toggle** — at the top right, toggle between 中文 and English
- **Logout** — each person taps the door icon (🚪) to switch users
- **No passwords** — just select your name from the dropdown
- **Mobile-friendly** — Mom can tap "Add to Home Screen" on her iPhone to make it feel like a real app
- **Free tier** — Supabase and Netlify are both free for this use case

---

## Troubleshooting

**"Setup Required" error?**
- Check that both the URL and API Key are copied correctly
- Make sure you clicked "Save & Connect"
- If still stuck, try clearing browser cache and refreshing

**Can't see family members' activities?**
- Make sure everyone is using the same Supabase URL/Key
- The app auto-syncs every few seconds, so wait a moment after another person posts

**Game not working?**
- Games are still in development. In the meantime, use the activity buttons (Stretch/Walk) to track daily habits.

**Mom confused about setup?**
- You set it up for her on her phone (or computer) once. After that, she just selects her name and uses it.

---

## What's Next (Phase 2)

Once you've tested with the family for a few days:
1. Monitor which features get the most engagement
2. Note any technical issues
3. Plan for AI-suggested messages feature (the #1 priority from your feedback)
4. Gather qualitative feedback from Mom on what motivates her most

This real usage will inform your next round of improvements and eventually your investor conversations.

---

## File Locations

- **App file:** `warmly-app-production.html` — open this locally to test, or deploy to Netlify for live URL
- **Setup notes:** Keep your Supabase URL and API Key somewhere safe (password manager is fine)
- **Deployment link:** Bookmark your Netlify URL so you can quickly send it to others

---

Good luck! You're about to get real data on whether the family wellness loop actually works. 🚀

When you're ready to move to the next phase (landing page, waitlist, user interviews), let me know.
