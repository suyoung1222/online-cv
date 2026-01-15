# Personalization Guide for Jon Barron Template

This guide lists all the specific locations in `index.html` where you need to edit to personalize your website.

## File Structure
The template is already set up with a flat structure perfect for GitHub Pages:
- `index.html` - Main website file (in root directory)
- `stylesheet.css` - Stylesheet (in root directory)
- `images/` - Directory for images
- `data/` - Directory for PDFs, text files, and other data

## Personalization Points in `index.html`

### 1. Page Title (Line 6)
**Location:** `<head>` section
```html
<title>Jon Barron</title>
```
**Action:** Replace "Jon Barron" with your name

---

### 2. Meta Author Tag (Line 8)
**Location:** `<head>` section
```html
<meta name="author" content="Jon Barron">
```
**Action:** Replace "Jon Barron" with your name

---

### 3. Main Name Display (Line 23)
**Location:** Main content area, first column
```html
<p class="name" style="text-align: center;">
  Jon Barron
</p>
```
**Action:** Replace "Jon Barron" with your name

---

### 4. Bio/Description Text (Lines 26-29)
**Location:** Main content area, first column, below name
```html
<p>
  I'm a principal research scientist at <a href="https://deepmind.google/">Google DeepMind</a> in San Francisco, where I lead a small team that mostly works on <a href="https://www.matthewtancik.com/nerf">NeRF</a>.
  At Google I've worked on <a href="https://www.google.com/glass/start/">Glass</a>,  <a href="https://ai.googleblog.com/2014/04/lens-blur-in-new-google-camera-app.html">Lens Blur</a>, <a href="https://ai.googleblog.com/2014/10/hdr-low-light-and-high-dynamic-range.html">HDR+</a>, <a href="https://blog.google/products/google-ar-vr/introducing-next-generation-jump/">VR</a>, <a href="https://ai.googleblog.com/2017/10/portrait-mode-on-pixel-2-and-pixel-2-xl.html">Portrait Mode</a>, <a href="https://ai.googleblog.com/2020/12/portrait-light-enhancing-portrait.html">Portrait Light</a>, <a href="https://blog.google/products/maps/three-maps-updates-io-2022/">Maps</a>, and <a href="https://research.google/blog/bringing-3d-shoppable-products-online-with-generative-ai/">Shopping</a>.
  I did my PhD at <a href="http://www.eecs.berkeley.edu/">UC Berkeley</a>, where I was advised by <a href="http://www.cs.berkeley.edu/~malik/">Jitendra Malik</a>.
  I've received the <a href="https://www.thecvf.com/?page_id=413#YRA">PAMI Young Researcher Award</a>.
</p>
```
**Action:** Replace this entire paragraph with your own bio/description. You can keep or remove the links as needed.

---

### 5. Social Links (Lines 32-37)
**Location:** Main content area, first column, below bio
```html
<p style="text-align:center">
  <a href="mailto:jonbarron@gmail.com">Email</a> &nbsp;/&nbsp;
  <a href="data/JonBarron-CV.pdf">CV</a> &nbsp;/&nbsp;
  <a href="data/JonBarron-bio.txt">Bio</a> &nbsp;/&nbsp;
  <a href="https://scholar.google.com/citations?hl=en&user=jktWnL8AAAAJ">Scholar</a> &nbsp;/&nbsp;
  <a href="https://twitter.com/jon_barron">Twitter</a> &nbsp;/&nbsp;
  <a href="https://github.com/jonbarron/">Github</a>
</p>
```
**Action:** Update each link:
- **Email:** Replace `mailto:jonbarron@gmail.com` with your email
- **CV:** Replace `data/JonBarron-CV.pdf` with your CV path (or remove if you don't have one)
- **Bio:** Replace `data/JonBarron-bio.txt` with your bio file path (or remove if you don't have one)
- **Scholar:** Replace the Google Scholar URL with your profile URL (or remove if not applicable)
- **Twitter:** Replace `https://twitter.com/jon_barron` with your Twitter URL (or remove if not applicable)
- **Github:** Replace `https://github.com/jonbarron/` with your GitHub URL (or remove if not applicable)
- **LinkedIn:** You can add a LinkedIn link here if desired: `<a href="https://linkedin.com/in/yourprofile">LinkedIn</a> &nbsp;/&nbsp;`

---

### 6. Profile Image (Line 41)
**Location:** Main content area, second column (right side)
```html
<a href="images/JonBarron.jpg"><img style="width:100%;max-width:100%;object-fit: cover; border-radius: 50%;" alt="profile photo" src="images/JonBarron.jpg" class="hoverZoomLink"></a>
```
**Action:** 
1. Replace `images/JonBarron.jpg` with your profile image path (e.g., `images/yourname.jpg`)
2. Place your profile image in the `images/` directory
3. Recommended: Use a square image for best results (the border-radius: 50% makes it circular)

---

### 7. Research Section (Lines 48-50)
**Location:** Below the header section
```html
<h2>Research</h2>
<p>
  I'm interested in computer vision, deep learning, generative AI, and image processing. Most of my research is about inferring the physical world (shape, motion, color, light, etc) from images, usually with radiance fields. Some papers are <span class="highlight">highlighted</span>.
</p>
```
**Action:** Replace with your own research interests/description

---

### 8. Publications/Projects Section
**Location:** Lines 55 onwards
The template includes many research papers and projects. You'll need to:
- Remove or replace the existing publications/projects with your own
- Each entry follows a similar structure with images, titles, authors, links, and descriptions
- You can keep the structure but replace the content

---

## Additional Files to Update

### Favicon (Line 10)
```html
<link rel="shortcut icon" href="images/favicon/favicon.ico" type="image/x-icon">
```
**Action:** Replace `images/favicon/favicon.ico` with your favicon path, or remove this line if you don't have a favicon

### CV and Bio Files
If you want to keep the CV and Bio links working:
- Place your CV PDF in `data/YourName-CV.pdf` and update the link in line 33
- Place your bio text file in `data/YourName-bio.txt` and update the link in line 34

---

## Quick Checklist

- [ ] Update page title (line 6)
- [ ] Update meta author (line 8)
- [ ] Update main name display (line 23)
- [ ] Replace bio/description (lines 26-29)
- [ ] Update email link (line 32)
- [ ] Update CV link (line 33) or remove
- [ ] Update Bio link (line 34) or remove
- [ ] Update Scholar link (line 35) or remove
- [ ] Update Twitter link (line 36) or remove
- [ ] Update GitHub link (line 37) or remove
- [ ] Add LinkedIn link (optional)
- [ ] Replace profile image path (line 41)
- [ ] Add your profile image to `images/` directory
- [ ] Update research description (lines 48-50)
- [ ] Replace publications/projects with your own (lines 55+)
- [ ] Update favicon (line 10) or remove

---

## Notes

- The file structure is already flat and GitHub Pages compatible
- All images should be placed in the `images/` directory
- All data files (PDFs, text files) should be placed in the `data/` directory
- The template uses relative paths, so everything should work correctly on GitHub Pages
- Your existing `.git` configuration is preserved, so you can push to your current repository
