---
tags:
  - AWS
---

#### API Gateway
- REST API 및 Websocket API 를 생성/유지/관리하는 AWS 서비스
- Lambda, AWS Service, VPC, HTTP webpage 등과 연동하여 Resource 에 대한 HTTP Method 정의 가능
- ==API Gateway 와 Lambda 를 연동하여 사용하기 용이==하다.
	- ==User -> API Gateway -> Lambda==
- ==고객이 애플리케이션 개발만을 집중==하고, ==인프라는 AWS 에게 분담==하고자 할 경우,
  API Gateway - Lambda 는 유용하게 사용 가능