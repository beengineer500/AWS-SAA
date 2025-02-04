---
tags:
  - AWS
---

#### **정의 및 목적**

- 웹 애플리케이션 및 사이트의 ==SSL/TLS 인증서를 프로비저닝, 관리 및 배포하여 네트워크 트래픽을 암호화하고 보안을 강화==한다.

#### **기능**

- ==SSL/TLS 인증서의 생성, 관리 및 자동 갱신==
- ==Elastic Load Balancing (ELB), Amazon CloudFront, Amazon API Gateway 등과 통합==
- ==퍼블릭 및 프라이빗 인증서 지원==

---


#### 비교 (vs [[AWS Secrets Manager]], [[AWS Key Management System (AWS KMS)]])

**관리 대상**

- **AWS KMS**
	-  ==암호화 키를 생성하고 관리==하여 ==데이터 암호화 및 복호화를 지원==한다.
- **AWS Secrets Manager**
	-  데이터베이스 ==자격 증명, API 키 등 다양한 시크릿 정보==를 ==안전하게 저장하고 관리==한다.
- **AWS Certificate Manager(ACM)**
	-  ==SSL/TLS 인증서를 프로비저닝, 관리 및 배포==하여 ==네트워크 통신을 보호==한다.


**기능**

- **AWS KMS**
	-  데이터 암호화 키의 생성, 관리, 접근 제어 및 감사 기능을 제공한다.
- **AWS Secrets Manager**
	-  시크릿 정보의 저장, 자동 교체, 접근 제어 및 감사 기능을 제공한다.
- **AWS Certificate Manager(ACM)**
	-  SSL/TLS 인증서의 생성, 자동 갱신 및 AWS 서비스와의 통합을 지원한다.


**사용 사례**

- **AWS KMS**
	- ==데이터 암호화 및 복호화==가 필요한 경우
	  (S3 버킷의 데이터 암호화 등)
- **AWS Secrets Manager**
	- ==데이터베이스, 애플리케이션 등과 통합되어 보안 정보를 관리==한다.
	- 애플리케이션에서 데이터베이스 ==자격 증명이나 API 키 등의 시크릿 정보를 안전하게 관리==해야 하는 경우
- **AWS Certificate Manager(ACM)**
	- 주로 ==네트워크 트래픽 암호화==를 위한 서비스와 통합된다.
	- 웹 애플리케이션에 ==SSL/TLS 인증서를 적용하여 HTTPS 통신을 구현==해야 하는 경우