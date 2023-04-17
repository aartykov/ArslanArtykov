---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.avatar
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      # Override your bio text from `authors/admin/_index.md`?
      text:
  
  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Machine Learning Research Engineer
          company: Deep Learning and Medical Image Analysis Laboratory (DeepMIA) 
          company_url: 'https://deepmia.boun.edu.tr/'
          company_logo: boun_logo
          location: Istanbul/Turkey
          date_start: '2022-11-01'
          date_end: ''
          description: |2-
              Responsibilities include:

              * Deep Learning based Algorithm Development  
              * Dataset Preparation for ML Algorithm Training
              
            
        
        - title: Graduate Research Assistant
          company: ITU Aerospace Research Center 
          company_url: 'https://arc.itu.edu.tr/'
          company_logo: 
          location: Istanbul/Turkiye
          date_start: '2021-02-01'
          date_end: '2022-06-01'
          description: |2-
              Responsibilities include:

              * Algorithm Development for an Autonomous Drone
              * Dataset Preparation for ML Algorithm Training
              * Deploying ML Algorithms on Platforms
        
    design:
      columns: '2'
  
  - block: features
    content:
      title: Skills
      items:
        - name: Python
          description: 90%
          icon: r-project
          icon_pack: fab
        - name: PyTorch
          description: 90%
          icon: chart-line
          icon_pack: fas
        - name: 
          description: 10%
          icon: camera-retro
          icon_pack: fas
          
  - block: awards
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Awards'
      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - date_end: '2021-09-01'
          date_start: '2020-09-01'
          description: ''
          organization: The Boeing Company
          organization_url: ''
          title: 'Boeing Scholarship'
          url: ''
        
        - date_end: ''
          date_start: '2020-08-01'
          description: ''
          organization: Istanbul Technical University
          organization_url: ''
          title: Student Salutatorian
          url: ''
          
        - date_end: '2020-08-01'
          date_start: '2017-08-01'
          description: ''
          organization: Presidency for Turks Abroad and Related Communities
          organization_url: ''
          title: Turkiye Scholarship
          url: ''
        
    design:
      columns: '2'
  
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: Deep Learning
          tag: Deep Learning
        - name: Other
          tag: Demo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
 
  - block: collection
    content:
      title: Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
 
  - block: contact
    id: contact
    content:
      title: Contact
      # Contact (add or remove contact options as necessary)
      email: artikov.arslan@gmail.com
      phone: +90 553 157 0831
      appointment_url: ''
      address:
        street: 
        city: 
        region: 
        postcode: ''
        country: 
        country_code:
      directions: 
      contact_links:
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'
---
