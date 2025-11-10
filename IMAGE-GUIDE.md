# Image Integration Guide for Ed Salas Website

## Current Status
✅ All website structure and content complete
⏳ Placeholder images in place - ready for real photos
🎯 Next step: Replace placeholders with actual speaking/forum photos

## Where Real Images Are Needed

### 1. **Hero Section Profile Photo**
**Location:** Top banner (hero section)  
**Current:** `images/profile.jpg` with fallback to placeholder  
**Dimensions:** 180x180px circular  
**Recommendation:**  
- Professional headshot with neutral/solid background
- High resolution (at least 400x400px before cropping to circle)
- Warm, approachable expression
- Business casual attire

### 2. **Sticky Sidebar Profile Photo**
**Location:** Right sidebar (appears on scroll)  
**Current:** Same as hero - `images/profile.jpg`  
**Dimensions:** 65x65px circular  
**Note:** Uses same image as hero section, automatically resized

### 3. **Speaking & Forums Section** (3 Images Needed)
**Location:** Near bottom of page, before Contact section  
**Current:** Placeholder images with gradient overlays  
**Dimensions:** 600x400px (3:2 aspect ratio)

#### Image 1: Global Leadership Summit
- **Caption:** "Global Leadership Summit" - Bentonville, Arkansas - 2024
- **Ideal photo:** Speaking at podium/stage, audience visible, professional conference setting
- **Alternative:** Panel discussion, workshop facilitation, or keynote moment

#### Image 2: HR Innovation Forum  
- **Caption:** "HR Innovation Forum" - San José, Costa Rica - 2023
- **Ideal photo:** Speaking at event, presenting to group, or panel participation
- **Alternative:** Workshop setting, breakout session, or networking at forum

#### Image 3: Executive Coaching Summit
- **Caption:** "Executive Coaching Summit" - Miami, Florida - 2022
- **Ideal photo:** Teaching/facilitating moment, coaching demonstration, or summit presentation
- **Alternative:** Group coaching session, masterclass, or certification workshop

## How to Add Your Images

### Option 1: Use Local Images (Recommended)
1. Create an `images/` folder in your project directory (already exists)
2. Add your images with these names:
   - `images/profile.jpg` - Your professional headshot
   - `images/speaking1.jpg` - Global Leadership Summit photo
   - `images/speaking2.jpg` - HR Innovation Forum photo  
   - `images/speaking3.jpg` - Executive Coaching Summit photo

### Option 2: Update HTML Directly
Find these lines in `index.html` and update the URLs:

**Speaking Section** (around line 650-730):
```html
<!-- Image 1 -->
background: ... url('https://via.placeholder.com/600x400/1A3A52/FFFFFF?text=Leadership+Conference')
Replace with: url('images/speaking1.jpg')

<!-- Image 2 -->
background: ... url('https://via.placeholder.com/600x400/34495E/FFFFFF?text=HR+Innovation+Forum')
Replace with: url('images/speaking2.jpg')

<!-- Image 3 -->
background: ... url('https://via.placeholder.com/600x400/6B2737/FFFFFF?text=Executive+Coaching+Summit')
Replace with: url('images/speaking3.jpg')
```

## Image Requirements

### Technical Specifications
- **Profile Photos:** JPG or PNG, minimum 400x400px
- **Speaking Photos:** JPG, recommended 1200x800px (will be displayed at 600x400px for crisp quality on retina displays)
- **File Size:** Keep under 500KB each for fast loading
- **Format:** JPG preferred for photos (better compression)

### Visual Guidelines
- **Lighting:** Well-lit, professional photography
- **Background:** Relevant to the event context (conference halls, stages, audiences)
- **Composition:** You should be clearly visible and recognizable
- **Quality:** Sharp, in-focus, minimal noise/grain
- **Professionalism:** Business appropriate attire and setting

## Alternative: Quick Fix with Stock Photos
If you don't have professional speaking photos yet, you can temporarily use:
- Professional business stock photos from sites like Unsplash or Pexels
- Generic conference/speaking images until you have your own
- Remove the "Real Images Coming Soon" note after adding any images

## After Adding Images

### 1. Test Locally
Open `index.html` in your browser to verify:
- [ ] Profile photo displays correctly (circular crop looks good)
- [ ] Speaking images load without errors
- [ ] Images are appropriately sized and don't distort
- [ ] Page loads quickly (images not too large)

### 2. Update Contact WhatsApp
Replace `https://wa.me/yourphonenumber` with your actual WhatsApp number:
```html
href="https://wa.me/15551234567"  <!-- Replace with your number, including country code -->
```

### 3. Ready to Publish!
Once images are added and tested, you're ready to deploy online.

## Publishing Options (Next Step)

### Option A: GitHub Pages (Free, Easiest)
1. Create GitHub account (if don't have one)
2. Create new repository named `yourusername.github.io`
3. Upload all files (index.html, styles.css, images folder)
4. Site will be live at `https://yourusername.github.io`

### Option B: Netlify (Free, Drag & Drop)
1. Go to netlify.com
2. Sign up (free)
3. Drag your project folder to Netlify
4. Get custom domain like `edsalas.netlify.app`

### Option C: Custom Domain
1. Buy domain (edsalas.com, edsalasleadership.com, etc.)
2. Use any hosting above + connect domain
3. Professional email possible (ed@yourdomain.com)

## Questions to Answer Before Publishing

1. **Do you have professional photos ready?**
   - Profile headshot?
   - At least 1-2 speaking/forum photos?

2. **What's your WhatsApp number for contact?**
   - Need full international format: +1-555-123-4567

3. **Preferred website URL?**
   - GitHub Pages: username.github.io
   - Custom domain: edsalas.com (requires purchase)
   - Netlify: edsalas.netlify.app

4. **Email for contact form?**
   - Formspree placeholder needs real email address

---

## Ready to Add Images?

**If you have photos ready:**
1. Place them in the `images/` folder with names above
2. Open index.html in browser to test
3. Let me know and we'll proceed to publishing

**If you need help with images:**
1. Let me know what photos you have available
2. I can help you find the exact HTML lines to update
3. We can use temporary stock images while you gather professional photos

**Want to publish with placeholders?**
- We can deploy now with placeholder images
- Update later when you have professional photos
- Site will work perfectly, just less authentic visually

Let me know which path you'd like to take!
