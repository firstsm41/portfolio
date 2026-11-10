<div align="center">

# 최성민 · 포트폴리오

기획부터 설계, 개발, 배포, 운영까지 직접 맡아 실제 사용자에게 내놓은 프로젝트를 모았습니다.

[![Email](https://img.shields.io/badge/firstsm41@naver.com-03C75A?logo=naver&logoColor=white)](mailto:firstsm41@naver.com)
[![GitHub](https://img.shields.io/badge/github.com/firstsm41-181717?logo=github&logoColor=white)](https://github.com/firstsm41)

</div>

---

## 프로젝트

<table>
<tr>
<td width="42%" valign="top">
<a href="projects/prn/"><img src="projects/prn/images/student.png" alt="PRN 학생 화면" /></a>
</td>
<td valign="top">

### [PRN — 필요할 때 꺼내 쓰는 문제은행](projects/prn/)

외과 시험 문항 1,600여 개를 한 문제씩 풀고, 어디서든 바로 검색하고, 관리자가 검수해 올리는 모바일 문제은행.

- 흩어진 시험 자료(PDF·HTML·캡처)를 파싱해 **draft → 검수 → verified** 파이프라인으로
- 한국어 검색 정규화 — SQL과 브라우저 구현을 **전 유니코드에서 일치**시키는 생성기
- 권한·채점·수정 이력을 **DB(RLS·RPC·트리거)가 지키는** 보안 설계
- 단위·SQL·브라우저 E2E 테스트, 가짜 Supabase 게이트웨이로 키 없이 끝까지 테스트

![Next.js](https://img.shields.io/badge/Next.js_14-000000?logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?logo=supabase&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?logo=vercel&logoColor=white)

`2026.09 – 2026.11` · 개인 프로젝트 · [자세히 보기 →](projects/prn/) · [발표 자료 PDF](projects/prn/PRN-portfolio.pdf)

</td>
</tr>
</table>

<table>
<tr>
<td width="42%" valign="top">
<a href="projects/smartwall/"><img src="projects/smartwall/images/hero.png" alt="스마트월 관리 화면과 TV 화면" /></a>
</td>
<td valign="top">

### [스마트월 — 병원 대기실 TV 9대를 브라우저 하나로](projects/smartwall/)

삼성 세로형 사이니지 TV 에 사진·영상을 돌리고, 전원·예약·상태까지 웹 관리 화면 하나에서 다루는 시스템.

- 클라우드 화면 → **병원 PC 의 localhost 도우미** → 삼성 MDC 로 내부망 TV 를 켜고 끈다 (포트 개방·키 없이)
- 저장 공간 80MB 짜리 TV 브라우저에서 **끊기지 않는 재생** — 받으며 틀기, 멈춘 자리부터 이어 틀기, 스스로 새로 고침
- 올리는 순간 **브라우저(WebCodecs)가 영상을 TV 해상도로 다시 만들고 검증** — 4K 영상 5개 기준 −71%
- TV 가 1분마다 보내는 상태 보고로 **현장 문제를 재현하고 고친** 4일 · PR 28개

![React](https://img.shields.io/badge/React_19-20232A?logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?logo=supabase&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![Samsung](https://img.shields.io/badge/Samsung_MDC-1428A0?logo=samsung&logoColor=white)

`2026.11` · 1인 개발 · [자세히 보기 →](projects/smartwall/) · [발표 자료 PDF](projects/smartwall/SmartWall-portfolio.pdf)

</td>
</tr>
</table>

<!--
다음 프로젝트는 위 <table> 을 복사해 projects/<이름>/ 으로 추가한다.
-->
