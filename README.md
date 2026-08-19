# ARTfunny Portfolio Site

Clean, dark-theme multi-page portfolio for cartoon artwork, built for GitHub Pages.

**Live address (after setup):** https://Artfunny.github.io/ARTfunny2026/  
**Custom domain:** artfunny.co.uk (connect later when ready to leave Wix)

## Pages included
- Home
- Gallery
- Services
- ARToons
- Animations
- Contact

## How to put this on your GitHub repo

1. Go to https://github.com/Artfunny/ARTfunny2026
2. Click **Add file → Upload files**
3. Drag **all** the files and folders from this package into the root of the repository:
   - index.html
   - gallery.html
   - services.html
   - contact.html
   - artoons.html
   - animations.html
   - css/ (folder)
   - images/ (folder – currently empty)
   - videos/ (folder – currently empty)
   - README.md
4. Click **Commit changes**
5. Go to **Settings → Pages**
6. Under “Source” choose the branch `main` (or `master`) and folder `/ (root)`
7. Click Save

Within 1–2 minutes your site will be live at:  
https://Artfunny.github.io/ARTfunny2026/

## Adding your real images & videos later

### Gallery & ARToons
1. Upload your image files into the `images/` folder (via GitHub website: Add file → Upload files).
2. Open the relevant HTML file (gallery.html or artoons.html).
3. Find the placeholder blocks that look like this:

```html
<div class="gallery-item">
  <div class="placeholder-img">Add image<br>images/gallery-01.jpg</div>
  <div class="caption">Artwork Title 1</div>
</div>
```

4. Replace the inner `<div class="placeholder-img">...</div>` with a real image tag:

```html
<img src="images/your-real-filename.jpg" alt="Description of the artwork">
```

5. Change the caption text.
6. Commit the change. The site updates automatically.

### Animations
- Upload video files into the `videos/` folder, **or**
- Host the videos on YouTube / Vimeo and replace the placeholder with an embed code (I can help with that).

## Connecting your domain artfunny.co.uk later

When you are ready to point the domain away from Wix:

1. In the repo go to **Settings → Pages → Custom domain**
2. Enter `artfunny.co.uk` and save
3. At your domain registrar (where you manage artfunny.co.uk DNS) add:

**A records** (for the root domain):
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

**CNAME record** (for www):
```
www  →  Artfunny.github.io
```

4. Wait for DNS to propagate (can take from a few minutes up to 48 hours).
5. Back in GitHub Pages settings, tick **Enforce HTTPS**.

The site will then load on both artfunny.co.uk and www.artfunny.co.uk with a free SSL certificate and no Wix branding.

## Editing the site later
You can edit any page directly on the GitHub website:
- Click the file → pencil icon → make changes → Commit.
No coding software needed.

## Need changes?
Just tell me what you want adjusted (text, colours, extra pages, form, etc.) and I will update the files for you.
