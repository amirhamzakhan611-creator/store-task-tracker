# 🏪 Store Maintenance — GPM Checklist (PWA)

WhatsApp-style Daily / Weekly / Monthly / Quarterly maintenance checklist app — GitHub Pages pe deploy karke **phone mein real app jaisa install** kar sakte ho. 100% offline, no internet needed after install.

---

## 📁 Files in this repo

```
├── index.html          → Main app (sab kuch isi file mein hai)
├── manifest.json        → PWA settings (app name, icon, colors)
├── service-worker.js    → Offline caching (no internet ke baad bhi chalega)
├── icons/
│   ├── icon-192.png
│   ├── icon-512.png
│   └── apple-touch-icon.png
├── .nojekyll             → GitHub Pages ko batata hai ki Jekyll mat use karo
└── README.md             → Yeh file
```

---

## 🚀 GitHub par Upload kaise kare (Step-by-Step)

### Option A — GitHub website se (Easy, no computer needed)

1. **github.com** par jao aur login karo (`amirhamzakhan611-creator`)
2. **New repository** banao:
   - Repository name: `gpm-maintenance-checklist` (ya koi bhi naam)
   - **Public** select karo
   - **Create repository** click karo
3. Repo khulne ke baad **"uploading an existing file"** link click karo
4. Yeh saari files (index.html, manifest.json, service-worker.js, icons folder, .nojekyll, README.md) **drag & drop** kar do
5. Niche **"Commit changes"** button dabao

### Option B — Computer se Git command line (agar laptop available hai)

```bash
git clone https://github.com/amirhamzakhan611-creator/gpm-maintenance-checklist.git
cd gpm-maintenance-checklist
# yahan saari files copy karo
git add .
git commit -m "Add GPM maintenance checklist PWA"
git push origin main
```

---

## 🌐 GitHub Pages Enable kaise kare (App live karne ke liye)

1. Apne repo mein jao → **Settings** tab click karo
2. Left sidebar mein **Pages** click karo
3. **Source** mein select karo: `Deploy from a branch`
4. **Branch** mein select karo: `main` aur folder `/ (root)`
5. **Save** dabao
6. 1-2 minute wait karo — top par ek green box mein link milega:
   ```
   https://amirhamzakhan611-creator.github.io/gpm-maintenance-checklist/
   ```

---

## 📱 Phone mein App ki tarah Install kaise kare

### Android (Chrome):
1. Upar wala link Chrome mein open karo
2. 3-dot menu (⋮) → **"Install app"** ya **"Add to Home screen"**
3. **Install** dabao → Home screen pe app icon aa jayega ✅
4. Ab bina internet ke bhi khulega — bilkul real app jaisa!

### iPhone (Safari):
1. Link Safari mein open karo
2. Share button (□↑) → **"Add to Home Screen"**
3. **Add** dabao → app icon home screen pe ✅

---

## ✨ App Features

- ✅ **4 Tabs** — Daily (37 tasks) / Weekly (31 tasks) / Monthly (36 tasks) / Quarterly (40 tasks)
- ✅ **Tap to check** — task complete karne ke liye bas tap karo, green tick lagega
- ✅ **Auto-Save** — progress phone mein hi save hota hai (browser ki localStorage), app band karke fir se kholo to wahi se continue
- ✅ **100% Offline** — ek baar install karne ke baad internet ki zaroorat nahi
- ✅ **WhatsApp Copy Button** — pura report ek click mein copy hoke WhatsApp group mein paste kar sakte ho
- ✅ **Reset Button** — har tab ka apna reset (next day/week/month ke liye fresh start)
- ✅ **Progress Bar** — har section ka live progress dikhta hai

---

## 🔧 Update kaise kare (future mein tasks add/change karne ke liye)

`index.html` file ke andar `<ul class="cl">...</ul>` blocks mein naye `<li>` tasks add kar sakte ho. Format:

```html
<li onclick="tog(this)">
  <span class="cb">✓</span>
  <span class="tt">
    <strong>Task Name</strong>
    <span>Task description yahan likho</span>
  </span>
  <span class="pr H">H</span>  <!-- H=High, M=Medium, L=Low -->
</li>
```

File update karne ke baad GitHub par dobara upload/commit karo — Pages automatically update ho jayega (1-2 min mein).

---

## 📞 Support

Koi issue ho to GitHub repo ke **Issues** tab mein likh sakte ho, ya phir Claude se dobara pooch sakte ho changes ke liye.

---

**Made for:** Amir Khan — Senior Electrician Technician, Jubilant FoodWorks (Domino's India)  
**Region:** DPI West 1, Mumbai
