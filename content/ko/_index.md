---
# 홈페이지 제목을 비워두어 사이트 제목을 사용
title: ""
date: 2022-10-24
type: landing

design:
  # 기본 섹션 간격
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # 표시할 사용자 프로필 선택 (content/authors/ 폴더 내 사용자명)
      username: admin
      text: ""
      # 바이오그래피 아래에 동작 버튼 표시? (선택 사항)
      button:
        text: 이력서 다운로드
        url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # 배경 이미지 추가 (assets/media/ 폴더 내 이미지)
          filename: stacked-peaks.webp
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false

  - block: collection
    id: papers
    content:
      title: 주요 프로젝트
      filters:
        folders:
          - major_project
        featured_only: true
    design:
      view: article-grid
      columns: 3
  
  - block: collection
    content:
      title: 공부중인 라이브러리 및 기술
      text: ""
      filters:
        folders:
          - studying
        exclude_featured: false
    design:
      view: card
      columns: 3
  
  - block: collection
    content:
      title: 진행중인 프로젝트
      filters:
        folders:
          - progressing
    design:
      view: article-grid
      columns: 3
  - block: carousel
    content:
      slides:
        - image: unsplash/slider1.jpg
          content_html: "전북대학교 4학년"
        - image: unsplash/slider2.jpg
          content_html: "컴퓨터공학과"
        - image: unsplash/slider3.jpg
          content_html: "백엔드 개발자 희망"
        - image: unsplash/slider4.jpg
          content_html: "취미는 러닝"
      duration: 3000
      items: 1        
      height: 500   
      unit: px       
---
