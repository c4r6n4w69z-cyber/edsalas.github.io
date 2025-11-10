# Publishing Your Website Online - Step by Step

## You Have 3 Easy Options to Publish

---

## ⭐ OPTION 1: GitHub Pages (Recommended - 100% Free)

### Why Choose This?
- Completely free forever
- Professional URL: `yourusername.github.io`
- Easy to update anytime
- Backed by Microsoft/GitHub
- Can add custom domain later

### Steps:

#### 1. Create GitHub Account
- Go to https://github.com
- Click "Sign up"
- Choose username (suggestion: `edsalasay` or `edsalas`)
- Verify email

#### 2. Create Repository
- Click the `+` icon (top right)
- Select "New repository"
- **Repository name:** `yourusername.github.io` (e.g., `edsalasay.github.io`)
- Make it **Public**
- Don't initialize with README
- Click "Create repository"

#### 3. Upload Your Files
Two ways to do this:

**Easy Way (Drag & Drop):**
- In your new repository, click "uploading an existing file"
- Drag these files/folders from your Desktop:
  - `index.html`
  - `styles.css`
  - `images/` folder (if you have photos ready)
- Write commit message: "Initial website launch"
- Click "Commit changes"

**Command Line Way (if comfortable with terminal):**
```bash
cd "/Users/edsalas/Desktop/AI Projects"
git init
git add index.html styles.css images/
git commit -m "Initial website launch"
git remote add origin https://github.com/yourusername/yourusername.github.io.git
git push -u origin main
```

#### 4. Enable GitHub Pages
- Go to repository Settings → Pages
- Under "Source", select `main` branch
- Click Save
- Wait 1-2 minutes

#### 5. Visit Your Live Site!
Your website will be live at:
**`https://yourusername.github.io`**

### Updating Your Site Later
Just upload new files or edit directly on GitHub - changes appear in minutes!

---

## ⚡ OPTION 2: Netlify (Fastest Setup)

### Why Choose This?
- Easiest method (drag & drop)
- Instant deployment
- Free SSL certificate
- Custom domain support
- Automatic previews

### Steps:

#### 1. Go to Netlify
- Visit https://netlify.com
- Click "Sign up" (can use GitHub account)

#### 2. Deploy Site
- Click "Add new site" → "Deploy manually"
- **Drag your entire project folder** onto the Netlify drop zone
  - Select `/Users/edsalas/Desktop/AI Projects` folder
- Wait 30 seconds...
- Done! Your site is live!

#### 3. Your URL
Netlify gives you: `random-name-12345.netlify.app`

#### 4. Customize URL (Optional)
- Go to Site settings → Domain management
- Change to: `edsalas.netlify.app` or `edsalas-leadership.netlify.app`

### Updating Your Site
Just drag the updated folder again - instant deployment!

---

## 🌐 OPTION 3: Custom Domain (Most Professional)

### Why Choose This?
- Professional: `edsalas.com` or `edsalasleadership.com`
- Full control
- Professional email possible
- Best for business use

### Steps:

#### 1. Buy a Domain
**Recommended Registrars:**
- **Namecheap** (cheapest, ~$10/year)
- **Google Domains** (easy, ~$12/year)
- **GoDaddy** (well-known, ~$15/year)

**Domain Suggestions:**
- `edsalas.com`
- `eduardosalas.com`
- `edsalasleadership.com`
- `edsalasconsulting.com`

#### 2. Choose Hosting Method
Once you have domain, connect it to:
- **GitHub Pages** (Option 1 above) + custom domain
- **Netlify** (Option 2 above) + custom domain
- **Traditional hosting** (Bluehost, SiteGround, etc.)

#### 3. Connect Domain
Each platform has simple guides:
- GitHub Pages: Settings → Pages → Custom domain
- Netlify: Site settings → Domain management → Add custom domain

---

## 📊 Quick Comparison

| Feature | GitHub Pages | Netlify | Custom Domain |
|---------|-------------|---------|---------------|
| **Cost** | FREE | FREE | $10-15/year |
| **Speed** | Fast | Fastest | Fast |
| **Ease** | Easy | Easiest | Medium |
| **URL** | username.github.io | random.netlify.app | yourdomain.com |
| **Updates** | Git/Upload | Drag & drop | Varies |
| **Professional** | ⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ |

---

## 🎯 My Recommendation for You

### Start with GitHub Pages (Option 1)
**Why?**
1. Free forever
2. Professional enough for speaking engagements
3. Easy to maintain
4. Can add custom domain anytime
5. URL `edsalasay.github.io` looks professional

### Later: Add Custom Domain
When ready for maximum professionalism:
1. Buy `edsalas.com` (~$10)
2. Connect to GitHub Pages
3. Now accessible at `edsalas.com`

---

## Before Publishing Checklist

### Required Updates
- [ ] Add WhatsApp number (replace `yourphonenumber`)
- [ ] Add real profile photo (or keep placeholder)
- [ ] Add speaking photos (or keep placeholders)
- [ ] Test locally - everything works?

### Optional Enhancements
- [ ] Update contact form email (Formspree)
- [ ] Add Google Analytics code
- [ ] Create favicon (small site icon)
- [ ] Add meta description for SEO

---

## After Publishing

### 1. Test Your Live Site
Visit your URL and check:
- [ ] All pages load correctly
- [ ] Links work (LinkedIn, Instagram, WhatsApp)
- [ ] Images display (or placeholders show)
- [ ] Contact form works
- [ ] Responsive on mobile

### 2. Share Your Site
- Update LinkedIn profile with website URL
- Add to email signature
- Share in Instagram bio
- Include in speaking proposals

### 3. SEO Setup (Optional but Recommended)
- Submit site to Google Search Console
- Create Google My Business profile
- Share on social media for backlinks

---

## Common Questions

**Q: Can I publish without real photos?**  
A: Yes! Placeholders look professional. Add real photos later.

**Q: How do I update after publishing?**  
A: Just re-upload files (GitHub/Netlify) - changes appear in minutes.

**Q: What if I want to change hosting later?**  
A: Easy! Download your files and upload to new platform.

**Q: Do I need technical skills?**  
A: No! All options are designed for non-technical users.

**Q: How long until my site is live?**  
A: GitHub Pages: 2-5 minutes | Netlify: 30 seconds

**Q: Can I use my site for business?**  
A: Absolutely! All options support professional/business use.

---

## Ready to Publish?

### Next Steps:
1. **Choose your option** (I recommend GitHub Pages to start)
2. **Follow the steps above** (takes 10-15 minutes)
3. **Let me know your URL** and I'll verify everything works!

### Need Help?
If you get stuck at any step, just let me know exactly where and I'll guide you through it!

### Want to Test First?
We can do a "practice run" where I walk you through each step before actually publishing.

---

## Contact Form Setup (After Publishing)

Your contact form currently points to Formspree placeholder. To make it work:

1. Go to https://formspree.io
2. Sign up (free plan: 50 submissions/month)
3. Create new form
4. Copy your form ID
5. Update line in index.html:
   ```html
   <form action="https://formspree.io/f/YOUR_FORM_ID">
   ```
6. Re-upload file

**OR** simply use:
- Direct email link: `mailto:your@email.com`
- WhatsApp for primary contact
- LinkedIn messages

---

Let me know which option appeals to you and I'll help you get live! 🚀
