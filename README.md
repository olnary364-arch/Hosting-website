# Nary OL - Personal Portfolio Website

A modern, professional, and responsive personal portfolio website built with HTML5, CSS3, and JavaScript.

## 📁 Project Structure

```
OL Nary/
├── index.html          # Main HTML file with all sections
├── styles.css          # All styling and responsive design
├── script.js           # JavaScript for interactivity
└── README.md           # This file
```

## ✨ Features

### 🎨 Design
- **Dark Navy/Blue Hero Section** - Eye-catching gradient background with animated shapes
- **White/Light Background** - Clean, professional appearance
- **Blue Accent Color** - Consistent branding throughout
- **Dark Mode Support** - Toggle between light and dark themes
- **Glassmorphism Effects** - Modern frosted glass navigation bar
- **Scroll Progress Indicator** - Visual progress bar at the top
- **Animated Skill Bars** - Progress bars that animate on scroll
- **Fully Responsive** - Works perfectly on desktop, tablet, and mobile devices
- **Poppins Font** - Modern Google Font typography

### 🖼️ Animations & Effects
- **Preloader** - Smooth loading animation
- **Scroll Animations** - Fade-in elements on scroll
- **Floating Badges** - Animated badges on hero image
- **Hover Effects** - Smooth transitions on all interactive elements
- **Gradient Borders & Text** - Modern gradient accents
- **Shimmer Effect** - Animated shimmer on progress bars
- **Back-to-Top Button** - Smooth scroll to top

### 📑 Sections Included

1. **Navigation Bar**
   - Logo with icon (Nary OL)
   - Menu links with icons to all sections
   - Download CV button
   - Mobile hamburger menu with animation
   - Theme toggle (light/dark mode)
   - Active section highlighting

2. **Hero Section**
   - Greeting and introduction
   - Call-to-action buttons with icons
   - Social media icons (GitHub, LinkedIn, Facebook, Email)
   - Floating badges (Web Developer, 5+ Projects)
   - Professional student portrait with animated circular background

3. **About Me Section**
   - Personal introduction
   - Key information with icons (Name, Age, Study, Location, Email)
   - Professional image
   - Read More button

4. **Skills Section**
   - 6 skill cards with icons and animated progress bars
   - Skills: HTML, CSS, JavaScript, Python, Git & GitHub, Database
   - Hover animations with gradient icon backgrounds
   - Shimmer effect on progress bars

5. **Projects Section**
   - 3 project cards with images
   - Project descriptions and technology tags with icons
   - Hover effects and smooth animations

6. **Education Section**
   - Education details with icon
   - Study period and description
   - Date with calendar icon

7. **Contact Section**
   - Contact information boxes with icons (Email, Phone, Location)
   - Contact form with validation
   - Send Message button with icon

8. **Footer**
   - Logo and navigation links with icons
   - Copyright information
   - Back-to-top button

### 🚀 Functionality
- **Smooth Scrolling** - Smooth navigation between sections
- **Dark Mode Toggle** - Switch between light and dark themes (persisted via localStorage)
- **Scroll Progress Indicator** - Shows scroll progress at top of page
- **Preloader** - Loading animation on page load
- **Mobile Hamburger Menu** - Responsive navigation for smaller screens
- **Hover Animations** - Interactive elements with smooth transitions
- **Animated Skill Bars** - Progress bars animate when scrolled into view
- **Scroll Animations** - Elements fade in on scroll
- **Form Validation** - Contact form with email validation
- **Back-to-Top Button** - Easy navigation to top of page
- **Active Navigation Highlighting** - Current section indicator

## 💻 How to Use

### Opening the Website

1. Navigate to the project folder: `c:\Users\NARY.OL\Desktop\OL Nary`
2. Double-click `index.html` to open in your default browser
3. Or right-click `index.html` → Open with → Your preferred browser

### Customizing the Content

#### Update Personal Information
Open `index.html` and find these sections to customize:

- **Hero Section**: Change greeting, name, subtitle, description
- **About Section**: Update personal details and bio
- **Contact Section**: Update email, phone, location

#### Replace Placeholder Images
The website currently uses placeholder images. To use your own:

1. Save your images in the project folder
2. Find `<img src="https://via.placeholder.com/...">` in `index.html`
3. Replace with: `<img src="your-image-name.jpg" alt="description">`

Example:
```html
<!-- Before -->
<img src="https://via.placeholder.com/300x350/1e3c72/ffffff?text=Nary+OL" alt="Nary OL">

<!-- After -->
<img src="profile.jpg" alt="Nary OL">
```

#### Update Skills Progress
In the Skills section, find progress bars like:
```html
<div class="progress" data-width="90%"></div>
```

Change the `data-width` percentage to reflect your actual skill level. The bars will animate when you scroll to them.

#### Add/Modify Projects
In the Projects section, duplicate a project card and update:
- Project image
- Project title and description
- Technology tags (with icons)

#### Add Your CV File
1. Save your CV file (PDF, Word, etc.) in the project folder
2. Find the CV button in the navbar
3. In `script.js`, uncomment and update this line:
   ```javascript
   window.location.href = 'your-cv.pdf';
   ```

#### Update Social Media Links
Find social icon links in the Hero section:
```html
<a href="https://github.com/yourusername" class="social-icon" title="GitHub">
    <i class="fab fa-github"></i>
</a>
```

Replace `#` with your actual social media URLs.

### Dark Mode
A theme toggle button is available in the navigation bar. Your preference is saved in localStorage and persists across sessions.

## 🎯 Technical Details

### Dependencies
- **Font Awesome 6.4.0** - Icon library (loaded via CDN)
- **Google Fonts (Poppins)** - Modern typography (loaded via CDN)
- No additional frameworks or dependencies needed

### Browser Compatibility
- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

### Performance
- Optimized CSS animations with cubic-bezier easing
- Smooth scroll behavior
- Lightweight JavaScript with IntersectionObserver
- IntersectionObserver-based lazy animations for performance
- Responsive images

## 📱 Responsive Breakpoints

- **Desktop**: 1200px and above (full layout)
- **Tablet**: 769px - 1199px (adjusted spacing and font sizes)
- **Mobile**: Below 768px (single column, hamburger menu)
- **Small Mobile**: Below 480px (optimized for small screens)

## 🎨 Color Scheme

```css
Primary Color: #1e3c72 (Dark Navy Blue)
Secondary Color: #2a5298 (Medium Blue)
Accent Color: #0066cc (Bright Blue)
Accent Light: #4da3ff (Light Blue)
Light Background: #f0f4f8
Text Color: #1a1a2e
Dark Mode: Supported via data-theme attribute
```

## 📝 Customization Tips

### Change Color Scheme
Edit the CSS variables in `styles.css`:
```css
:root {
    --primary-color: #1e3c72;
    --secondary-color: #2a5298;
    --accent-color: #0066cc;
    /* ... other colors ... */
}
```

### Dark Mode Colors
```css
[data-theme="dark"] {
    --primary-color: #0f1b3d;
    --secondary-color: #1a2d5e;
    --accent-color: #4da3ff;
    --light-bg: #111827;
    --dark-text: #e5e7eb;
    --light-text: #9ca3af;
    --white: #1f2937;
}
```

### Change Font
The website uses Poppins from Google Fonts. To change:
1. Edit the `@import` statement in `styles.css`
2. Or add a different font link in `index.html` `<head>`

### Modify Spacing
Adjust padding and margins in `styles.css` under each section class.

### Add/Remove Animations
All animated elements use the `.animate-on-scroll` class. Remove this class from any element to disable its scroll animation.

## 🐛 Troubleshooting

### Hamburger Menu Not Working
- Ensure `script.js` is properly linked in `index.html`
- Check browser console for JavaScript errors

### Theme Toggle Not Working
- Ensure localStorage is enabled in your browser
- Check console for errors related to `localStorage`

### Scroll Progress Not Showing
- Ensure `scrollProgress` element exists in HTML
- Check that `script.js` is loaded after DOM

### Images Not Showing
- Verify image file paths are correct
- Ensure images are in the same folder or provide full paths
- Check file permissions

### Styling Issues
- Clear browser cache (Ctrl+Shift+Delete)
- Try a different browser
- Check CSS file is properly linked

### Form Not Submitting
- Check browser console for errors
- Verify all form fields are filled
- Ensure email format is valid

## 📚 Resources

- [HTML5 Documentation](https://developer.mozilla.org/en-US/docs/Web/HTML/)
- [CSS3 Guide](https://developer.mozilla.org/en-US/docs/Web/CSS/)
- [JavaScript Tutorial](https://developer.mozilla.org/en-US/docs/Web/JavaScript/)
- [Font Awesome Icons](https://fontawesome.com/)
- [Google Fonts](https://fonts.google.com/)
- [Poppins Font](https://fonts.google.com/specimen/Poppins)

## 🚀 Deployment

### Deploy to GitHub Pages
1. Create a GitHub repository
2. Push your project files
3. Enable GitHub Pages in repository settings
4. Your site will be live at `https://yourusername.github.io/repository-name`

### Deploy to Other Platforms
- Netlify
- Vercel
- Heroku
- AWS S3

## 📧 Contact Form Integration

Currently, the form displays a success message but doesn't send emails. To enable email functionality:

1. **Using Formspree**:
   - Go to [Formspree.io](https://formspree.io/)
   - Create an account and new form
   - Replace form action with your Formspree endpoint

2. **Using Email.js**:
   - Install Email.js library
   - Configure with your email service
   - Update `script.js` with Email.js code

3. **Using Backend Service**:
   - Set up a server (Node.js, Python, etc.)
   - Create endpoint to handle form submissions
   - Update form action to your backend URL

## 🎓 Learning Resources

This portfolio template is great for learning:
- Semantic HTML structure
- Modern CSS Grid and Flexbox
- CSS Custom Properties (Variables)
- Responsive design techniques
- Vanilla JavaScript interactivity
- Animation and transition techniques
- IntersectionObserver API
- CSS Backdrop Filter / Glassmorphism
- localStorage for theme persistence

## 📄 License

Feel free to use this template for your personal portfolio.

## 🎉 Next Steps

1. ✅ Open `index.html` in your browser
2. ✅ Test responsiveness on different devices
3. ✅ Customize content with your information
4. ✅ Replace placeholder images
5. ✅ Update social media links
6. ✅ Add your CV file
7. ✅ Try the dark mode toggle
8. ✅ Deploy to your preferred hosting platform

---

**Happy building! Your portfolio is ready to showcase your skills. Good luck! 🚀**