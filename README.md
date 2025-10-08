# NOMA - Network of Moroccans in America

A beautiful static website for the Network of Moroccans in America, featuring Moroccan-inspired design elements and modern web practices.

## 🇲🇦 About

NOMA is a community organization dedicated to connecting Moroccan-Americans across the United States. This website serves as the digital hub for the organization, providing information about services, events, and ways to get involved.

## 🎨 Design Features

- **Moroccan Color Palette**: Traditional Moroccan colors including red (#C1272D), green (#006233), and gold (#D4AF37)
- **Modern Layout**: Clean, responsive design that works on all devices
- **Smooth Animations**: Scroll-triggered animations and smooth transitions
- **Interactive Elements**: Mobile-friendly navigation, contact form, and interactive map

## 📋 Sections

1. **Home** - Hero section with call-to-action
2. **About Us** - Organization information and community statistics
3. **Our Purpose** - Six key areas of focus
4. **Get Help** - Services and resources available
5. **Location** - Interactive map showing Chicago headquarters
6. **Contact** - Contact form and information

## 🚀 Getting Started

This is a static website requiring no build process. Simply open `index.html` in a web browser.

### Option 1: Direct File Access
```bash
# Navigate to the project directory
cd /Users/mt/Workspace/NOMA

# Open in your default browser (macOS)
open index.html

# Or on Linux
xdg-open index.html

# Or on Windows
start index.html
```

### Option 2: Local Server (Recommended)
Using Python:
```bash
# Python 3
python3 -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

Using Node.js:
```bash
npx http-server -p 8000
```

Then visit: `http://localhost:8000`

## 📁 File Structure

```
NOMA/
├── index.html          # Main HTML file
├── styles.css          # Moroccan-inspired styling
├── script.js           # Interactive functionality
└── README.md           # This file
```

## 🎯 Customization

### Update Contact Information
Edit the contact details in `index.html` around line 220 (location section) and line 250 (contact section).

### Update Map Location
Replace the Google Maps embed URL in `index.html` (line 237) with your actual headquarters location.

### Change Colors
All colors are defined as CSS variables in `styles.css` at the top:
```css
:root {
    --primary-red: #C1272D;
    --secondary-green: #006233;
    --gold: #D4AF37;
    /* ... */
}
```

### Connect Contact Form
The contact form currently shows an alert on submission. To connect it to a backend:
1. Edit the form handling in `script.js` (around line 50)
2. Integrate with a service like Formspree, EmailJS, or your own backend

## 🌐 Deployment

This static site can be deployed to:
- **GitHub Pages**: Free hosting for static sites
- **Netlify**: Drag and drop deployment
- **Vercel**: Easy static site hosting
- **AWS S3**: Scalable hosting solution
- **Traditional web hosting**: Upload via FTP

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 🤝 Contributing

This is a community project. To contribute:
1. Fork the repository
2. Make your changes
3. Test thoroughly on multiple devices
4. Submit a pull request

## 📞 Support

For questions or support, contact:
- Email: info@nomausa.org
- Phone: (312) 555-NOMA

## 📄 License

© 2025 NOMA - Network of Moroccans in America. All rights reserved.

---

Built with ❤️ for the Moroccan-American community

