# Jyoti Mahila Cooperative Website

A static website for Jyoti Mahila Cooperative - empowering women through collaboration, sustainability, and community-driven excellence.

## 📁 Folder Structure

```
jyoti-static-website/
├── index.html          # Home page
├── about.html          # About Us page
├── css/
│   └── style.css       # Main stylesheet
├── images/             # Create this folder and add your images
│   ├── logo.png
│   ├── 0.jpeg
│   ├── 1.jpeg
│   ├── 5.jpeg
│   ├── 7.jpeg
│   ├── 12.jpeg
│   ├── 13.jpeg
│   ├── 22.jpeg
│   ├── 31.jpeg
│   ├── 35.jpeg
│   └── community.jpeg
└── README.md           # This file
```

## 🚀 How to Deploy to GitHub Pages

### Step 1: Prepare Your Images

1. Create an `images` folder in the website directory
2. Add all your images to this folder:
   - logo.png (your cooperative logo)
   - 0.jpeg, 1.jpeg, 5.jpeg, 7.jpeg, 12.jpeg, 13.jpeg, 22.jpeg, 31.jpeg, 35.jpeg
   - community.jpeg

### Step 2: Create GitHub Repository

1. Go to [github.com](https://github.com) and sign in
2. Click the "+" icon → "New repository"
3. Repository name: `jyoti-coop` (or any name you prefer)
4. Make it **Public**
5. Click "Create repository"

### Step 3: Upload Files to GitHub

**Option A: Using GitHub Website (Easiest)**
1. On your repository page, click "uploading an existing file"
2. Drag and drop ALL files and folders (index.html, about.html, css folder, images folder)
3. Scroll down and click "Commit changes"

**Option B: Using Git Command Line**
```bash
# Navigate to your website folder
cd jyoti-static-website

# Initialize git
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit"

# Add remote (replace YOUR-USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR-USERNAME/jyoti-coop.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 4: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (top menu)
3. Scroll down to **Pages** (left sidebar)
4. Under "Source", select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **Save**
6. Wait 2-3 minutes

Your site will be live at: `https://YOUR-USERNAME.github.io/jyoti-coop/`

### Step 5: Connect Your Custom Domain

1. In GitHub Pages settings, under "Custom domain", enter: `yourwebsite.com`
2. Click **Save**
3. Go to your domain registrar (where you bought your domain)
4. Add these DNS records:

**A Records** (point to GitHub Pages):
```
Type: A
Name: @
Value: 185.199.108.153

Type: A
Name: @
Value: 185.199.109.153

Type: A
Name: @
Value: 185.199.110.153

Type: A
Name: @
Value: 185.199.111.153
```

**CNAME Record** (for www subdomain):
```
Type: CNAME
Name: www
Value: YOUR-USERNAME.github.io
```

5. Wait 24-48 hours for DNS propagation
6. Enable "Enforce HTTPS" in GitHub Pages settings (after DNS is active)

## 📝 How to Update Your Website

### Method 1: Through GitHub Website
1. Go to your repository
2. Click on the file you want to edit (e.g., `index.html`)
3. Click the pencil icon (Edit)
4. Make your changes
5. Scroll down and click "Commit changes"

### Method 2: Using Git
```bash
# Make changes to your files
# Then:
git add .
git commit -m "Updated content"
git push
```

Changes will appear on your live site within a few minutes.

## 🎨 Customizing Your Website

### Change Logo Size
In `css/style.css`, find:
```css
.logo img {
    height: 80px; /* Change this value */
}
```

### Update Contact Information
Edit the footer section in both `index.html` and `about.html`:
```html
<p>Email: info@jyotimahila.coop</p>
<p>Phone: +977-XXX-XXXXXX</p>
```

### Add More Pages
1. Copy `about.html`
2. Rename it (e.g., `contact.html`)
3. Update the content
4. Add a link in the navigation of all pages

## 💡 Tips

- All images should be in the `images/` folder
- Keep image file sizes under 1MB for faster loading
- Test your site locally by opening `index.html` in a browser before uploading
- Use Chrome DevTools (F12) to check for errors

## 🆘 Troubleshooting

**Images not showing?**
- Check that image filenames match exactly (case-sensitive)
- Ensure images are in the `images/` folder
- Clear browser cache (Ctrl + F5)

**Custom domain not working?**
- Wait 24-48 hours for DNS propagation
- Check DNS settings with: [whatsmydns.net](https://www.whatsmydns.net/)
- Ensure HTTPS is enabled in GitHub Pages settings

**Changes not appearing?**
- Clear browser cache
- Wait a few minutes (GitHub Pages can take 1-5 minutes to update)
- Check if commit was successful on GitHub

## 📞 Support

For any issues with deployment, refer to:
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [GitHub Community Forum](https://github.community/)

---

**Made with ❤️ for Jyoti Mahila Cooperative**
