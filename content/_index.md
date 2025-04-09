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
      #button跳转到qq群？

    design:
      css_class: dark
      background:
        color: '#f0f0f0'
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
      #title: '🛠战队研究方向'
      title: ''
      #subtitle: '战队研究方向'
      text: |-


          ## 战队研究方向
          可操控智能机器人：英雄、步兵、平衡步兵、无人机、飞镖发射架
            自主决策智能系统：哨兵、制导飞镖镖体
          ## 什么是RM？
          rm....
          😃

    design:
      columns: '1'
      #css_class: dark
      background:
        color: '#f0f0f0'  # 设置背景颜色




  #- block: collection
    #id: awards
    #content:
      #title: History Award
    # filters:
    #    folders:
    #      - awards
        
    #    featured_only: true
    #design:
    #  view: article-grid
    #  columns: 2
  #- block: collection
  #  content:
  #    title: Recent Publications
  #    text: ""
  #    filters:
  #      folders:
  #        - publication
  #      exclude_featured: false
  #  design:
  #    view: citation

#  - block: collection
#    id: details
#    content:
#      title: 🦈战队详情
#      filters:
#        folders:
#          - event
#    design:
#      view: article-grid
#      columns: 1
  - block: collection
    id: details
    content:
      title: 🦈战队详情
      filters:
        folders:
          - event
    design:
      view: article-list
      columns: 1


      
  - block: collection
    id: news
    content:
      title: Recent News
      #subtitle: ''
      #text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 3
      # Filter on criteria
      filters:
        #author: ""
        category: ""
        tag: "news"
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
 

  - block: markdown
    id: join_us
    content:
      title: '👉 加入我们：'
      subtitle: ''
      text: |-
       <div class="text-center">
          欢迎对机器人制造、控制感兴趣的小伙伴们加入我们！

          QQ迎新群:665139428

          也欢迎大家关注鲨鲨酱的：

          哔哩哔哩：南海鲨机器人实验室
        </div>
    design:
      columns: '1'


---
