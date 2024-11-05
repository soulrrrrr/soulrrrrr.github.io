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
        style: 'text-align: justify; font-size: 0.8em;'
  - block: markdown
    content:
      title: Me in 10 seconds
      # subtitle: 
      text: 
          I studied computer science at NYCU and NTU in Taiwan.  
          I am currently an incoming graduate student at the University of Illinois at Urbana-Champaign (UIUC).
          I love to share what I read to empower people.
  - block: markdown
    content:
      title: Me in 10 minutes
      # subtitle: 
      text: 
          Check my [About](/about/) page.
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
