# 36 Views of the Golden Gate Bridge
### by Brad Miller

---

## Site Structure

```
36views/
├── index.html        ← Home page (hero with image #2)
├── gallery.html      ← All 36 photos with lightbox
├── about.html        ← Series concept / Hokusai / Rivière
├── contact.html      ← Artist bio and email
└── photos/
    ├── 1.jpg
    ├── 2.jpg
    └── ... through 36.jpg
```

---

## Deploying to GitHub Pages

### Step 1 — Create GitHub account
Go to https://github.com → Sign Up (free)

### Step 2 — Create a repository
- Click the **+** icon → **New Repository**
- Name it: `36views`
- Set to **Public**
- Click **Create Repository**

### Step 3 — Upload site files
- Click **Add File → Upload Files**
- Drag in this entire folder's contents (all HTML files + the photos/ folder)
- Click **Commit Changes**

### Step 4 — Enable GitHub Pages
- Go to **Settings** tab → **Pages** (left sidebar)
- Under "Branch" select **main** → click **Save**
- Your site goes live at: `https://yourusername.github.io/36views`

---

## Connecting Your Custom Domain

### Step 5 — Buy your domain
Go to https://namecheap.com → search `36viewsofthegoldengatebridge.com` → purchase

### Step 6 — Add DNS records in Namecheap
Go to **Domain List → Manage → Advanced DNS** and add:

| Type   | Host | Value                  |
|--------|------|------------------------|
| A      | @    | 185.199.108.153        |
| A      | @    | 185.199.109.153        |
| A      | @    | 185.199.110.153        |
| A      | @    | 185.199.111.153        |
| CNAME  | www  | yourusername.github.io |

### Step 7 — Tell GitHub your domain
- Back in GitHub: **Settings → Pages**
- Under "Custom Domain" type: `36viewsofthegoldengatebridge.com`
- Check **Enforce HTTPS**
- Click Save

### Step 8 — Wait
DNS propagation: 15 minutes to 24 hours. Then your site is live at:
**https://36viewsofthegoldengatebridge.com**

---

## Editing the Site in the Future

### To add or swap a photo:
1. Go to your GitHub repository
2. Click the `photos/` folder
3. Click **Add File → Upload Files** to add new photos
4. To remove: click the photo → click the trash icon
5. Keep filenames numbered (e.g. `37.jpg`) and update `gallery.html` to change `const total = 36;` to your new count

### To edit text:
1. Go to your GitHub repository
2. Click any `.html` file
3. Click the **pencil icon** (Edit)
4. Make your changes
5. Click **Commit Changes**

### To reorder photos:
Simply rename the files (e.g. rename `5.jpg` to `05_new.jpg`) or update the order
in `gallery.html` in the JavaScript section.

---

## Notes
- The home page hero uses `photos/2.jpg`
- The contact page background uses `photos/15.jpg` (deer on Marin hillside)
- All fonts load from Google Fonts (free, no account needed)
- The Great Wave image on the About page loads from Wikimedia Commons (public domain)
