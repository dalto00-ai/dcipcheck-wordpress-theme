# DCIPCHECK WordPress/Elementor Export Files

This directory contains WordPress and Elementor theme files for the DCIPCHECK IP lookup tool.

## Files Included

### WordPress Theme File
- **theme.json** - WordPress block theme configuration file with color palette, typography, and global styles

### Elementor Templates
- **dcipcheck-header.json** - Header template with logo and navigation
- **dcipcheck-main-page.json** - Main IP lookup page template with hero, search, cards, and map sections
- **dcipcheck-footer.json** - Footer template with copyright and links

## How to Use

### WordPress theme.json
1. Copy `theme.json` to your WordPress theme root directory
2. The file defines your theme's color palette, typography, and global styles
3. WordPress will automatically detect and apply these settings

### Elementor Templates
1. Go to **WordPress Admin > Elementor > Templates**
2. Click **Import Templates**
3. Upload each `.json` file from the `elementor-templates` folder
4. Click **Import** for each template
5. Assign templates to your pages:
   - Header: Go to **Elementor > Theme Builder > Header** and assign `DCIPCHECK Header`
   - Footer: Go to **Elementor > Theme Builder > Footer** and assign `DCIPCHECK Footer`
   - Main Page: Create a new page and insert the `DCIPCHECK IP Lookup Page` template

## Important Notes

### Images and Media
- Replace `[YOUR_LOGO_URL]` in the header template with your actual logo URL
- Upload your logo to WordPress Media Library first
- All images referenced in templates must be uploaded to your WordPress site

### Functionality Requirements
For the IP lookup functionality to work, you'll need:
1. **Custom Plugin or Code**: The templates provide the UI structure only
2. **IP API Integration**: Connect to ip-api.com or similar service via custom PHP code
3. **JavaScript**: Add custom JS to handle form submissions and API calls
4. **Database**: Optional - to store lookup history

### Color Palette
The theme uses these colors (matching your React app):
- Primary: #3b82f6 (Blue)
- Secondary: #1e40af (Dark Blue)
- Success: #22c55e (Green)
- Warning: #f59e0b (Orange)
- Destructive: #ef4444 (Red)

### Typography
- Primary Font: Inter (sans-serif)
- Monospace Font: JetBrains Mono

### Google AdSense
- AdSense placeholder divs are included in the templates
- Replace with actual AdSense ad units once your site is approved
- Remember to add the AdSense verification code to your WordPress header

### Multi-Language Support
These templates are ready for translation plugins like:
- WPML
- Polylang
- TranslatePress

## Customization

You can customize these templates in Elementor:
1. Edit any imported template from **Elementor > Templates**
2. Modify colors, fonts, spacing, and content
3. Save changes - they'll apply across all pages using that template

## Support

For WordPress/Elementor specific help:
- WordPress Documentation: https://wordpress.org/documentation/
- Elementor Documentation: https://elementor.com/help/

For DCIPCHECK specific features:
- Refer to your React application codebase for API integration details
