---
title: 'Home'
date: 2024-05-13
type: landing
sections:
  - block: resume-biography
    content:
      # The user's folder name in content/authors/
      username: admin
    design:
      banner:
        filename: banner.jpg
      spacing:
        padding: [0, 0, 0, 0]
      biography:
        style: 'text-align: justify; font-size: 0.8em; padding: 10px;'
  - block: markdown
    content:
      title: Me in 10 seconds
      # subtitle: 
      text: 
          I am currently studying Computer Science at the University of Illinois Urbana-Champaign (UIUC).
          I love sharing what I read to empower people.
    design:
      spacing:
        # Customize the section spacing. Order is top, right, bottom, left.
        padding: ['0', '20px', '0', '20px']
  - block: markdown
    content:
      title: Me in 10 minutes?
      # subtitle: 
      text: 
          See my "[about](/about/)" page.
  - block: markdown
    content:
      title: What am I doing now?
      # subtitle: 
      text: 
          See my "[now](/now/)" page.
  - block: collection
    content:
      title: Articles
      filters:
        folders:
          - books
    design:
      spacing:
        padding: ['3rem', 0, '6rem', 0]
      view: card
---
