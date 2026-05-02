# Copilot Cloud Agent Instructions for Project-Git

## Repository Overview

**Project Type:** Static HTML/CSS Portfolio Website  
**Language:** HTML, CSS  
**Repository Size:** ~286 KB (small)  
**Default Branch:** `master`  
**No Build System:** This repository contains only static HTML files and CSS stylesheets with no build, test, or deployment pipeline.

### What This Repository Does

This is a team portfolio website showcasing profiles of three students from the National Technical University of Ukraine "Dnipro Polytechnic." The repository contains:

- **git.html/git.css** - Main team page displaying all three team members with clickable links to individual pages
- **bob.html/bob.css** - Individual profile page for Boboshko Oleksii
- **dima.html/dima.css** - Individual profile page for Kuchugurny Dmitro
- **ira.html/ira.css** - Individual profile page for Patlan Iryna
- **Image files** - Profile photos (dima.jpg, ira.jpg, leha.jpg, ntu_dp.png)

## File Structure

All files are located at the **repository root** (no subdirectories):

```
Project-Git/
├── git.html            # Main team page
├── git.css             # Main team page styles
├── bob.html            # Bob's profile
├── bob.css             # Bob's profile styles
├── dima.html           # Dima's profile
├── dima.css            # Dima's profile styles
├── ira.html            # Ira's profile
├── ira.css             # Ira's profile styles
├── dima.jpg            # Dima's profile photo
├── ira.jpg             # Ira's profile photo
├── leha.jpg            # Bob's profile photo
├── ntu_dp.png          # University logo/image
└── .github/
    └── copilot-instructions.md  # This file
```

## Key Information for Code Changes

### HTML Structure
- All HTML files use UTF-8 encoding with `<meta charset="UTF-8">`
- All HTML files set viewport meta tag: `<meta name="viewport" content="width=device-width, initial-scale=1.0">`
- Links between pages use relative file references (e.g., `href="bob.html"`)
- **Important:** The main navigation page is `git.html` which links to all individual profile pages

### CSS Styling
- All CSS files use a consistent background color: `rgb(144, 187, 204)` (light blue)
- Profile images are styled as circles with `border-radius: 50%`
- All pages use flexbox for layout: `display: flex; flex-direction: column; align-items: center;`
- Font families used: 'Segoe UI', 'Impact', 'Haettenschweiler', sans-serif
- Text shadows use `-webkit-text-stroke` for outlined text effects

### HTML-CSS Linking
- Individual profile pages link their corresponding CSS files: `<link rel="stylesheet" href="[name].css">`
- **Critical:** Bob's page links to `bob.css`, Dima's to `dima.css`, Ira's to `ira.css`
- Main team page links to `git.css`

### Image References
- Images are referenced by filename only (all at root): `src="leha.jpg"`, `src="dima.jpg"`, `src="ira.jpg"`
- Image dimensions vary: individual profile photos are 400x400px (personal pages) and 200x200px (team page)

## Build and Deployment

**No build system, tests, or CI/CD pipeline exists.** This is a static website that works immediately when HTML files are served in a web browser. To validate changes:

1. **Open any HTML file directly in a web browser** to preview changes locally
2. **Test all navigation links** - From git.html, verify links to bob.html, dima.html, and ira.html work
3. **Verify image display** - All image files must be present in the root directory
4. **Check styling** - Ensure CSS files are properly linked and styles render correctly

## Important Notes

- **No dependencies, package manager, or build tools** - This is pure HTML/CSS
- **No validation pipeline or automated tests** - Changes are validated by manual browser testing
- **Relative file paths only** - All links and image references use relative paths (no absolute paths)
- **All files must remain at repository root** - Do not move files into subdirectories unless updating all references
- **CSS consistency** - Maintain the blue background color scheme (`rgb(144, 187, 204)`) and flexbox layouts across pages
- **Ukrainian text** - Most content is in Ukrainian; preserve text encoding and character support

## Recent Activity

The repository was created 36 days ago and last updated 31 days ago. There is currently one open pull request (#3 "Dima bran") that has not been merged.

## Trust These Instructions

These instructions reflect the current state and structure of the repository. **Trust this information and only perform a search if you find the instructions to be incomplete or inaccurate.** The repository is small and simple with no hidden complexity, build systems, or validation pipelines.
