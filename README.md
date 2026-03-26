# PetComfort Hub - Static HTML Website

## Overview
This is the static HTML, CSS, and JavaScript version of the PetComfort Hub pet care website, converted from a React application.

## File Structure

```
/public/
├── index.html              # Home page
├── about.html              # About Us page
├── services.html           # Services page
├── contact.html            # Contact page with Google Maps
├── privacy-policy.html     # Privacy Policy (legal page)
├── terms-conditions.html   # Terms & Conditions (legal page)
├── disclaimer.html         # Disclaimer (legal page)
├── cookie-policy.html      # Cookie Policy (legal page)
├── css/
│   └── styles.css          # Custom CSS styles
└── js/
    └── main.js             # JavaScript for interactivity
```

## Features

### Main Pages
1. **Home (index.html)**
   - Hero section with CTA buttons
   - About preview section
   - Services overview (6 services)
   - Why Choose Us section
   - Pricing plans
   - Testimonials
   - Call-to-action section

2. **About (about.html)**
   - Company story
   - Mission statement
   - Core values (Compassion, Trust, Professional Care, Pet Happiness)
   - Team photos
   - Statistics section

3. **Services (services.html)**
   - Detailed service descriptions for all 6 services:
     - Dog Walking
     - Pet Sitting
     - Pet Grooming
     - Pet Boarding
     - Pet Wellness Check
     - Puppy & Kitten Care
   - Pricing information for each service
   - Benefits and features

4. **Contact (contact.html)**
   - Contact form with validation
   - Contact information cards
   - Business hours
   - Embedded Google Maps

### Legal Pages
- Privacy Policy
- Terms & Conditions
- Disclaimer
- Cookie Policy

## Interactive Components

### Header Navigation
- Responsive navigation menu
- Mobile hamburger menu
- Active page highlighting
- "Book Pet Care" CTA button

### Contact Form Popup
- Accessible from any page via buttons
- Form validation
- Privacy policy consent checkbox
- Toast notifications for success/error
- Modal overlay backdrop

### Cookie Banner
- Appears on first visit
- Accept/Reject options
- Stores consent in localStorage
- Link to Cookie Policy page

### Forms
- Contact form on Contact page
- Popup booking form
- Both include:
  - Required field validation
  - Policy consent checkbox
  - Service selection dropdown
  - Toast notifications

## Technologies Used

- **HTML5** - Semantic markup
- **Tailwind CSS** - Styling via CDN
- **Vanilla JavaScript** - All interactivity
- **Lucide Icons** - Icon library via CDN
- **Google Maps** - Embedded map on contact page

## JavaScript Functionality

The `main.js` file handles:
- Mobile menu toggle
- Cookie banner show/hide/consent
- Contact popup open/close
- Form submissions
- Toast notifications
- Active navigation highlighting
- Current year display in footer

## Responsive Design

All pages are fully responsive with breakpoints:
- Mobile: < 768px
- Tablet: 768px - 1024px
- Desktop: > 1024px

## Browser Support

Compatible with all modern browsers:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Opera (latest)

## Local Storage Usage

The website uses localStorage for:
- Cookie consent (key: 'cookieConsent')

## Images

All images are loaded from Unsplash via direct URLs. The images used:
- Pet care professionals
- Dogs, cats, puppies, kittens
- Grooming services
- Pet owners with pets

## Forms

### Contact Form Fields:
- Full Name (required)
- Email (required)
- Phone (required)
- Service selection (required)
- Message (optional)
- Privacy policy consent checkbox (required)

### Popup Form Fields:
Same as contact form

## Color Scheme

- Primary Blue: #2563EB (blue-600)
- Primary Green: #10B981 (green-600)
- Background: Gradients from blue-50 to green-50
- Text: Gray-900, Gray-700, Gray-600
- Accent: Blue-400 for links and icons

## Contact Information

- **Address**: 10222 Desert Sands St Ste 204, San Antonio, TX 78116, United States
- **Phone**: +1-925-306-9647
- **Email**: help@petcomforthub.site

## Running the Website

1. Simply open any HTML file in a web browser
2. All pages are standalone and don't require a build process
3. No server required - works with file:// protocol
4. For best experience, serve via a local web server:
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Node.js http-server
   npx http-server
   ```

## Notes

- All external dependencies (Tailwind CSS, Lucide Icons) are loaded via CDN
- Forms use simulated submission (show toast notification but don't actually submit)
- Google Maps embed uses a placeholder URL - replace with actual coordinates
- No backend integration - this is a frontend-only static website
- Cookie consent only stores preference, doesn't implement actual cookie functionality

## Customization

### To Update Images:
Replace Unsplash URLs in HTML files with your own image URLs

### To Update Contact Info:
Search and replace in all HTML files:
- Phone number: +1-925-306-9647
- Email: help@petcomforthub.site
- Address: 10222 Desert Sands St Ste 204, San Antonio, TX 78116

### To Update Styling:
- Edit `/public/css/styles.css` for custom styles
- Modify Tailwind classes directly in HTML

### To Update Functionality:
- Edit `/public/js/main.js` for JavaScript behavior

## Accessibility Features

- Semantic HTML5 elements
- ARIA labels on interactive elements
- Keyboard navigation support
- Focus visible styles
- Alt text on all images
- Proper heading hierarchy

## Performance

- Minimal external dependencies
- Lazy loading for embedded maps
- Optimized image loading from CDN
- No JavaScript frameworks - pure vanilla JS

## License

All rights reserved © 2026 PetComfort Hub
