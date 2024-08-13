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
        url: utils/cv.pdf
    design:
      css_class: white
      background:
        color: white
        image:
          # Add your image background to `assets/media/`.
          filename: bg2.jpg
          filters:
            brightness: 1
          size: cover
          position: center
          parallax: false

  # - block: markdown
  #   content:
  #     title: '📚 My Research'
  #     subtitle: ''
  #     text: |-
  #       Use this area to speak to your mission. I'm a research scientist in the Moonshot team at DeepMind. I blog about machine learning, deep learning, and moonshots.

  #       I apply a range of qualitative and quantitative methods to comprehensively investigate the role of science and technology in the economy.
        
  #       Please reach out to collaborate 😃
  #   design:
  #     columns: '1'

  # - block: collection
  #   id: papers
  #   content:
  #     title: Featured Publications
  #     filters:
  #       folders:
  #         - publication
  #       featured_only: true
  #   design:
  #     view: article-grid
  #     columns: 2

  - block: collection
    content:
      title: Research
      text: |-
        <div style="font-family: 'Times New Roman', Times, serif; font-size: 20px; ">
        My research interests lie in 3D computer vision and multi-modal learning,
        especially in the context of scene understanding and generation.
        I have worked on several projects about 3D semantic learning, static and dynamic scene reconstruction, and 3D object detection.
        <br><br>
        
        I'm looking for research internship opportunities in related fields.
        Feel free to contact me! 😃
        </div>
      filters:
        folders:
          - research
        exclude_featured: false
    design:
      view: citation
      

  - block: resume-experience
    content:
      # The user's folder name in `content/authors/`
      username: admin
    design:
      # Hugo date format
      date_format: 'January 2006'
      # Education or Experience section first?
      is_education_first: false
      spacing:
        padding: [0, 0, 0, 0]

  - block: collection
    content:
      title: Awards & Honors
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: awards
      # Choose how many pages you would like to display (0 = all pages)
      count: 0
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
      view: community/my-date-title-summary
      # Reduce spacing
      # spacing:
      #   padding: [0, 0, 0, 0]


      

  ###################################################################

  - block: collection
    demo: true
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
    demo: true
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
---