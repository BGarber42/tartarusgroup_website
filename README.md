# Tartarus Group Website

A modern, professional static website for Tartarus Group, showcasing full-stack cloud software development services with AWS infrastructure, CI/CD, and modern web solutions.

## 🚀 Features

- **Modern Design**: Clean, professional layout with excellent UX
- **Responsive**: Mobile-first design that works on all devices
- **Performance Optimized**: Fast loading for GitHub Pages hosting
- **SEO Friendly**: Proper meta tags and semantic HTML structure
- **Interactive**: Smooth animations and modern interactions
- **Accessible**: WCAG compliant with proper focus management

## 🛠️ Tech Stack

- **HTML5**: Semantic markup structure
- **CSS3**: Modern styling with CSS Grid and Flexbox
- **Vanilla JavaScript**: No frameworks for optimal performance
- **Google Fonts**: Inter font family for modern typography
- **GitHub Pages**: Static hosting platform

## 📁 Project Structure

```
TartarusGroup/
├── index.html              # Main HTML file
├── styles/
│   └── main.css           # Main stylesheet
├── scripts/
│   └── main.js            # JavaScript functionality
├── assets/                # Images and other assets
└── README.md              # This file
```

## 🚀 Getting Started

### Local Development

1. **Clone the repository** (if using Git):
   ```bash
   git clone <your-repo-url>
   cd TartarusGroup
   ```

2. **Open in your browser**:
   - Simply open `index.html` in your web browser
   - Or use a local server for development:
     ```bash
     # Using Python 3
     python -m http.server 8000
     
     # Using Node.js (if you have npx)
     npx serve .
     
     # Using PHP
     php -S localhost:8000
     ```

3. **View the website**:
   - Navigate to `http://localhost:8000` (if using a server)
   - Or open `index.html` directly in your browser

### Customization

#### Colors and Branding
Edit the CSS custom properties in `styles/main.css`:
```css
:root {
    --primary-color: #2563eb;    /* Your brand color */
    --primary-dark: #1d4ed8;     /* Darker shade */
    --accent-color: #f59e0b;     /* Accent color */
    /* ... other variables */
}
```

#### Content Updates
- **Company Information**: Update the content in `index.html`
- **Contact Information**: Change email addresses and contact details
- **Services**: Modify the services section to match your offerings
- **About Section**: Update company description and tech stack

#### Images and Assets
- Add your logo to `assets/` directory
- Update favicon: `assets/favicon.ico`
- Replace placeholder images with your own

## 🌐 Deployment

### GitHub Pages Deployment

1. **Create a GitHub repository**:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/yourusername/tartarusgroup.git
   git push -u origin main
   ```

2. **Enable GitHub Pages**:
   - Go to your repository settings
   - Scroll down to "GitHub Pages" section
   - Select "Deploy from a branch"
   - Choose "main" branch and "/ (root)" folder
   - Click "Save"

3. **Custom Domain Setup** (Optional):
   - In repository settings, under "GitHub Pages"
   - Add your custom domain (e.g., `tartarusgroup.com`)
   - Create a `CNAME` file in the root with your domain
   - Configure DNS with your domain provider

### Cloudflare Setup

1. **Add your domain to Cloudflare**:
   - Sign up/login to Cloudflare
   - Add your domain
   - Update nameservers at your domain registrar

2. **Configure DNS**:
   - Add a CNAME record pointing to `yourusername.github.io`
   - Enable Cloudflare proxy (orange cloud)

3. **SSL/TLS Settings**:
   - Set SSL/TLS encryption mode to "Full"
   - Enable "Always Use HTTPS"

## 📧 Contact Form

The contact form is currently set up for demonstration. To make it functional:

### Option 1: Formspree (Recommended)
1. Sign up at [formspree.io](https://formspree.io)
2. Create a new form
3. Update the form action in `index.html`:
   ```html
   <form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```

### Option 2: Netlify Forms
1. Deploy to Netlify
2. Add `data-netlify="true"` to the form
3. Netlify will automatically handle form submissions

### Option 3: Custom Backend
Replace the form handling in `scripts/main.js` with your own API endpoint.

## 🔧 Performance Optimization

The website is already optimized for performance:

- **Minimal Dependencies**: No heavy frameworks
- **Optimized Images**: Use WebP format when possible
- **Efficient CSS**: Minimal, focused stylesheets
- **Fast Loading**: Optimized for GitHub Pages

### Additional Optimizations

1. **Image Optimization**:
   ```bash
   # Install and use tools like:
   npm install -g imagemin-cli
   imagemin assets/* --out-dir=assets/optimized
   ```

2. **CSS Minification**:
   ```bash
   # Use tools like:
   npm install -g clean-css-cli
   cleancss -o styles/main.min.css styles/main.css
   ```

3. **JavaScript Minification**:
   ```bash
   # Use tools like:
   npm install -g uglify-js
   uglifyjs scripts/main.js -o scripts/main.min.js
   ```

## 🎨 Customization Guide

### Adding New Sections

1. **HTML Structure**:
   ```html
   <section id="new-section" class="new-section">
       <div class="container">
           <h2 class="section-title">New Section</h2>
           <!-- Your content here -->
       </div>
   </section>
   ```

2. **CSS Styling**:
   ```css
   .new-section {
       padding: 80px 0;
       background-color: var(--white);
   }
   ```

3. **Navigation Link**:
   ```html
   <li class="nav-item">
       <a href="#new-section" class="nav-link">New Section</a>
   </li>
   ```

### Modifying Animations

Edit the CSS animations in `styles/main.css`:
```css
@keyframes fadeInUp {
    from {
        opacity: 0;
        transform: translateY(30px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}
```

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 📞 Support

For questions or support:
- Email: hello@tartarusgroup.com
- GitHub Issues: [Create an issue](https://github.com/yourusername/tartarusgroup/issues)

---

**Built with ❤️ for Tartarus Group** 