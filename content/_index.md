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


        My work has focused on using fMRI and high-dimensional models to map the functional network in the human cerebral cortex that mediates active spatial navigation.


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
        gradient_mesh:
          enable: true

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
