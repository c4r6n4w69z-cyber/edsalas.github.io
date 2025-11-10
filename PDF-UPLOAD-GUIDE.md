# PDF Upload Guide for Ed Salas Website

## Where to Upload Your PDF Files

You have **3 main options** for uploading and hosting your PDF files:

---

## Option 1: GitHub Repository (Recommended for GitHub Pages)

### Steps:
1. **Create a `documents/` folder** in your repository:
   - In GitHub, go to your repository
   - Click "Add file" → "Create new file"
   - Type `documents/README.md` (this creates the folder)
   - Click "Commit new file"

2. **Upload your PDF files**:
   - Navigate to the `documents/` folder
   - Click "Add file" → "Upload files"
   - Drag and drop your PDF files (e.g., `leadership-ai-era.pdf`, `neuroleadership-guide.pdf`, `transformation-framework.pdf`)
   - Click "Commit changes"

3. **Update the HTML links**:
   - In `index.html`, find the download links (around line 590-640)
   - Replace `href="#"` with `href="documents/your-file-name.pdf"`
   - Example: `href="documents/leadership-ai-era.pdf"`

### Your PDF URL format:
```
https://yourusername.github.io/documents/your-file.pdf
```

---

## Option 2: Cloud Storage Services (Easiest)

### A. Google Drive:
1. Upload PDF to Google Drive
2. Right-click the file → "Get link"
3. Change permissions to "Anyone with the link can view"
4. Copy the sharing link
5. Use this format for direct download:
   ```
   https://drive.google.com/uc?export=download&id=FILE_ID
   ```
   (Extract FILE_ID from the sharing link)

### B. Dropbox:
1. Upload PDF to Dropbox
2. Right-click → "Share"
3. Create a link
4. Change the end of URL from `?dl=0` to `?dl=1`
5. Use this link in your HTML

### C. OneDrive:
1. Upload PDF to OneDrive
2. Right-click → "Share"
3. Get the sharing link
4. Use the "Embed" option for direct access

---

## Option 3: GitHub Releases (For Larger Files)

### Steps:
1. Go to your repository on GitHub
2. Click "Releases" (on the right sidebar)
3. Click "Create a new release"
4. Fill in tag version (e.g., `v1.0`)
5. Upload your PDF files as release assets
6. Publish the release
7. Right-click the PDF link → "Copy link address"
8. Use this link in your HTML

---

## How to Update the HTML After Uploading

### For Each PDF Document:

Find the download link in `index.html` (search for "Download PDF"):

**Before:**
```html
<a href="#" onclick="alert('PDF would be downloaded here'); return false;">
```

**After:**
```html
<a href="documents/your-file-name.pdf" download>
```

Or for cloud storage:
```html
<a href="https://your-cloud-storage-link.pdf" target="_blank">
```

---

## Example: Complete Update

### If you're using GitHub repository:

1. **Create folder structure:**
   ```
   your-repo/
   ├── index.html
   ├── index-es.html
   ├── styles.css
   └── documents/
       ├── leadership-ai-era.pdf
       ├── neuroleadership-guide.pdf
       └── transformation-framework.pdf
   ```

2. **Update index.html (Document 1):**
   ```html
   <!-- Find this section around line 590 -->
   <a href="documents/leadership-ai-era.pdf" download style="display: flex; align-items: center; justify-content: center; gap: 0.5rem; padding: 1rem; background: var(--vibrant-teal); color: white; text-decoration: none; border-radius: 10px; font-weight: 600; transition: all 0.3s ease;">
       <svg width="20" height="20" viewBox="0 0 24 24" fill="white">
           <path d="M5 20h14v-2H5v2zM19 9h-4V3H9v6H5l7 7 7-7z"/>
       </svg>
       Download PDF
   </a>
   ```

3. **Repeat for all 3 documents** with their respective filenames

---

## File Naming Best Practices

- Use lowercase letters
- Replace spaces with hyphens (-)
- Keep names descriptive but concise
- Examples:
  - ✅ `leadership-ai-era.pdf`
  - ✅ `neuroleadership-guide-2024.pdf`
  - ✅ `transformation-framework.pdf`
  - ❌ `My Document With Spaces.pdf`
  - ❌ `file1.pdf`

---

## Maximum File Size Recommendations

- **GitHub Repository**: Up to 25MB per file (100MB max)
- **Google Drive**: No practical limit (15GB free storage)
- **Dropbox**: Based on your plan (2GB free)
- **OneDrive**: Based on your plan (5GB free)

---

## Testing Your Upload

1. **Commit and push your changes**
2. **Visit your live site**
3. **Click the "Download PDF" button**
4. **Verify the PDF downloads correctly**

---

## Need Help?

If you have questions about:
- Where your repository is located
- How to access GitHub
- How to upload files
- How to edit HTML

Please let me know and I can provide more specific guidance!

---

## Quick Start Checklist

- [ ] Choose upload method (GitHub/Cloud Storage)
- [ ] Create `documents/` folder (if using GitHub)
- [ ] Upload your 3 PDF files
- [ ] Copy the file URLs/paths
- [ ] Update `index.html` with actual PDF links
- [ ] Update `index-es.html` (Spanish version) with same links
- [ ] Test on your live site
- [ ] Verify downloads work correctly

**Current Status:** Your website has placeholder PDF cards ready. You just need to upload the actual files and update the links!
