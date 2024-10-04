---
title: 'One fitness CRM'

authors:
  - admin

date: '2013-07-01T00:00:00Z'
doi: ''

publishDate: '2017-01-01T00:00:00Z'

# 요약
summary: 해당 프로젝트는 One Fitness 헬스장의 전산 시스템을 웹 형태로 전환하며, 각 트레이너들의 PT를 관리하고, 월급을 자동으로 계산하는 프로젝트입니다.

tags:
  - React
  - Fast API

share: false
featured: true

image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
  focal_point: ''
  preview_only: false
---

# 프로젝트 설명
해당 프로젝트는 기존 One fitness 헬스장의 전산 시스템이 엑셀로 되어있습니다. 엑셀에 되어있음에 따라서 PT 횟수를 수동으로 주입해야 하며, 트레이너들이 자기의 책임을 모두 지지 않고 PT 기록을 거짓으로 넣는 경우가 있기에 이러한 경우를 방지하고자 만드는 프로젝트 입니다.

## 프로젝트 사용 도구
### Frontend:
프론트 엔드에서는 React를 사용합니다. React와 관련된 여러 라이브러리를 도입하여 프로젝트의 구조와 개발을 더 쉽게 하였습니다.

- TanStack Router
  - 기존 React-Router-Dom 의 경우 일일이 Route를 수동으로 설정해줘야 하지만, 해당 라이브러리를 사용하면 디렉터리 구조로 라우터를 설정해줍니다.
- TanStack Query
  - 해당 라이브러리를 사용하여 UPDATE, PUT, PATCH, GET 요청 이후 수행할 작업을 자동화 하여 데이터의 동기화를 유지합니다.
- Axios
  - 해당 라이브러리는 API 호출과 관련한 설정을 보다 쉽게 해주는 라이브러리에 속합니다.

### Backend:
백엔드에서는 Fast API과 SQLite를 사용합니다.

- Swegger
  - Swegger를 통해서 API 명세서 작성을 자동화하고, API의 테스트를 보다 용이하게 합니다.
- Docker
  - Docker를 통해서 서버를 컨테이너화 시킨 다음에 프론트엔드 개발시 서버의 응답을 보다 용이하게 설정합니다.

## Github Link
- 해당 프로젝트는 비공개 레포지토리에서 진행하였기에 공개가 불가능 합니다.
