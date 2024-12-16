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
    id: experience
    content: 
      username: abhinav-exp
    design:
      # Hugo date format
      date_format: 'January 2006'
      # Education or Experience section first?
      is_education_first: false
---

