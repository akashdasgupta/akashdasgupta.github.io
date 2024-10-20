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
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        My research focuses on the measurement and analysis of perovskite solar cells, with a particular emphasis on using advanced spectroscopy techniques to gain insights into device performance and degradation. I specialize in developing innovative approaches for data acquisition, enabling a deeper understanding of the fundamental processes that govern the behavior of perovskite materials.
        Using my strong expertise in spectroscopy, optical modelling and drift-diffusion simulations, and bayesian inference, I work to quantify key parameters such as charge collection efficiency, material heterogeneity, and recombination processes. I design and build custom measurement systems to acquire high-quality data, and leverage my coding skills to run simulations that complement experimental results.
        By combining detailed experimental analysis with modeling, my goal is to provide a clearer understanding of the limits and potential of perovskite solar cells, offering valuable insights that can guide future research and development in the field.
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Recent Publications
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
---
