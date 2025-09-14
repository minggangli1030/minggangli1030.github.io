# Claude Code Instructions

This document contains instructions and context for Claude Code when working on this Jekyll website.

## Site Overview

This is a personal academic website built with Jekyll, showcasing:
- Personal information and CV
- Projects and coursework
- Photography (Kenya 2018 wildlife collection)
- Miscellaneous content

## Development Commands

### Local Development
- `bundle exec jekyll serve` - Start local development server
- `bundle exec jekyll build` - Build the site

### Testing
- Check that the site builds without errors before making changes
- Test responsive design on mobile and desktop

## Site Structure

### Key Directories
- `_pages/` - Main site pages (about, projects, coursework, misc, photography)
- `_data/navigation.yml` - Site navigation configuration
- `images/` - General site images and assets
- `Kenya 2018/` - Photography collection from Kenya trip
- `_config.yml` - Jekyll configuration
- `assets/` - CSS, JS, and other assets

### Navigation Structure
Main navigation items (in order):
1. Home
2. CV (PDF link)
3. Projects
4. Coursework
5. Misc (contains photography and other content)

### Collections
The site uses Jekyll collections for:
- `teaching`
- `publications`
- `portfolio`
- `talks`

## Photography Section

The photography showcase is organized under Misc and includes:
- Wildlife photos from Kenya 2018 trip
- Categorized by: Birds, Large Birds & Water Birds, Mammals, Reptiles & Other Wildlife
- Responsive gallery layout with hover effects
- All photos are located in `/Kenya 2018/` directory

## Content Guidelines

- Keep the academic/professional tone consistent
- Use proper image alt text for accessibility
- Maintain responsive design principles
- Follow existing markdown formatting conventions

## Common Tasks

### Adding New Photos
1. Place images in appropriate directory
2. Update relevant page markdown
3. Ensure proper alt text and captions
4. Test responsive layout

### Adding Navigation Items
1. Edit `_data/navigation.yml`
2. Create corresponding page in `_pages/`
3. Test navigation functionality

### Updating CV
1. Replace PDF in `images/` directory
2. Update link in `_data/navigation.yml` if filename changes

## Site Author Info

- Name: Minggang (Martin) Li
- Email: minggangli@berkeley.edu
- GitHub: minggangli1030
- LinkedIn: minggangli1030
- Location: Berkeley, CA
- Institution: UC Berkeley (Applied Math, Data Science, CS)