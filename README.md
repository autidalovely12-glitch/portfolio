# Personal Portfolio Website

A modern, responsive portfolio website with a beautiful dark blue/purple gradient theme. Features Home, About, Contact Info, and Photos pages.

## Features

- 🎨 Modern gradient design with purple-to-pink color scheme
- 📱 Fully responsive (mobile, tablet, desktop)
- ⚡ Smooth animations and transitions
- 🎯 Four main pages: Home, About, Contact Info, Photos
- 🌟 Interactive elements and hover effects
- 📧 Contact form (frontend ready)

## Pages

1. **Home** (`index.html`) - Landing page with hero section
2. **About** (`about.html`) - Personal information and skills
3. **Contact Info** (`contact.html`) - Contact details and message form
4. **Photos** (`photos.html`) - Photo gallery/portfolio showcase

## How to Push to GitHub and Deploy

### Step 1: Create a GitHub Account (if you don't have one)
1. Go to [github.com](https://github.com)
2. Sign up for a free account

### Step 2: Create a New Repository
1. Click the "+" icon in the top right corner
2. Select "New repository"
3. Name it: `yourusername.github.io` (replace `yourusername` with your actual GitHub username)
   - **Important**: This exact naming format enables GitHub Pages automatically!
   - Example: If your username is `johndoe`, name it `johndoe.github.io`
4. Make it **Public** (required for free GitHub Pages)
5. **Don't** initialize with README, .gitignore, or license (we already have files)
6. Click "Create repository"

### Step 3: Install Git (if not already installed)
1. Download Git from [git-scm.com](https://git-scm.com/download/win)
2. Install it with default settings
3. Open PowerShell or Command Prompt

### Step 4: Initialize Git and Push Your Code

Open PowerShell in your project folder (`C:\Users\rosal\OneDrive\Desktop\lovely`) and run these commands:

```powershell
# Initialize Git repository
git init

# Add all your files
git add .

# Create your first commit
git commit -m "Initial commit: Portfolio website"

# Add your GitHub repository as remote (replace YOUR_USERNAME with your actual username)
git remote add origin https://github.com/YOUR_USERNAME/YOUR_USERNAME.github.io.git

# Push to GitHub
git branch -M main
git push -u origin main
```

**Note**: You'll be prompted to enter your GitHub username and password (or personal access token).

### Step 5: Enable GitHub Pages
1. Go to your repository on GitHub
2. Click on **Settings** (top menu)
3. Scroll down to **Pages** (left sidebar)
4. Under "Source", select **main** branch
5. Click **Save**
6. Your site will be live at: `https://YOUR_USERNAME.github.io`

### Step 6: Wait for Deployment
- GitHub Pages usually takes 1-2 minutes to deploy
- You'll see a green checkmark when it's ready
- Visit your site URL to see it live!

## Customizing Your Portfolio

### Update Personal Information

1. **Name**: Replace "Your Name" in all HTML files
2. **Email**: Update in `contact.html` (line with `your.email@example.com`)
3. **Social Links**: Update LinkedIn, GitHub links in `contact.html`
4. **About Section**: Edit the text in `about.html`
5. **Skills**: Modify the skill cards in `about.html`
6. **Photos**: Replace photo placeholders in `photos.html` with your actual images

### Adding Your Photo

1. Add your photo to the project folder
2. In `index.html`, replace the `.image-placeholder` div with:
```html
<div class="hero-image">
    <img src="your-photo.jpg" alt="Your Name" style="width: 400px; height: 500px; object-fit: cover; border-radius: 20px; border: 2px solid rgba(102, 126, 234, 0.3);">
</div>
```

### Adding Real Photos to Photos Page

Replace the photo placeholders in `photos.html`:
```html
<div class="photo-card">
    <img src="photo1.jpg" alt="Description" style="width: 100%; height: 300px; object-fit: cover;">
    <div class="photo-overlay">
        <h3>Project Title</h3>
        <p>Description</p>
    </div>
</div>
```

## File Structure

```
lovely/
├── index.html          # Home page
├── about.html          # About page
├── contact.html        # Contact page
├── photos.html         # Photos page
├── styles.css          # Main stylesheet
├── script.js           # JavaScript functionality
└── README.md          # This file
```

## Technologies Used

- HTML5
- CSS3 (with CSS Grid and Flexbox)
- JavaScript (Vanilla JS)
- Google Fonts (Poppins)

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Troubleshooting

### Git Push Issues
- **Authentication Error**: Use a Personal Access Token instead of password
  - Go to GitHub Settings → Developer settings → Personal access tokens
  - Generate a new token with `repo` permissions
  - Use the token as your password

### GitHub Pages Not Working
- Make sure repository name is exactly `yourusername.github.io`
- Check that repository is set to **Public**
- Verify the `main` branch is selected in Pages settings
- Wait a few minutes for deployment to complete

### Images Not Showing
- Make sure image files are in the same folder or update paths
- Use relative paths like `./images/photo.jpg`
- Check file names match exactly (case-sensitive)

## Future Enhancements

- Add a blog section
- Integrate with a contact form service (Formspree, Netlify Forms)
- Add dark/light theme toggle
- Implement a blog or project showcase
- Add animations library (AOS, GSAP)

## License

This project is open source and available for personal use.

---

**Need Help?** Check out [GitHub Docs](https://docs.github.com/en/pages) for more information on GitHub Pages.

