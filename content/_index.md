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
        I study the cognitive and neural basis of complex, naturalistic human behavior.
        My research program combines interactive neuroimaging experiments built in modern game engines with high-dimensional computational models of brain activity.


        Real-world experience emerges from a continuous loop of perception, cognition, and action that static experimental paradigms cannot engage.
        I built a naturalistic neuroimaging platform that immerses participants in dynamic virtual worlds that respond to their actions, and uses the game engine itself to extract tens of thousands of features for modeling.


        With this platform I have produced the first quantitative map of the cortical network that mediates active navigation.
        Current work extends it to collaborative problem solving, interactions between humans and embodied AI agents, and the dynamics of brain activity that produce continuous behavior.
      # Show a call-to-action button under your biography? (optional)
      # button:
      #   text: Download CV
      #   url: uploads/resume.pdf
      headings:
        about: 'Human brain substrates of the perception-cognition-action loop'
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
