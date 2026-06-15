<!--

Spring JPA Hibernate
JQuery
JUnit
JWT
Gradle
Sonarcube
Jira

- 뱃지 사이트 참고 (최신 기술용)
https://github.com/Ileriayo/markdown-badges
-->




<!--
## Hi there 👋

**look516/look516** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->





### 안녕하세요, 함께 고민하고 싶은 백엔드 개발자 조아영입니다.
아직 배워가는 단계이지만<br>
열린 마음으로 서로의 코드를 나누며,<br>
내일은 조금 더 성장한 서비스를 만들어 가보고 싶습니다.
<br><br>

## 🛠 Tech Stack

**AI**<br>
![Claude](https://img.shields.io/badge/Claude-D97757?style=flat&logo=claude&logoColor=white)

**Skills**<br>
![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=flat&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=spring-boot&logoColor=white)
![Kafka](https://img.shields.io/badge/Apache_Kafka-231F20?style=flat&logo=apache-kafka&logoColor=white)

<!-- English / Chinese -->

**DB**<br>
![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=flat&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)

**Environment**<br>
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=flat&logo=github&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)

**Communication/Docs**<br>
![Notion](https://img.shields.io/badge/Notion-%23000000.svg?style=flat&logo=notion&logoColor=white)
![Slack](https://img.shields.io/badge/Slack-4A154B?style=flat&logo=slack&logoColor=white)
![Swagger](https://img.shields.io/badge/-Swagger-%23Clojure?style=flat&logo=swagger&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat&logo=postman&logoColor=white)

<!-- ![Drawio](https://img.shields.io/badge/drawio-%23F08705?style=for-the-badge&logo=diagrams.net&logoColor=white) -->


<!--
## 🚀 관심 도메인
동기화 · 자동화 · 티켓팅 · 스트리밍 · 채팅 플랫폼 백엔드
-->
<!--
- 대용량 트래픽 처리 (Redis Sorted Set 대기열, Lua 분산락)
- MSA / Kafka 이벤트 기반 아키텍처
- 동시성 제어 & SAGA 패턴
- AI Native
-->
<br>

## 📌 Project
<!-- | 프로젝트 | 설명 | 담당 도메인 | 기술 | 기간 | 트러블슈팅 | -->

### [sparta-logistics](https://github.com/swissmissed2/sparta-logistics/tree/dev)
- **기간**: 2026/05/14~2026/05/31 (약 2주)
- **설명**: 주문 생성부터 배송 완료까지의 흐름을 Kafka 기반의 오케스트레이션/코레오그라피 Saga 패턴으로 처리하는 Spring Boot MSA 물류 관리 플랫폼 프로젝트입니다.
- **핵심 설계**: MSA(배포 환경 대비), EDA(with Kafka), Saga Pattern, feign 통신
  <br>분산 트랜잭션, 서킷 브레이커, 동시성 제어, Zipkin 분산 추적
- **목표**:<br>
동시성 제어를 통한 데이터 **정합성** 보장,
<br>그리고 재시도 로직에서의 **멱등성** 확보 사이에서
<br> 균형있게 최적화하는 문제에 집중

#### Delivery-service(담당 도메인) 특징
1. JUnit5 & Mockito를 활용한 **테스트 코드 설계**<br>
   Claude-AI로 복잡한 비즈니스 로직의 테스트 케이스를 빠르게 설계하여 단위 테스트 진행
<br>

2. **상태 전이 캡슐화**<br>
배송 경로의 상태 변화(WAITING → IN_TRANSIT → ARRIVED)를 엔티티 내부의 도메인 메서드에서만 제어하도록 구현하여, 외부에서 비정상적인 상태 변경이 불가능하도록 차단
<br>

3. **이중 동시성 제어** (배송 담당자 배정)<br>
PESSIMISTIC_WRITE (비관적 락)로 중복 배정 시나리오를 방지하고, JPA @Version 기반의 낙관적 락을 병행하여 시스템 처리량과 무결성 간의 균형 확보
<br>

4. **복원력**(Resilience) 설계<br>
배송 담당자 배정 실패 시 Scheduler를 통한 재시도 로직을 구현하여, 이벤트 기반 시스템에서의 데이터 누락 방지 및 서비스 안정성 강화
<br>


<!--
## 📊 GitHub Stats
![Stats](https://github-readme-stats.vercel.app/api?username={look516}&show_icons=true&theme=default)
-->

## 📫 Contact
[![Velog](https://img.shields.io/badge/Velog-20C997?style=flat&logo=velog&logoColor=white)](https://velog.io/@iicarus)
[![Gmail](https://img.shields.io/badge/Gmail-caybnow@gmail.com-D14836?style=flat&logo=gmail&logoColor=white)](mailto:caybnow@gmail.com)
<!-- [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](정비중) -->
