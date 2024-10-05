---
# Leave the homepage title blank to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Select the user profile to display (username inside content/authors/ folder)
      username: admin
      text: ""
      # Show action button below biography? (optional)
      button:
        text: Download Resume
        url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add background image (image inside assets/media/ folder)
          filename: stacked-peaks.webp
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false

  - block: collection
    id: papers
    content:
      title: Major Projects
      filters:
        folders:
          - major_project
        featured_only: true
    design:
      view: article-grid
      columns: 3
  
  - block: collection
    content:
      title: Libraries and Technologies I'm Studying
      text: ""
      filters:
        folders:
          - studying
        exclude_featured: false
    design:
      view: card
      columns: 3
  
  - block: collection
    content:
      title: Ongoing Projects
      filters:
        folders:
          - progressing
    design:
      view: article-grid
      columns: 3
    
  - block: carousel
    content:
      slides:
      - image: /unsplash/slider1.jpg
        content_html: "4th year at Jeonbuk National University"
      - image: /unsplash/slider2.jpg
        content_html: "Department of Computer Engineering"
      - image: /unsplash/slider3.jpg
        content_html: "Aspiring Backend Developer"
      - image: /unsplash/slider4.jpg
        content_html: "Hobby is running"
      duration: 3000
      items: 1        
      height: 500   
      unit: px
---
