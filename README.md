# Photography Portfolio & Booking Website

A professional, modern website for photographers to showcase their work and allow clients to book appointments.

## Features

✨ **Beautiful Design**
- Responsive layout that works on mobile, tablet, and desktop
- Modern, professional aesthetic
- Smooth animations and transitions

📸 **Photo Gallery**
- Display your photography portfolio
- Grid layout with hover effects
- Easy to customize with your own images

📅 **Booking System**
- Client booking form with date/time selection
- Service type selection with pricing
- Session duration options
- Form validation and confirmation message

💼 **Service Management**
- Display multiple photography services
- Show pricing for each service
- Professional service cards

📞 **Contact Information**
- Easy-to-find contact details
- Email and phone links
- Location information

## Getting Started

### 1. Clone or Download Files
All files are ready to use:
- `index.html` - Main website structure
- `styles.css` - Styling and responsive design
- `script.js` - Interactivity and booking functionality

### 2. Customize Your Information

Open `index.html` and update:

**Navbar/Brand Name:**
```html
<h1>📸 Your Photo Studio</h1>
```

**Contact Information (near the bottom):**
```html
<p><a href="mailto:contact@yourphoto.com">contact@yourphoto.com</a></p>
<p><a href="tel:+1234567890">(123) 456-7890</a></p>
<p>Your City, State</p>
```

**Pricing** (in the Services section):
Modify the prices in:
```html
<p class="price">$150/hour</p>
```

### 3. Add Your Photos

Replace the image URLs in the gallery section with your own photos:

```html
<img src="YOUR_IMAGE_URL" alt="Description">
```

You can host images on:
- **Free options:** Unsplash, Pexels, Pixabay
- **Paid options:** AWS S3, Google Cloud Storage, Cloudinary
- **Free with account:** Imgur, GitHub (as raw files)

### 4. Deploy Your Website

**Free Hosting Options:**

**GitHub Pages (Recommended - Free & Easy)**
1. Push your files to your GitHub repository
2. Go to Settings → Pages
3. Set source to "main" branch
4. Your site will be live at `https://dagerk029-afk.github.io/buddy/`

**Other Free Options:**
- **Netlify** - netlify.com (drag & drop deployment)
- **Vercel** - vercel.com
- **GitHub Pages** - github.com/settings/pages
- **Firebase Hosting** - firebase.google.com
- **Heroku** - heroku.com

## Booking System

### How It Works

1. Clients fill out the booking form with their details
2. They select the service type, date, time, and duration
3. Form validates all required fields
4. Confirmation message displays after submission
5. Form data is logged to browser console

### Connecting to a Backend (Optional)

To actually receive booking emails, you'll need a backend service. Uncomment and modify the fetch code in `script.js`:

```javascript
fetch('/api/bookings', {
    method: 'POST',
    headers: {
        'Content-Type': 'application/json',
    },
    body: JSON.stringify(formData)
})
```

**Backend Services (Free/Affordable):**
- **Formspree** - formspree.io (free form submissions)
- **EmailJS** - emailjs.com (send emails from JavaScript)
- **Firebase** - firebase.google.com (database + functions)
- **Supabase** - supabase.com (PostgreSQL database)

## Customization

### Colors
Edit the CSS variables in `styles.css`:
```css
:root {
    --primary-color: #2c3e50;      /* Main color */
    --accent-color: #e74c3c;        /* Highlight color */
    --light-bg: #ecf0f1;            /* Background */
}
```

### Fonts
Change fonts in the `body` selector:
```css
font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
```

### Services
Add or modify services in the Services section of `index.html`:
```html
<div class="service-card">
    <div class="service-icon">📸</div>
    <h3>Your Service</h3>
    <p>Description</p>
    <p class="price">$Price</p>
</div>
```

## Mobile Optimization

The website is fully responsive with breakpoints at 768px for mobile devices. Test on different devices using:
- Chrome DevTools (F12)
- Safari Developer Tools
- Mobile browser simulators

## Performance Tips

1. **Optimize Images** - Compress images before uploading
   - Use tools like TinyPNG or Squoosh
   - Target ~100-200KB per image

2. **Lazy Loading** - Add to images for faster loading:
   ```html
   <img src="image.jpg" loading="lazy" alt="Description">
   ```

3. **CDN for Images** - Use Cloudinary or Imgix for automatic optimization

## SEO Optimization

To improve search engine visibility:

1. Update `<title>` in HTML with your business name
2. Add meta description:
   ```html
   <meta name="description" content="Professional photography services and booking">
   ```

3. Add structured data (JSON-LD) for better search results
4. Use descriptive alt text for all images

## Browser Support

Works on:
- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Mobile browsers (iOS Safari, Chrome Mobile)

## Next Steps

1. ✅ Customize with your information
2. ✅ Add your photos to the gallery
3. ✅ Deploy to GitHub Pages or hosting platform
4. ✅ (Optional) Set up backend for real booking emails
5. ✅ Test on mobile devices
6. ✅ Share your website link with clients!

## Support & Updates

For questions or improvements:
- Check the code comments
- Review HTML structure in `index.html`
- Customize CSS in `styles.css`
- Modify functionality in `script.js`

## License

Feel free to use and modify this website for your photography business!

---

**Ready to get started?** Open `index.html` in a browser to preview your new photography website! 📸
