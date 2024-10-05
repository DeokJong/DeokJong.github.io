---
title: 'Jeonbuk National University Capstone Project'

authors:
  - admin

date: '2013-07-01T00:00:00Z'
doi: ''

publishDate: '2017-01-01T00:00:00Z'

# Summary
summary: This project was developed during the 2024 Capstone Project for the first semester at Jeonbuk National University. It is a project focused on creating a multi-monitoring system.

tags:
  - React
  - Capstone

share: false
featured: true

image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
  focal_point: ''
  preview_only: false
---

# Multi-PC Environment Monitoring and Remote Chat Technology
- This project was created for the 2024 Capstone Project at Jeonbuk National University.

## Introduction
The company that requested this project was facing the following issues:

The company manages POS systems across several stores. The inquiries from the stores usually state a general problem like, "The POS system is not working properly." Since the store employees cannot identify the exact cause of the problem, they provide vague feedback. As a result, the company ends up investing a significant amount of human resources to determine the cause of the issue.

Thus, the company required a new program to gather information about the POS system and capture screenshots to quickly identify the problem on the store's end.

## Project Breakdown
To address this, we divided the project into the following roles:

1. A client that collects data from the POS system, receives commands, and periodically sends the collected data to the server.
2. An admin page to view the client information stored on the server and send commands to the client.
3. A server that stores client data and relays the administrator's commands.

## Flowchart
- In summary, this project is divided into three subprojects:
  - `Web Browser (admin-page)`
  - `Server (backend)`
  - `Client (collector)`
- For more information on each subproject, please refer to the `README` in the subfolders.
- The overall flowchart of this project is illustrated below:
![Server Activity Diagram](https://github.com/jbnu-capstone-jjinjjin/project/assets/129056857/dcfe1e79-135a-4316-85b8-6460183b8144)
![Daemon Activity Diagram](https://github.com/jbnu-capstone-jjinjjin/project/assets/129056857/2d3cbbe6-8c1f-4c5a-a807-8619b35b5f71)

## Feature Summary
- Web Browser (admin-page)
 1. Retrieves the HW information, SDK information, and RESOURCE information of the client.
 2. Obtains the PID of the programs running on the client based on the RESOURCE information and forcibly terminates those programs using the PID.
 3. Captures and views the current screen of the client.
- Server (backend)
 1. Stores the HW information, SDK information, and RESOURCE information of the client.
 2. Stores the screenshots sent by the client.
 3. Delivers commands from the admin-page to the client.
 4. Provides the admin-page with client information for viewing.
- Client (collector)
 1. Collects and sends the HW information, SDK information, and RESOURCE information of the installed device to the server. The RESOURCE information is sent at user-defined intervals (default is every 5 minutes).
 2. Terminates the program when receiving the PID from the server and then updates and sends the RESOURCE information to the server again.
 3. Captures and sends a screenshot to the server upon receiving a command from the server.

## Role

In this project, I was responsible for implementing the collector.

## Github Link
[Capstone Project](https://github.com/jbnu-capstone-jjinjjin/project)
