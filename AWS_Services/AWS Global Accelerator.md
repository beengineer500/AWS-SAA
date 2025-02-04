---
tags:
  - AWS
---

#### **정의 및 기능**

- ==AWS 글로벌 네트워크를 활용==하여, 
  ==TCP 및 UDP 기반 애플리케이션의 성능과 가용성을 향상==시키는 서비스이다.
- 전 세계 사용자에게 ==두 개의 고정 공용 IP 주소를 제공==하며, 
  ==사용자의 위치에 따라 최적의 AWS 리전 엔드포인트로 트래픽을 라우팅한다==.
- ==지연 시간을 최소화==하고, ==리전 간 자동 장애 조치==를 지원한다.


#### **사용 사례**
    
- ==글로벌 게임 서비스(예: UDP 기반)==
- ==실시간 통신 애플리케이션(예: VoIP, 화상 회의)==
- IoT 데이터 수집 및 처리

---

#### **주요 차이점 요약 (vs [[Amazon CloudFront]])**

**프로토콜**
- CloudFront
	- ==HTTP/HTTPS==
- Global Accelerator
	-  ==TCP/UDP==

**콘텐츠 캐싱**

- CloudFront
	- ==엣지 로케이션에서 콘텐츠를 캐싱하여 제공==
- Global Accelerator
	- ==캐싱 기능 없음==

**고정 IP 주소**

- CloudFront
	- 고정 IP 주소 없음, 도메인 이름(CNAME)을 통해 접근
- Global Accelerator
	- ==두 개의 고정 공용 IP 주소 제공==

**사용 사례**

- CloudFront
	- 웹 콘텐츠 및 API 가속화, ==정적 및 동적 콘텐츠 제공==
- Global Accelerator
	- 실시간 애플리케이션, 비-HTTP 프로토콜 기반 서비스

