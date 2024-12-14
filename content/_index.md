---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"
  background: 
    color: 'white'

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: abhinav
      text: ""
      # Show a call-to-action button under your biography? (optional)
    design:
      css_class: light
      background:
        color: light-grey
  - block: collection
    id: publication
    content:
      title: Selected Publications
      filters:
        folders:
          - publication
        featured_only: false
    design:
      css_class: light
      background:
        color: "#f5f5f5"
      view: citation
  - block: resume-experience
    content:
      title: Experience
      username: abhinav-exp
    design:
      # Hugo date format
      date_format: 'January 2006'
      # Education or Experience section first?
      is_education_first: false
  # - block: markdown
  #   content:
  #     title: New
  #     text: "Something new"
      # text: |-
      # Reach out to me at [agrawal.
      # <a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/hugo-blox-builder on GitHub">Star</a> 
      # abhinav1@gmail.com](mailto:agrawal.abhinav1@gmail.com) or [aagrawal@cs.umass.edu](mailto:aagrawal@cs.umass.edu)

  # - block: resume-experience
  #   content:
  #     # The user's folder name in `content/authors/`
  #     username: abhinav
  #   design:
  #     # Hugo date format
  #     date_format: 'January 2006'
  #     # Education or Experience section first?
  #     is_education_first: false
  # - block: resume-awards
  #   content:
  #     title: Awards
  #     # Note: `username` refers to the user's folder name in `content/authors/`
  #     username: abhinav

#   - block: resume-biography-3
#     content:
#       # Choose a user profile to display (a folder name within `content/authors/`)
#       username: abhinav
#       text: ""
#       # Show a call-to-action button under your biography? (optional)
#     design:
#       background:
#         color: white
#  - block: collection
#     id: section-1
#     content:
#       title: Section 1
#       subtitle: A subtitle
#       text: Add any **markdown** formatted content here - text, images, videos, galleries - and even HTML code!
#       # Display content from the `content/post/` folder
#       filters:
#         folders:
#           - publication
#     design:
#       # Choose how many columns the section has. Valid values: '1' or '2'.
#       columns: '1'
#       # Choose your content listing view - here we use the `showcase` view
#       view: showcase
#       # For the Showcase view, do you want to flip alternate rows?
#       flip_alt_rows: true

# - block: collection
#     content:
#       title: Recent Publications
#       text: ""
#       filters:
#         folders:
#           - publication
#         exclude_featured: false
#     design:
#       view: card
  # - block: markdown
  #   content:
  #     title: "Contact Me"
---

