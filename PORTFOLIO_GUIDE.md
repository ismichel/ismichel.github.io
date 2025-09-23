# Portfolio Website Guide

This guide explains how to use the enhanced portfolio features on your website.

## New Features Added

### 1. Enhanced About Section
- More professional and portfolio-focused introduction
- Clear statement about job search status
- Highlighted multidisciplinary background

### 2. Expandable Project Details
Each project in the Technical Projects section now supports:
- **Learn More button**: Click to expand detailed project information
- **Detailed Description**: Comprehensive project overview
- **Creation Process**: Step-by-step development process
- **Demo Videos**: Embedded video demonstrations
- **Technologies Used**: Visual tags showing tech stack

### 3. Technical Skills Section
- Organized by category (Programming Languages, Frameworks, Tools, etc.)
- Color-coded skill tags
- Responsive grid layout

### 4. Improved Styling
- Modern, clean design
- Hover effects on interactive elements
- Better responsive design for mobile devices
- Enhanced project cards with shadows and animations

## How to Add New Projects

To add a new project with detailed information, create a new markdown file in `_posts/` with the following frontmatter:

```yaml
---
layout: post
title: "Your Project Title"
date: 2024-01-15 10:00:00 +00:00
image: /images/your-project-image.jpg
categories: other
course: "Course Name or Project Type"
author: "Your Name"
detailed_description: "Comprehensive description of what the project does and its impact."
creation_process: "Step-by-step description of how you built the project, challenges faced, and solutions implemented."
demo_video: "/videos/your-demo.mp4"  # Optional
technologies: ["Python", "React", "TensorFlow", "AWS"]  # Optional
code: https://github.com/yourusername/project
website: https://your-project-demo.com
---
Your project excerpt that appears in the main listing.
```

## Supported Project Fields

- `detailed_description`: Long-form project description
- `creation_process`: Development process and methodology
- `demo_video`: Path to demo video file
- `technologies`: Array of technologies used
- `code`: Link to source code
- `website`: Link to live demo
- `paper`: Link to research paper
- `poster`: Link to poster presentation
- `slides`: Link to presentation slides
- `video`: Link to external video

## Demo Videos

To add demo videos:
1. Place video files in the `videos/` directory
2. Reference them in the `demo_video` field
3. Supported formats: MP4, WebM, OGG
4. Videos will be embedded with native HTML5 controls

## Customization

### Skills Section
Edit the skills in `_layouts/default.html` around line 244-288 to match your actual skills.

### Colors and Styling
Modify `style.scss` to change colors, fonts, and layout.

### Section Order
Reorder sections in `_layouts/default.html` by moving the table blocks around.

## Best Practices

1. **Project Images**: Use high-quality, consistent images (recommended size: 300x200px)
2. **Demo Videos**: Keep videos under 2 minutes for better user engagement
3. **Descriptions**: Write detailed descriptions that highlight your problem-solving skills
4. **Technologies**: Be specific about versions and frameworks used
5. **Links**: Ensure all external links are working and up-to-date

## Mobile Responsiveness

The portfolio is optimized for:
- Desktop (1200px+)
- Tablet (768px - 1199px)
- Mobile (320px - 767px)

Test your site on different devices to ensure optimal viewing experience.
