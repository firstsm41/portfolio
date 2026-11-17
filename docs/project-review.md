# 프로젝트 포트폴리오 작성 근거

기준일: 2026-11-17. 기존 PRN·스마트월 문서를 유지하고, 7개 상세 페이지를 추가했습니다.

## 검토한 소스

| 상세 문서 | 확인한 저장소·버전 | 중점 |
|---|---|---|
| [Medicine WMS](../projects/medicine-wms/) | firstsm41/medicine-wms · `715b4bc86a8c` | 회원 JDBC, 승인 로그인, 회원 조회·변경 |
| [CROFLE 화면](../projects/crofle/) | firstsm41/CROFLE_FRONT_NEW · `d24e073cd218`, 팀 최종 프론트엔드의 개인 커밋 | Vue 인증 화면·API·라우트 |
| [전지천 퀴즈](../projects/jeonjicheon-quiz/) | firstsm41/jeonjicheon-quiz · `d23d0ce658eb` | 6문항, 응답 집계, 발표 화면, SQL 정책 |
| [리쥬베리](../projects/rejuberry/) | 비공개 원본 코드의 검토 시점 버전 | 근무표 생성, 개인정보 조회 경계, 마감·정정, 모듈 구성 |
| [모아봄](../projects/moabom/) | 비공개 원본 코드의 검토 시점 버전 | 반복·오프라인 작업, 위젯, 외부 구독 요청, 테스트 |
| [CROFLE 인증 API](../projects/live-crowdfunding-backend/) | firstsm41/Live-CrowdFunding-Backend · `03a6e7f43003`, EdenKwon 버전 `baa7e30053d0` | 공통 계정, JWT·Redis, 소셜·복구 |
| [All Live Young](../projects/all-live-young/) | firstsm41/all-live-young · `e0a123a7daca`, EdenKwon 버전 `b306fba9e175` | 회원·문의·답변·Mapper·트랜잭션 |

프로젝트 소개를 위해 앱을 실행하거나 운영 DB·메일·소셜 인증을 호출하지 않았습니다.
기존 테스트는 구현과 경계 조건을 이해하는 근거로 읽었으며, 이번 문서 변경의 검증은 문서 렌더·링크·기여 근거·공개 내용 확인입니다.

## 요청받은 EdenKwon 저장소 비교

- [EdenKwon/all-live-young](https://github.com/EdenKwon/all-live-young)
- [EdenKwon/Live-CrowdFunding-Backend](https://github.com/EdenKwon/Live-CrowdFunding-Backend)

두 저장소를 각각 본인 포크 main과 Git으로 비교했습니다. 검토한 버전에서는 `src/main/java`의 tree SHA가 각각 같았고, 전체 파일 비교에서도 차이는 README였습니다. 따라서 동일한 애플리케이션 코드에 대한 다른 팀원의 설명을 함께 검토한 것으로 다룹니다.

All Live Young의 EdenKwon README는 입고 기능, CROFLE의 EdenKwon README는 프로젝트 등록·심사·예약 관련 내용을 중심으로 설명합니다. 그 설명·회고·성과를 최성민 개인의 구현이나 성과로 복사하지 않았습니다.

CROFLE 백엔드 README에는 Spring Boot 3.3.4가 적혀 있지만, 검토한 `build.gradle`은 3.3.5이므로 상세 문서에는 코드 기준 버전을 적었습니다.

## 개인 역할 확인

| 프로젝트 | 본인 확인 내용 | 코드·GitHub 교차 확인 |
|---|---|---|
| WMS | 로그인·회원관리 | `sungmin` 작성자와 firstsm41 계정 연결, 회원관리 추가 커밋 |
| All Live Young | 회원관리·고객센터 | `CSM` 작성자와 firstsm41 계정 연결, 회원·문의·답변·공지 변경 |
| CROFLE | AAA · 로그인·프론트엔드 | SungMin CHOI/firstsm41의 인증·복구·소셜 로그인·화면 변경 |

커밋 개수는 기여 크기나 성능 성과로 환산하지 않았습니다. 팀 공통 인증 설정이나 다른 팀원의 입고·재고·예약·결제 기능은 시스템 설명과 개인 담당 범위를 구분했습니다.

## 문서에서 구분한 구현과 한계

- WMS·All Live Young은 학습 프로젝트의 회원 흐름을 설명하고, 저장 방식과 검증의 개선점을 별도로 적었습니다.
- CROFLE 초기 프론트엔드와 최종 팀 저장소를 독립 서비스로 중복 계산하지 않았습니다.
- CROFLE 인증 API는 토큰 흐름을 설명하되, 운영 보안이나 계정 복구의 완전한 E2E 검증을 주장하지 않았습니다.
- 전지천 퀴즈의 문항 데이터는 객관식 5개·주관식 1개였습니다. PIN·결과 공개 UI는 서버 인증으로 설명하지 않았습니다.
- 리쥬베리·모아봄은 비공개 코드의 설계를 요약했습니다. 원본 파일·운영 데이터·인증 정보·실제 사용자의 사진·내부 기준값은 옮기지 않았습니다.
- 기존 PRN·스마트월 문서의 측정 수치를 다른 프로젝트의 성과로 사용하지 않았습니다.
