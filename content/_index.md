---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
type: landing

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
      text: |-		
        I use dynamic neuroimaging experiments and use advanced computational methods to understand the cognitive and neural basis of complex, naturalistic human behavior. 


        My research focuses on spatial navigation, collaborative problem solving, and dynamic multiagent interactions.


        Real-world experiences emerge out of a continuous perception-cognition-action loop that cannot be captured by classical experimental paradigms.
        To enable ecologically valid experiments, I built a naturalistic neuroimaging paradigm that immerse participants in dynamic virtual worlds, and utilitizes the capabilities of modern game engines to extract features for analysis.
      # Show a call-to-action button under your biography? (optional)
      # button:
      #   text: Download CV
      #   url: uploads/resume.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        # Painted on the section itself, behind the gradient mesh
        color:
          light: '#0a0a0f'
          dark: '#0a0a0f'
        # Painted on .home-section-bg, above the gradient mesh
        # At 50% width, 100% is exactly half the brain's width right of centre, and half its height is
        # 21.63vw (50% width scaled by the 1510/1745 source aspect ratio, halved).
        image:
          filename: colorful-brain.png
          size: 33%
          position: center
          parallax: false
        gradient_mesh:
          enable: true
          intensity: medium

      # Name heading sizing to accommodate long or short names
      name:
        size: md # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: square # Options: circle (default), square, rounded
  - block: collection
    id: publications
    content:
      title: Featured Publications
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 3
      show_date: false
      show_read_time: false
      show_read_more: false
  - block: collection
    content:
      title: Recent Publications
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
---
