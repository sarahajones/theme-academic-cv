---
# Leave the homepage title empty to use the site title
title: ""
date: 2026-09-25
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
      title: 'My Research'
      subtitle: ''
      text: |-
        My research asks how people make decisions and applies this question to financial and health decisions. I am interested in how people use the information available to them, and how the environments they're in, including increasingly AI-mediated ones, shape those choices over time.

        This spans several connected threads: the cognitive mechanisms behind confidence and categorisation judgements, the persistence of financial cognitive biases across economic groups, how digital and AI-mediated systems influence real-world financial behaviour, and how these patterns vary across cultures and countries.

        My current research examines how income and assets can shape financial wellbeing, including work showing that cognitive biases in financial decisions persist across economic groups. A related line looks at subjective financial strain, rather than poverty-line status alone, as a driver of financial decision-making and temporal discounting. I also study confidence in decision-making, building on my doctoral research on metacognitive confidence in categorisation judgements. At Columbia, I lead work on the role of AI as a behavioural intervention tool, co-developing and evaluating AI-assisted savings support and chatbot-based interventions with external partners. This applied lens extends to health decisions as well, including analyses of a flu vaccination text-message intervention and appointment no-show rates.

        Alongside this, I direct the Junior Researcher Programme, coordinating large-scale multinational behavioural science studies across 20+ countries, and I'm an advocate for open science practices throughout my work.
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
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      view: article-grid
      columns: 1
  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: date-title-summary
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
  - block: cta-card
    demo: true # Only display this section in the Hugo Blox Builder demo site
    content:
      title: ""
      text: |-
        ""
    design:
      card:
        # Card background color (CSS class)
        css_class: "bg-primary-700"
        css_style: ""
---
