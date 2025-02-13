# Texas Web Design Landing Page - Maintenance Guide

This guide will help you maintain and customize the Texas Web Design landing page. Whether you're new to web development or need a quick reference, follow these instructions to make common updates safely and effectively.

## Table of Contents
- [Updating Text and Styling](#updating-text-and-styling)
- [Managing Links](#managing-links)
- [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
- [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains the main navigation and logo. To update:

1. **Company Name/Logo**
```html
<!-- Find this section near the top -->
<a href="/" class="text-2xl font-bold bg-gradient-to-r from-blue-600 to-indigo-600 bg-clip-text text-transparent">
    Texas Web Design  <!-- Change this text -->
</a>
```

2. **Navigation Menu Items**
```html
<div class="hidden md:flex space-x-8">
    <a href="#features">Features</a>  <!-- Change menu text here -->
    <a href="#faq">FAQ</a>
    <a href="#contact">Contact</a>
</div>
```

### Hero Section
Located at the top of the page:

```html
<h1 class="text-5xl md:text-6xl font-bold leading-tight mb-8">
    Best Websites In Texas  <!-- Main headline -->
</h1>
<p class="text-xl text-gray-600 mb-12">
    Creating stunning, high-performance websites...  <!-- Subheadline -->
</p>
```

### Features Section
To modify feature cards:

```html
<div class="p-8 rounded-2xl bg-white border border-gray-100">
    <h3 class="text-xl font-bold mb-4">Free Hosting</h3>  <!-- Feature title -->
    <p class="text-gray-600">Premium hosting included...</p>  <!-- Feature description -->
</div>
```

### Understanding Tailwind Classes

Common classes explained:
- `text-xl`, `text-2xl`: Text size
- `mb-4`, `mt-8`: Margin spacing
- `py-24`: Vertical padding
- `bg-white`: Background color
- `text-gray-600`: Text color

To modify styling:
1. Find the element you want to change
2. Locate its class attribute
3. Add or modify Tailwind classes
4. Test on different screen sizes

## Managing Links

### Navigation Links
Current navigation links are:

```html
<div class="hidden md:flex space-x-8">
    <a href="#features">Features</a>
    <a href="#faq">FAQ</a>
    <a href="#contact">Contact</a>
    <a href="https://twd.com">Get Started</a>  <!-- External link to update -->
</div>
```

To update:
1. Locate the `href` attribute
2. For internal links (same page):
   - Use `#section-id` format
   - Ensure the target section has matching ID
3. For external links:
   - Replace `https://twd.com` with your actual URL
   - Include `https://` prefix

### Call-to-Action Buttons
Located in hero and CTA sections:

```html
<a href="https://twd.com" class="px-8 py-4 bg-blue-600 text-white rounded-full">
    Start Your Project  <!-- Button text -->
</a>
```

## Adding Privacy and Terms Pages

### Footer Link Updates
Locate the footer section:

```html
<div>
    <h4 class="text-lg font-semibold text-white mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="#" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="#" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

To link privacy and terms pages:
1. Create `privacy.html` and `terms.html` in your project folder
2. Update the href attributes:
```html
<li><a href="privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

## Troubleshooting

Common issues and solutions:

1. **Broken Internal Links**
   - Verify section IDs match href values
   - Check for typos in IDs
   - Ensure sections have unique IDs

2. **Styling Issues**
   - Check for missing or mistyped Tailwind classes
   - Verify class names are spelled correctly
   - Test responsiveness using browser developer tools

3. **External Links**
   - Confirm URLs include `https://` or `http://`
   - Test links in different browsers
   - Verify domain names are spelled correctly

Remember to:
- Always backup files before making changes
- Test all changes in multiple browsers
- Verify mobile responsiveness
- Check spelling and grammar in content updates

Need more help? Contact your web development team or refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs).