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
      view: article-grid
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
    
  - block: slider
    content:
      slides:
      - title: 나는 누구인가?
        content: DevOps에 관심이 많은 학생
        align: center
        background:
          image:
            filename: coders.jpg
            filters:
              brightness: 0.7
          position: right
          color: '#666'
      - title: 배운 기술
        content: 'React, Spring Boot, FastAPI'
        align: left
        background:
          image:
            filename: contact.jpg
            filters:
              brightness: 0.7
          position: center
          color: '#555'
      - title: 저에게 연락하려면 아래의 버튼을 눌러주세요!
        align: right
        background:
          image:
            filename: welcome.jpg
            filters:
              brightness: 0.5
          position: center
          color: '#333'
        link:
          text: 연락
          url: ../contact/
    design:
      slide_height: '800px'
      is_fullscreen: true
---
