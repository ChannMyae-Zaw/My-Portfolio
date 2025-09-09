# Geometric Portfolio Website

A modern, responsive portfolio website with geometric design elements and smooth animations.

## Features

- 🎨 **Geometric Design**: Clean, modern aesthetic with geometric shapes and animations
- 📱 **Responsive**: Fully responsive design that works on all devices
- ✉️ **Contact Form**: Functional contact form with EmailJS integration
- 🎭 **Animations**: Smooth scroll animations and interactive elements
- ⚡ **Performance**: Optimized for fast loading and smooth performance

## Sections

1. **Landing Page**: Hero section with animated geometric background
2. **About Page**: Introduction with skills showcase
3. **Projects Page**: Portfolio projects with hover effects
4. **Contact Page**: Contact form with email functionality

## Setup Instructions

### 1. Clone or Download
Download the project files to your local machine.

### 2. Install Dependencies
```bash
npm install
```

### 3. Configure EmailJS (for contact form)

1. **Sign up at [EmailJS](https://www.emailjs.com/)**
2. **Create an Email Service**:
   - Connect your email provider (Gmail, Outlook, etc.)
   - Note down your Service ID

3. **Create an Email Template**:
   - Use these template variables:
     - `{{from_name}}` - Sender's name
     - `{{from_email}}` - Sender's email
     - `{{subject}}` - Email subject
     - `{{message}}` - Email message
   - Note down your Template ID

4. **Get your User ID** from the EmailJS dashboard

5. **Update the configuration** in `js/main.js`:
   ```javascript
   const EMAILJS_SERVICE_ID = 'your_actual_service_id';
   const EMAILJS_TEMPLATE_ID = 'your_actual_template_id';
   const EMAILJS_USER_ID = 'your_actual_user_id';
   ```

### 4. Customize Content

1. **Personal Information**:
   - Update your name in the hero section
   - Add your photo to the about section
   - Update contact details

2. **Projects**:
   - Replace placeholder projects with your actual work
   - Add project images and links
   - Update project descriptions and technologies

3. **Skills**:
   - Modify the skills section to reflect your expertise
   - Update skill descriptions

### 5. Run the Website

#### Option 1: Using Live Server (Recommended)
```bash
npm start
```
This will start a local server at `http://localhost:3000`

#### Option 2: Using any HTTP Server
You can use any static file server or simply open `index.html` in your browser.

## Customization

### Colors
Update the CSS custom properties in `styles/main.css`:
```css
:root {
    --primary-color: #6366f1;    /* Main brand color */
    --secondary-color: #f59e0b;  /* Secondary accent */
    --accent-color: #ec4899;     /* Accent color */
    /* ... other colors */
}
```

### Typography
The website uses Inter font from Google Fonts. You can change it by updating the font import in `index.html` and the CSS variable:
```css
:root {
    --font-family: 'Your-Font', sans-serif;
}
```

### Geometric Shapes
Modify the geometric elements by adjusting the CSS animations and clip-path properties in the stylesheet.

## File Structure

```
MyPortfolio/
├── index.html          # Main HTML file
├── styles/
│   └── main.css        # All CSS styles
├── js/
│   └── main.js         # JavaScript functionality
├── package.json        # Dependencies and scripts
└── README.md          # This file
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Performance Tips

1. **Optimize Images**: Compress any images you add
2. **Minimize JavaScript**: The current JS is already optimized
3. **Use WebP**: Consider WebP format for better compression
4. **CDN**: Use a CDN for production deployment

## Deployment

### GitHub Pages
1. Push your code to a GitHub repository
2. Go to Settings > Pages
3. Select source branch (usually `main`)
4. Your site will be available at `https://username.github.io/repository-name`

### Netlify
1. Connect your GitHub repository to Netlify
2. Set build command: (leave empty for static site)
3. Set publish directory: (root directory)
4. Deploy!

### Vercel
1. Connect your GitHub repository to Vercel
2. Deploy with default settings

## License

MIT License - feel free to use this template for your own portfolio!

## Support

If you encounter any issues or need help customizing the template, feel free to:
1. Check the browser console for any error messages
2. Ensure all file paths are correct
3. Verify EmailJS configuration if contact form isn't working

---

**Happy coding! 🚀**

