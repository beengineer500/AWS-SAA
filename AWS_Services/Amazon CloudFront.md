---
tags:
  - AWS
---

#### **정의 및 기능**

- ==콘텐츠 전송 네트워크(Content Delivery Network) 서비스==이다.
- ==전 세계에 분산된 엣지 로케이션==을 통해 ==정적 및 동적 웹 콘텐츠를 사용자에게 빠르게 전달==한다.
	- ==콘텐츠를 빠르게 배포하기 위한 서비스==이지,
	  콘텐츠 업로드/다운로드 속도를 빠르게 하는 서비스가 아니다.
- ==주로 HTTP/HTTPS 프로토콜을 사용==하며, 
  ==이미지, 비디오 등의 캐시 가능한 콘텐츠==와 API 응답 등의 ==동적 콘텐츠==의 ==성능을 향상==시킨다.


#### **사용 사례**

- ==웹사이트의 정적 콘텐츠 제공==
	- e.g.) 이미지, CSS, JavaScript 파일 등
- ==동영상 스트리밍 서비스==
- API 엔드포인트 가속화


----

## 주요 차이점 요약 (vs [[AWS Global Accelerator]])

#### 프로토콜

- CloudFront
	- ==HTTP/HTTPS==
- Global Accelerator
	- ==TCP/UDP==


#### 콘텐츠 캐싱

- CloudFront
	- 엣지 로케이션에서 ==콘텐츠를 캐싱==하여 제공
- Global Accelerator
	- ==캐싱 기능 없음==


#### 고정 IP 주소

- CloudFront
	- 고정 IP 주소 없음, ==도메인 이름(CNAME)을 통해 접근==
- Global Accelerator
	- ==두 개의 고정 공용 IP 주소 제공==


#### 사용 사례

- CloudFront
	- 웹 ==콘텐츠 및 API 가속화, 정적 및 동적 콘텐츠 제공==
- Global Accelerator
	- ==실시간 애플리케이션==, 비-HTTP 프로토콜 기반 서비스