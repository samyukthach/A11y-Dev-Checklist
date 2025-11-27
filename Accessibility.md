# Accessibility Checklist

**Landmarks & Regions**
 For native landmarks
  - Use `<header>` for top-level page header  
  - Use `<main>` for main content  
  - Use `<nav>` for primary navigation  
  - Use `<aside>` for complementary content  
  - Use `<footer>` for page footer  

 Or Use ARIA incase of not using native elements:
  - `role="banner"` → site header  
  - `role="main"` → main content  
  - `role="contentinfo"` → footer  
  - `role="complementary"` → sidebar or secondary content  
  - `role="navigation"` → primary or secondary navigation  
Tip: Avoid multiple identical landmarks without unique labels (`aria-label`) to distinguish them.  

**Page Titles**
- `<title>` element must accurately describe page content.  
- Page titles should be unique per page.  

**Bypass**
- Ensure **skip links** (`Skip to main content`) are present and functional.
  
**Headings**
- Only one `<h1>` per page**.  
- Maintain correct heading hierarchy (`h1` → `h2` → `h3`).  
- Avoid skipping heading levels.  
- All headings must have meaningful text no empty headings.  
- Headings should describe the section content.  

  
**Touch target**
- Target size should be min 24 * 24px square and it is possible to draw 24*24 aligned within targets		
- Minimum touch target size: 44x44 CSS pixels (SC 2.5.5 Target Size).  
- Ensure sufficient spacing between touch targets to avoid accidental taps.  
- Avoid requiring precise gestures provide alternatives if dragging/swiping is needed (SC 2.5.7 Dragging Movements). 
- Make the entire interactive area clickable, not just the visible text or icon.  
- Ensure touch targets are keyboard focusable and accessible via assistive technologies.  
- Avoid overlapping or hidden touch targets.  
- Ensure links inside text blocks are large enough and spaced properly for finger taps.  
- Test on real devices, not just desktop simulators.  								
Tip: For projects with lots of small icons or inline links, consider adding extra padding or hidden clickable areas to meet touch target size requirements without changing the visual design.



