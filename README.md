# TTS-App
Text to Speech Project for Spring Boot and Kotlin, Auth Server, Python with Fast API (gTTS)

Python의 gTTS lib를 활용하여 텍스트를 음성으로 변환하는 서비스를 구현해봅니다.

<br/>

## 프로젝트 구조
---
- 추가, 변경 가능
<p align="center">
  <img src="https://user-images.githubusercontent.com/67903919/140641098-2d97d191-654c-42d3-8c72-631f44d8c750.png" width="85%">
</p>

<br/>

## 프로젝트 개발 요구 사항 정의
---

### 서버 구조
- User API, Auth, TTS Server, MySQL, Prometeus + Grafana 는 같은 Host System에 Docker Container 형태로 배포되어야 한다. (Docker File, Compose 활용)
- 배포 시에는 Docker File, Docker Compose를 활용하여야 한다.

### 파일 관리
- Text File Upload 혹은 사용자가 Text 작성하였을 때에는 내용의 무결성 검증을 진행하여야 한다.
- Host File System을 활용하여 File에 대해 Persist, Download(Download Page 제공), Select, Delete(Scheduler) 기능을 작성해야 한다.
- File Multiple download 시 확장자가 아니라 Zip에 압축하여 제공하여야 한다.

<br/>

## 프로젝트 개발 시 준수 사항
---

### Convention
- 명시적인 Naming Convention 준수
- Encapsulation 을 지킬 수 있는 원칙들을 준수
- 좋은 커밋 메시지를 위해 Git commit 규칙을 준수 https://blog.ull.im/engineering/2019/03/10/logs-on-git.html

<br/>

### Work Flow
- Git Branch Strategy "**Git-Flow**" 

<p align="center">
  <img src="https://user-images.githubusercontent.com/67903919/103394069-98138f00-4b69-11eb-925e-d79966b3f716.png" width="80%">
</p>

<br/>

### Tech Stack 
+ Spring Boot 2.5.6 + Kotlin
+ Spring Actuator + Admin + Security + Resource Server + Authorization Server
+ Python + Fast API + gTTS
+ React + TypeScript + React-Router-Dom + Material-UI
+ Testcontainers (redis, mysql..) + MySQL + Data JPA, QueryDSL
+ Prometheus + Grafana
+ Docker Compose + Docker


### 당연한 결과입니다!
