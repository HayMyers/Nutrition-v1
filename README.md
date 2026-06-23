# Nutrition v1

A private, installable workout + nutrition tracker. Each person who installs it gets their own
account and data, stored privately on their own device. No servers, no sign-up fees, no backend.

## What's in this folder

Upload **all** of these to the same place (the repository root):

| File | What it is |
|------|------------|
| `index.html` | The entire app |
| `manifest.json` | Makes it installable as an app |
| `sw.js` | Service worker — lets it work offline & update cleanly |
| `icon-192.png` | App icon (small) |
| `icon-512.png` | App icon (large) |
| `apple-touch-icon.png` | iPhone home-screen icon |

---

## Part 1 — Put it online (free, ~5 minutes)

You'll host it with **GitHub Pages**.

1. Go to **github.com** and sign in (create a free account if needed).
2. Click **+** (top right) → **New repository**.
3. Name it something like `nutrition-v1`. Set it to **Public**. Click **Create repository**.
4. On the new repo page, click **uploading an existing file**.
5. Drag in **all 6 files** from this folder. Click **Commit changes**.
6. Go to the repo's **Settings** → **Pages** (left sidebar).
7. Under **Branch**, pick **main** and **/ (root)**, then **Save**.
8. Wait ~1 minute, refresh. GitHub shows your live link, like:
   `https://YOUR-USERNAME.github.io/nutrition-v1/`

That link is your app. It's served over HTTPS, which is what makes the camera barcode
scanner and food search work.

### Updating later
If you ever change `index.html`, re-upload it to the repo (Add file → Upload files → commit).
Everyone gets the update next time they open the app.

---

## Part 2 — Add it to your iPhone home screen

1. Open your link in **Safari** (must be Safari, not Chrome).
2. Tap the **Share** button (square with an up arrow).
3. Scroll down → **Add to Home Screen** → **Add**.
4. It now has its own icon and opens full-screen like a real app.

(On Android: open in Chrome → menu **⋮** → **Install app / Add to Home screen**.)

---

## Part 3 — Share with your friends

Just send them the link. Each friend:
1. Opens it in Safari and adds it to their home screen (Part 2).
2. Creates their own account inside the app.
3. Their data is completely private to their own phone.

---

## Good to know

- **Accounts are per-device.** Because there's no server, an account lives on the phone where
  it was created. Logging in on a different phone won't show the same data. To move to a new
  phone, use **Settings → Export backup** on the old one and **Import backup** on the new one.
- **Camera & food search need internet + HTTPS.** They work on your hosted link, not when
  opening the file directly. Manual food entry always works.
- **Your numbers** (calories, protein/carbs/fat) come from the Mifflin–St Jeor equation plus
  your activity level, and the workout templates follow evidence-based volume and rep guidance.
  Tweak anything in **Settings**.

Built as a personal tool — not medical advice. Check with a professional for personalized
medical, nutrition, or training guidance.
