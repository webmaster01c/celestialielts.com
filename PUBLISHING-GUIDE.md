# 🚀 Celestial IELTS — Complete Publishing Guide
### Zero coding knowledge required. Takes about 30–45 minutes total.

---

## What you'll set up:
- **GitHub** — stores your website files (free, forever)
- **GitHub Pages** — publishes the website live (free, forever)
- **Cloudflare** — makes it load fast from India, Canada, UK & UAE (free)
- **Your domain** — connected to everything above

---

## STEP 1 — Create a GitHub account
1. Go to **https://github.com**
2. Click **"Sign up"**
3. Enter your email, create a password, choose a username (e.g. `celestialielts`)
4. Verify your email and log in

---

## STEP 2 — Create your repository (your website's home)
1. Once logged in, click the **"+"** icon at the top right
2. Click **"New repository"**
3. Under **Repository name**, type exactly: `celestialielts.com`
   *(or whatever your domain name is — it helps with organisation)*
4. Make sure **"Public"** is selected
5. Tick **"Add a README file"**
6. Click **"Create repository"** (green button)

---

## STEP 3 — Upload your website files
1. Inside your new repository, click **"Add file"** → **"Upload files"**
2. Drag and drop ALL the files I gave you:
   - `index.html`
   - `sitemap.xml`
   - `robots.txt`
   - The entire `pages/` folder (with all 5 HTML files inside)
   - The `images/` folder (empty for now — we'll add your photos here later)
3. At the bottom, under **"Commit changes"**, just click **"Commit changes"**
4. Wait a few seconds for everything to upload

> 💡 **Tip:** Upload the `pages` folder by creating it first. Click "Add file" → "Create new file", type `pages/placeholder.txt`, then commit. Then upload your pages into it.

---

## STEP 4 — Turn on GitHub Pages (publish the site)
1. In your repository, click **"Settings"** (top tab)
2. In the left sidebar, click **"Pages"**
3. Under **"Source"**, select **"Deploy from a branch"**
4. Under **"Branch"**, select **"main"** and **"/ (root)"**
5. Click **"Save"**
6. Wait 2–3 minutes, then refresh — you'll see a green banner with your site URL like: `https://celestialielts.github.io/celestialielts.com/`
7. **Test it** — click the link to make sure the site loads!

---

## STEP 5 — Set up Cloudflare (free CDN for speed + your domain)
1. Go to **https://cloudflare.com** and sign up free
2. Click **"Add a Site"**
3. Enter your domain name (e.g. `celestialielts.com`) and click **"Add Site"**
4. Select the **Free plan** and continue
5. Cloudflare will scan your domain's DNS — click **"Continue"**
6. You'll see two **Cloudflare nameservers** (looks like `xxx.ns.cloudflare.com`)
7. **Copy both of these** — you'll need them in the next step

---

## STEP 6 — Point your domain to Cloudflare
1. Log into wherever you bought your domain (GoDaddy / Namecheap / BigRock etc.)
2. Find **"Nameservers"** or **"DNS Settings"** for your domain
3. Replace the existing nameservers with the two Cloudflare nameservers you copied
4. Save. This can take up to 24 hours to fully update (usually much faster)

---

## STEP 7 — Connect your domain to GitHub Pages in Cloudflare
Once Cloudflare is active on your domain:

1. In Cloudflare dashboard → **DNS** → **Add record**
2. Add these 4 records (GitHub's IPs):

| Type | Name | Content |
|------|------|---------|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |

3. Also add:

| Type | Name | Content |
|------|------|---------|
| CNAME | www | YOUR-GITHUB-USERNAME.github.io |

4. Make sure the **orange cloud (Proxy)** is ON for all records

---

## STEP 8 — Add your custom domain in GitHub
1. Back in GitHub → your repository → **Settings** → **Pages**
2. Under **"Custom domain"**, type `celestialielts.com` (your actual domain)
3. Click **"Save"**
4. Tick **"Enforce HTTPS"** if available
5. Wait 10–30 minutes for SSL certificate to issue

---

## STEP 9 — Add your personal details (before going live)
Open each HTML file and replace these placeholders:

| Placeholder | Replace with |
|-------------|-------------|
| `YOUR_WHATSAPP_NUMBER` | Your number in format: `919876543210` (no + sign, no spaces) |
| `YOUR_TELEGRAM_LINK` | Your Telegram username or channel link |
| `YOUR_SPOTIFY_LINK` | Your Spotify podcast/show link |
| `VIDEO_ID_1`, `VIDEO_ID_2` etc. | Your YouTube video IDs (the part after `?v=` in the URL) |
| `celestialielts.com` in footers | Already correct if that's your domain |

**To edit files on GitHub:**
1. Click the file name in your repository
2. Click the **pencil icon** (Edit) at the top right
3. Make your changes
4. Click **"Commit changes"** at the bottom

---

## STEP 10 — Add your photos
1. Take or choose your best photo (even a good phone photo works)
2. In GitHub, go to your `images/` folder
3. Upload your photo — name it `trainer.jpg`
4. In `index.html` and `pages/about.html`, find this comment:
   ```
   <!-- Replace with: <img src="/images/trainer.jpg" ... -->
   ```
5. Replace that whole `<div class="about-img-placeholder">` block with:
   ```html
   <img src="/images/trainer.jpg" alt="Celestial IELTS certified trainer" style="width:100%;border-radius:32px;object-fit:cover;aspect-ratio:4/5;" />
   ```

---

## STEP 11 — Submit to Google Search Console
This gets Google to index your site and appear in search results.

1. Go to **https://search.google.com/search-console**
2. Sign in with your Google account
3. Click **"Add Property"** → enter `https://celestialielts.com`
4. Choose **"HTML tag"** verification method — copy the tag Google gives you
5. In your `index.html`, paste it inside the `<head>` section
6. Commit the change, wait 5 minutes, then click **"Verify"** in Google
7. Once verified, click **"Sitemaps"** → enter `sitemap.xml` → Submit
8. Google will now crawl and index your site within a few days

---

## STEP 12 — Submit to Bing (for India traffic)
Bing is widely used in India and feeds into some Indian search engines.

1. Go to **https://www.bing.com/webmasters**
2. Sign in and add your site
3. Submit your sitemap URL: `https://celestialielts.com/sitemap.xml`

---

## Your website checklist ✅

- [ ] GitHub account created
- [ ] Repository created and files uploaded
- [ ] GitHub Pages enabled
- [ ] Cloudflare set up
- [ ] Domain pointing to Cloudflare
- [ ] Custom domain added in GitHub Pages
- [ ] HTTPS enabled
- [ ] WhatsApp number added throughout
- [ ] Telegram link added
- [ ] Spotify link added
- [ ] YouTube video IDs added
- [ ] Your photo uploaded
- [ ] Google Search Console set up
- [ ] Sitemap submitted to Google
- [ ] Site tested on mobile and desktop

---

## How to update the website later
Every time you want to change something:
1. Go to **github.com** → your repository
2. Click the file you want to edit
3. Click the **pencil icon**
4. Make your change
5. Click **"Commit changes"**
6. The live site updates in 1–3 minutes automatically ✅

---

## How to add new student result cards to the website
1. Use the **Result Card Generator** (the tool in our Claude chat) to create a card
2. Download the card image
3. Upload it to your GitHub `images/` folder
4. In `pages/success-stories.html`, copy an existing `.score-card` block and update the student name, score, quote, and image

---

## Need help? 
Message us on WhatsApp — we're here to help you through every step.

---

*Celestial IELTS · celestialielts.com · Built with ❤️ and gold & purple*
