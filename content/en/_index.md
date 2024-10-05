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
    
  - block: slider
    content:
      slides:
      - title: Who am I?
        content: A student with an interest in DevOps
        align: center
        background:
          image:
            filename: slider/slider1.jpg
            filters:
              brightness: 0.7
          position: right
          color: '#666'
      - title: Technologies I've Learned
        content: 'React, Spring Boot, FastAPI'
        align: left
        background:
          image:
            filename: slider/slider2.jpg
            filters:
              brightness: 0.7
          position: center
          color: '#555'
      - title: Please click the button below to contact me!
        align: right
        background:
          image:
            filename: slider/slider3.jpg
            filters:
              brightness: 0.5
          position: center
          color: '#333'
        link:
          text: Contact
          url: ../contact/
    design:
      slide_height: '800px'
      is_fullscreen: true
---
