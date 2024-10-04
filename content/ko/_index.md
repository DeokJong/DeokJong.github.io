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
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  # - block: markdown
  #   content:
  #     title: '📚 나의 연구'
  #     subtitle: ''
  #     text: |-
  #       이 영역을 사용하여 귀하의 목표를 설명하세요. 저는 DeepMind의 Moonshot 팀에서 연구 과학자로 일하고 있습니다. 기계 학습, 딥러닝 및 문샷에 대해 블로그를 운영하고 있습니다.

  #       저는 질적 및 양적 방법을 모두 적용하여 과학과 기술이 경제에 미치는 역할을 포괄적으로 조사합니다.
        
  #       협업을 원하시면 언제든지 연락 주세요 😃
  #   design:
  #     columns: '1'
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
      - title: 👋 Welcome to the group
        content: Take a look at what we're working on...
        align: center
        background:
          image:
            filename: coders.jpg
            filters:
              brightness: 0.7
          position: right
          color: '#666'
      - title: Lunch & Learn ☕️
        content: 'Share your knowledge with the group and explore exciting new topics together!'
        align: left
        background:
          image:
            filename: contact.jpg
            filters:
              brightness: 0.7
          position: center
          color: '#555'
      - title: World-Class Semiconductor Lab
        content: 'Just opened last month!'
        align: right
        background:
          image:
            filename: welcome.jpg
            filters:
              brightness: 0.5
          position: center
          color: '#333'
        link:
          text: Join Us
          url: ../contact/
    design:
      slide_height: '800px'
      is_fullscreen: true
  # - block: collection
  #   id: news
  #   content:
  #     title: 최근 뉴스
  #     subtitle: ''
  #     text: ''
  #     # 표시할 페이지 유형 (예: post, talk, publication...)
  #     page_type: post
  #     # 표시할 페이지 수 선택 (0 = 모든 페이지)
  #     count: 5
  #     # 필터 기준
  #     filters:
  #       author: ""
  #       category: ""
  #       tag: ""
  #       exclude_featured: false
  #       exclude_future: false
  #       exclude_past: false
  #       publication_type: ""
  #     # 페이지 오프셋 수 선택
  #     offset: 0
  #     # 페이지 순서: 날짜 내림차순(desc) 또는 오름차순(asc)
  #     order: desc
  #   design:
  #     # 레이아웃 보기 선택
  #     view: date-title-summary
  #     # 간격 축소
  #     spacing:
  #       padding: [0, 0, 0, 0]
  # - block: cta-card
  #   demo: true # 이 섹션은 Hugo Blox Builder 데모 사이트에서만 표시됨
  #   content:
  #     title: 👉 이렇게 학술 웹사이트를 만들어보세요
  #     text: |-
  #       이 사이트는 250,000명 이상의 학자들이 신뢰하는 무료 Hugo 기반 오픈 소스 웹사이트 빌더인 Hugo Blox Builder로 생성되었습니다.

  #       <a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/hugo-blox-builder on GitHub">GitHub에서 Hugo Blox Builder에 Star 달기</a>

  #       블록을 사용하여 모든 것을 쉽게 빌드할 수 있습니다 - 코딩 불필요!
        
  #       랜딩 페이지, 학습 자료, 학술 이력서, 컨퍼런스, 기술 블로그 등 다양한 사이트를 구축할 수 있습니다.
  #     button:
  #       text: 시작하기
  #       url: https://hugoblox.com/templates/
  #   design:
  #     card:
  #       # 카드 배경 색상 (CSS 클래스)
  #       css_class: "bg-primary-700"
  #       css_style: ""
---
