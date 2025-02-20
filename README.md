# Just Spoiled Landing Page - Maintenance Guide

This guide will help you maintain and customize the Just Spoiled landing page. Whether you're new to web development or need a quick reference, you'll find step-by-step instructions for common updates.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Fixing and Managing Links](#fixing-and-managing-links)
3. [Adding Policy Pages](#adding-policy-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains your brand name and navigation menu. To update:

```html
<!-- Find this section at the top of the page -->
<div class="text-2xl font-bold">Just Spoiled</div>
```

To change the brand name, simply replace "Just Spoiled" with your desired text. The classes mean:
- `text-2xl`: Large text size
- `font-bold`: Bold weight text

### Hero Section
The main banner section contains three key elements:

```html
<div class="text-center text-white max-w-4xl">
    <h1 class="text-4xl md:text-6xl font-bold mb-6">Just Spoiled</h1>
    <p class="text-xl md:text-2xl mb-8">Convenience is Luxury</p>
    <a href="https://JonPaul.Hair" class="inline-block bg-white text-black px-8 py-4 rounded-full">
        Shop Now
    </a>
</div>
```

To modify:
1. Change the headline by replacing text in the `<h1>` tag
2. Update the tagline in the `<p>` tag
3. Modify the button text within the `<a>` tag

### Features Section
Each feature card follows this structure:

```html
<div class="bg-white p-8 rounded-xl shadow-lg hover:shadow-xl transition duration-300 transform hover:scale-105">
    <div class="text-4xl mb-4"><i class="fas fa-bolt text-blue-600"></i></div>
    <h3 class="text-xl font-bold mb-4">Fast</h3>
    <p class="text-gray-600">Lightning-quick service at your fingertips</p>
</div>
```

To update:
1. Change the icon by replacing `fa-bolt` with any [Font Awesome icon](https://fontawesome.com/icons)
2. Modify the title in the `<h3>` tag
3. Update the description in the `<p>` tag

## Fixing and Managing Links

### Navigation Menu Links
Located in the header:

```html
<div class="hidden md:flex space-x-8">
    <a href="#" class="hover:text-gray-600 transition-colors duration-300">Home</a>
    <a href="#" class="hover:text-gray-600 transition-colors duration-300">Shop</a>
    <a href="#" class="hover:text-gray-600 transition-colors duration-300">About</a>
    <a href="#" class="hover:text-gray-600 transition-colors duration-300">Contact</a>
</div>
```

To update links:
1. Replace `#` with your actual page URLs
2. Example: `<a href="about.html">About</a>`
3. For external links, use full URLs: `<a href="https://example.com">Example</a>`

### Call-to-Action (CTA) Links
Found throughout the page:

```html
<a href="https://JonPaul.Hair" class="inline-block bg-white text-black px-8 py-4 rounded-full">
    Shop Now
</a>
```

Replace `https://JonPaul.Hair` with your desired destination URL.

## Adding Policy Pages

### Footer Policy Links
Located at the bottom of the page:

```html
<div>
    <h4 class="text-lg font-semibold mb-4">Policies</h4>
    <ul class="space-y-2 text-gray-400">
        <li><a href="#" class="hover:text-white transition duration-300">Privacy Policy</a></li>
        <li><a href="#" class="hover:text-white transition duration-300">Terms of Service</a></li>
        <li><a href="#" class="hover:text-white transition duration-300">Shipping Policy</a></li>
    </ul>
</div>
```

To link policy pages:
1. Create your policy pages (e.g., `privacy.html`, `terms.html`)
2. Update the href attributes:
```html
<li><a href="privacy.html" class="hover:text-white transition duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="hover:text-white transition duration-300">Terms of Service</a></li>
```

## Troubleshooting

### Common Issues

1. **Broken Images**
   - Check that image URLs are correct
   - Ensure images exist at the specified path
   - Verify image file extensions match exactly

2. **Responsive Design Issues**
   - Don't remove `md:` prefixes from classes
   - Keep the viewport meta tag in the header
   - Test on multiple screen sizes

3. **Font Awesome Icons Not Showing**
   - Verify the Font Awesome CDN link is present in the header
   - Check icon class names against the [Font Awesome website](https://fontawesome.com)

### Need Help?
If you encounter issues:
1. Check the browser's developer tools (F12) for errors
2. Verify all CDN links are accessible
3. Ensure all HTML tags are properly closed
4. Test the page in multiple browsers

Remember to always backup your files before making changes!