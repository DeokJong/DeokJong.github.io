---
title: 'One Fitness CRM'

authors:
  - admin

date: '2013-07-01T00:00:00Z'
doi: ''

publishDate: '2017-01-01T00:00:00Z'

# Summary
summary: This project transitions the computerized system of One Fitness gym into a web-based format. It manages personal training (PT) sessions for each trainer and automatically calculates their salaries.

tags:
  - React
  - FastAPI

share: false
featured: true

image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
  focal_point: ''
  preview_only: false
---

# Project Description
The current computerized system at One Fitness gym is based on Excel. Since the PT sessions need to be manually recorded in Excel, there are cases where trainers might falsify their PT records. This project aims to prevent such occurrences by automating the process and ensuring accountability.

## Project Tools
### Frontend:
The frontend uses React, along with several libraries to simplify the project structure and development.

- TanStack Router:
  - Unlike React-Router-Dom, where routes must be manually configured, this library allows routes to be configured based on the directory structure.
- TanStack Query:
  - This library automates tasks after UPDATE, PUT, PATCH, and GET requests, maintaining data synchronization.
- Axios:
  - Axios is a library that simplifies API calls and related configurations.

### Backend:
The backend uses FastAPI and SQLite.

- Swagger:
  - Swagger automates API documentation and makes API testing easier.
- Docker:
  - Docker is used to containerize the server, making it easier to configure the server's responses during frontend development.

## Github Link
- This project was conducted in a private repository and is not publicly available.
