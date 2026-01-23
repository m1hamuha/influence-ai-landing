# AGENTS.md - Development Guidelines for AI Influencer Landing Page

## Overview
This is a static landing page for an AI influencer course built with vanilla HTML, CSS, and JavaScript. The project uses modern web standards with no build tools or frameworks.

## Build/Lint/Test Commands

### Build Commands
Since this is a static site with no build system:
- **Serve locally**: Use any static file server (e.g., `python -m http.server` or VS Code Live Server)
- **Deploy**: Upload files directly to web server or static hosting service

### Linting & Code Quality
No linter is currently configured. For consistency, use:
```bash
# ESLint (if added later)
npx eslint app.js

# CSS linting
npx stylelint styles.css

# HTML validation
npx html-validate index.html
```

### Testing Commands
No test framework is configured. For basic testing:
```bash
# Manual testing - open in browser
# Test functionality: timer, carousel, language switching, videos
```

### Running a Single Test
Since no automated tests exist:
- Test individual features manually by opening the page in a browser
- Use browser dev tools to verify JavaScript functionality
- Check responsive design with browser dev tools

## Code Style Guidelines

### JavaScript Style
- **Module Pattern**: Use Immediately Invoked Function Expressions (IIFE) for encapsulation
- **Modern JavaScript**: ES6+ features (arrow functions, template literals, destructuring)
- **DOM Manipulation**: Use modern APIs (querySelector, addEventListener)
- **Error Handling**: Basic try/catch for async operations, graceful degradation for unsupported features
- **Performance**: Use `requestAnimationFrame` for animations, efficient DOM queries
- **Naming**: camelCase for variables/functions, PascalCase for constructors
- **Comments**: No inline comments unless absolutely necessary - code should be self-documenting
- **Imports**: No module imports (vanilla JS) - all code in single file

### HTML Style
- **Semantic HTML**: Use proper semantic elements (section, nav, header, etc.)
- **Accessibility**: Include ARIA labels, alt text for images, proper heading hierarchy
- **Internationalization**: Use `data-i18n` attributes for translatable content
- **Structure**: BEM-like CSS class naming (block__element--modifier)
- **Performance**: Lazy load videos with proper attributes (autoplay, muted, playsinline)

### CSS Style
- **CSS Custom Properties**: Use CSS variables for colors, spacing, and reusable values
- **Responsive Design**: Use `clamp()`, `min()`, `max()` for fluid typography and spacing
- **Glassmorphism**: Consistent use of backdrop-filter, rgba colors, and subtle shadows
- **Animations**: Use CSS transforms and opacity for smooth animations
- **Organization**: Group related properties, use logical property ordering
- **Performance**: Use `transform` and `opacity` for animations (GPU-accelerated)

### General Principles
- **No Comments**: Avoid comments unless explaining complex business logic
- **Consistent Formatting**: 2-space indentation, single quotes for JavaScript
- **Cross-browser Compatibility**: Support modern browsers (Chrome, Firefox, Safari, Edge)
- **Mobile-first**: Responsive design with touch-friendly interactions
- **Performance**: Optimize images, lazy load videos, minimize DOM manipulation

### File Organization
- `index.html`: Main landing page
- `app.js`: All JavaScript functionality (single file)
- `styles.css`: All CSS styles (single file)
- `*.html`: Legal pages (privacy, consent, offer)
- `assets/`: Images, videos, and media files

### Security Best Practices
- **Input Validation**: Sanitize any user inputs (though minimal in this static site)
- **Content Security Policy**: Consider implementing CSP headers for production
- **HTTPS**: Always serve over HTTPS in production
- **No Secrets**: Never commit API keys or sensitive data

### Browser Support
- Modern browsers (Chrome 90+, Firefox 88+, Safari 14+, Edge 90+)
- Mobile browsers (iOS Safari, Chrome Mobile)
- Graceful degradation for older browsers

## Cursor Rules & Copilot Instructions
No Cursor rules (.cursor/rules/ or .cursorrules) or Copilot rules (.github/copilot-instructions.md) are currently configured for this repository.

## Development Workflow
1. Make changes to HTML/CSS/JS files
2. Test in browser (multiple devices/screen sizes)
3. Verify functionality: language switching, carousel, timer, videos
4. Check responsive design
5. Deploy by uploading files to hosting service

## Dependencies
- **None**: Pure vanilla JavaScript, HTML, CSS
- **Fonts**: Inter font family (loaded from system or CDN)
- **Icons**: Unicode emojis used throughout the design

## Performance Considerations
- Optimize images before adding to repository
- Use appropriate video formats (MP4 with proper compression)
- Minimize unused CSS/JavaScript
- Use semantic HTML for better SEO and accessibility

## Deployment
- Static hosting (Netlify, Vercel, GitHub Pages, etc.)
- No build step required
- Ensure all assets are included in deployment
- Test all functionality post-deployment

## Contributing
- Follow the established code style
- Test changes across multiple browsers and devices
- Maintain responsive design principles
- Ensure accessibility standards are met</content>
<parameter name="filePath">C:\DEVELOPMENT\workspace\my projects\influenceai-landing_v6\AGENTS.md