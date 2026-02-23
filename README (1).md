# APEX BOXING GYM — Website

A high-converting, fully responsive boxing gym landing page built with pure HTML/CSS/JS. No frameworks, no build steps, zero dependencies.

---

## 🚀 Deploy to Vercel in 3 Steps

### 1. Push to GitHub

```bash
git init
git add .
git commit -m "Initial commit — Apex Boxing site"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
git push -u origin main
```

### 2. Import into Vercel

1. Go to [vercel.com](https://vercel.com) → **Add New Project**
2. Click **Import** next to your GitHub repo
3. On the "Configure Project" screen, leave everything as default:
   - Framework Preset: **Other**
   - Build Command: *(leave blank)*
   - Output Directory: *(leave blank / use `.`)*
4. Click **Deploy** ✅

Your site will be live at `https://your-project.vercel.app` within ~30 seconds.

### 3. Add a Custom Domain (optional)

1. In Vercel dashboard → your project → **Settings → Domains**
2. Add your domain (e.g., `apexboxing.com`)
3. Update your DNS per Vercel's instructions

---

## 📁 File Structure

```
apex-boxing/
├── index.html     ← The entire website (single file)
├── vercel.json    ← Deployment + security headers config
└── README.md      ← This file
```

---

## ✏️ How to Customize

All content lives inside `index.html`. Search for these placeholders to update them quickly:

| What to change           | Search for                    |
|--------------------------|-------------------------------|
| Gym name                 | `APEX.BOXING`                 |
| Tagline / hero copy      | `TRAIN HARDER`                |
| Address                  | `2190-K Pimmit Dr`            |
| Phone number             | `(703) 555-0100`              |
| Email                    | `info@apexboxing.com`         |
| Coach names & bios       | `NIMA MAZHARI`, `GUSTAVO`     |
| Pricing amounts          | `$99`, `$149`, `$249`         |
| Brand color (red)        | `--red: #DC1414`              |
| Stats / numbers          | `data-to="500"`, etc.         |
| Social media links       | `href="#"` on FB/IG/YT        |

To change the accent color site-wide, edit one line in `:root`:
```css
--red: #DC1414;   /* swap to any color, e.g. #0066FF for blue */
```

---

## 🎯 Conversion Features Included

- **Live countdown timer** — urgency for the free trial offer
- **Scarcity notice** — "Only 8 spots left" messaging
- **Announcement bar** — persistent top-of-page CTA
- **Lead capture form** — name/email/phone/program, success state on submit
- **Animated counters** — stats animate into view on scroll
- **Scroll reveal** — elements fade in as user scrolls
- **Schedule tab switcher** — Adults / Kids toggle
- **Sticky nav** — becomes opaque with blur on scroll
- **Mobile menu** — full-screen overlay
- **Pricing urgency badges** — spots remaining per plan
- **Trust signals** — no contract, no card, cancel anytime

---

## 🔧 Adding Real Form Submissions

The form currently shows a success message client-side only. To connect it to a real backend:

**Option A — Formspree (free, 50 submissions/mo)**
```html
<!-- Replace the form-fields div's parent with: -->
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
  <!-- keep the same inputs -->
  <button type="submit" class="form-submit">CLAIM MY FREE WEEK →</button>
</form>
```

**Option B — Netlify Forms**
Add `netlify` attribute to the `<form>` tag if deploying on Netlify instead.

**Option C — Vercel Serverless Function**
Create `/api/submit.js` as a Vercel function and POST to it via `fetch`.

---

## 📱 Browser Support

Tested on Chrome, Firefox, Safari, Edge. Fully responsive from 320px to 4K.

---

*Replace placeholder content (gym name, coaches, address, pricing) before going live.*
