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
        - title: PhD Student
          company: Ecole des Ponts ParisTech
          company_url: 'https://imagine-lab.enpc.fr/'
          company_logo: 
          location: Paris/France
          date_start: '2023-10-01'
          date_end: ''
          description: |2-
              Research Topics:
              * Active object detection, 3D scene reconstruction, neural implicit models.
              
        - title: Machine Learning Engineer
          company: Upily
          company_url: 'https://upily.com/'
          company_logo: Artboard_1
          location: Istanbul/Turkey
          date_start: '2023-06-10'
          date_end: '2023-09-20'
          description: |2-
              Responsibilities include:
              * Research, development, and implementation of learning-based cartoon animation and speech generation methods.
              
    
        - title: Machine Learning Research Engineer
          company: Deep Learning and Medical Image Analysis Laboratory (DeepMIA)
          company_url: 'https://deepmia.boun.edu.tr/'
          company_logo: boun_logo
          location: Istanbul/Turkey
          date_start: '2022-11-01'
          date_end: '2023-06-10'
          description: |2-
              Responsibilities include:
              * Actively participating in research projects related to both autonomous driving and medical image analysis.
              * Advising and guiding bachelor's students on their graduation projects.
             
        - title: Graduate Research Assistant
          company: ITU Aerospace Research Center
          company_url: 'https://arc.itu.edu.tr/'
          company_logo: Istanbul_Technical_University_logo
          location: Istanbul/Turkey
          date_start: '2021-02-01'
          date_end: '2022-06-01'
          description: |2-
              Responsibilities include:
              * Participated in various industrial projects and helped develop navigation algorithms for cyber-physical systems.
              * Took part in dataset preparation for DL algorithm trainings.
        
        - title: Internship
          company: Altınay Aerospace and Advanced Technology Inc., Robotics Department
          company_url: 'http://www.altinay.com/'
          company_logo: 
          location: Istanbul/Turkey
          date_start: '2020-01-01'
          date_end: '2020-03-01'
          description: |2-
              Responsibilities include:
              * Helped developing a simulation software for a rover type vehicle with velodyne LIDAR mounted on top in Gazebo environment. 
              
              
    design:
      columns: '2'
  - block: accomplishments
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
        - certificate_url: 
          date_end: '2021-09-01'
          date_start: '2020-09-01'
          description: ''
          organization: The Boeing Company
          organization_url: 
          title: The Boeing Scholarhip
          url: ''
        - certificate_url: 
          date_end: ''
          date_start: '2020-08-01'
          organization: Istanbul Technical University
          organization_url:
          title: Student Salutatorian
          url:
        - certificate_url: 
          date_end: '2020-06-01'
          date_start: '2017-09-01'
          description: ''
          organization: Presidency for Turks Abroad and Related Communities
          organization_url: 
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
      
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        
      # Contact (add or remove contact options as necessary)
      email: artikov.arslan@gmail.com
      phone: +90 553 157 0831
      
      
      contact_links:
        
        
        
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      
    design:
      columns: '2'
---
