---
title:  "IT 용어 part1"
date:   2022-08-02
categories: [Tech]
tags: [Tech]
---

## Web 1.0, 2.0, 3.0

### 읽기 전용인 Web 1.0     
- 소수의 사람만 컨텐츠 창작
- 댓글을 남기거나 코맨트를 남기는 등의 상호작용은 불가능
### 쓰기 기능이 추가된(상호작용이 가능한) Web 2.0       
- 요즘 말하는 웹이 Web 2.0
- 초창기 모델이 블로그, 다이어리등
- 인스타나 페이스북 등의 SNS 역시 Web 2.0
### 탈중앙화와 AI를 활용한 사용자 맞춤형 Web 3.0
- 서버-클라이언트 구조 탈피 (탈중앙화)      
  -> 사용자들이 생성한 컨텐츠들의 대부분 특정 플랫폼에 속해 있음 (영상의 경우 유투브)       
  이 경우 유투브 서버에 동영상 컨텐츠가 저장되고 사용자(클라이언트)는 해당 서버에서만 데이터를 얻을 수 있음     
  이 같은 구조를 탈피하고자하는게 Web 3.0
- 맞춤형        
  -> 방대한 데이터에서 실제 사용자에게 필요한 정보만을 제공해주기 위함
- Web 3.0은 2D가 아닌 그 이상의 디지털 공간이 될 것이라 예상하는 사람도 많음

<br>

## 웹서버/WAS(Web Application Server)
### 정의: 
클라이언트의 요청을 받아들여 그에 맞는 결과를 전달해주는 프로그램       
웹 서버 : HTTP요청을 받아 HTML, CSS, 자바스크립트, 이미지 등 정적 파일을 제공       
WAS : DB조회나 다양한 로직처리를 필요로하는 동적 콘텐츠 제공
### 대표적인 웹 서버 / WAS:
웹 서버 : Apache, NginX, Microsoft IIS 등
WAS : Tomcat, JBoss, Jeus, Web Sphere 등        
<img src="../images/post/webserver-vs-was.png" width="500px" height="200px" title="Web vs Was">



