---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Select the user profile to display (username in the content/authors/ folder)
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
          # Add a background image (image from the assets/media/ folder)
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  # - block: markdown
  #   content:
  #     title: '📚 My Research'
  #     subtitle: ''
  #     text: |-
  #       Use this section to explain your goals. I am a research scientist at DeepMind's Moonshot team, and I blog about machine learning, deep learning, and moonshots.

  #       I apply both qualitative and quantitative methods to comprehensively investigate the role of science and technology in the economy.
        
  #       Feel free to reach out for collaborations 😃
  #   design:
  #     columns: '1'
  - block: collection
    id: papers
    content:
      title: Key Projects
      filters:
        folders:
          - major_project
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Libraries and Technologies I'm Studying
      text: ""
      filters:
        folders:
          - major_project
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: Libraries and Technologies I've Studied
      filters:
        folders:
          - event
    design:
      view: article-grid
      columns: 1
  # - block: collection
  #   id: news
  #   content:
  #     title: Recent News
  #     subtitle: ''
  #     text: ''
  #     # Select page type to display (e.g., post, talk, publication...)
  #     page_type: post
  #     # Select number of pages to display (0 = all pages)
  #     count: 5
  #     # Filter criteria
  #     filters:
  #       author: ""
  #       category: ""
  #       tag: ""
  #       exclude_featured: false
  #       exclude_future: false
  #       exclude_past: false
  #       publication_type: ""
  #     # Select number of page offsets
  #     offset: 0
  #     # Page order: descending (desc) or ascending (asc) by date
  #     order: desc
  #   design:
  #     # Select layout view
  #     view: date-title-summary
  #     # Reduce spacing
  #     spacing:
  #       padding: [0, 0, 0, 0]
  - block: cta-card
    demo: true # This section only shows up on the Hugo Blox Builder demo site
    content:
      title: 👉 Create an Academic Website Like This
      text: |-
        This site was built using Hugo Blox Builder, a free, open-source Hugo-based website builder trusted by over 250,000 scholars.

        <a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/hugo-blox-builder on GitHub">Star Hugo Blox Builder on GitHub</a>

        You can build everything easily using blocks - no coding required!
        
        Build landing pages, learning materials, academic CVs, conference sites, tech blogs, and more.
      button:
        text: Get Started
        url: https://hugoblox.com/templates/
    design:
      card:
        # Card background color (CSS class)
        css_class: "bg-primary-700"
        css_style: ""
---
