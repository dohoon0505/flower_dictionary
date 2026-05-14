# 꽃배달 창업 백과사전 · Flower Startup Encyclopedia

> 꽃배달 창업을 처음부터 끝까지 안내하는 실전 가이드북.
> **현재 버전 v1.0.0**

---

## 이 프로젝트는

시장 분석부터 상품 구성, 공급망, 채널 운영, 마케팅, 배송 운영, 재무·법규까지 — 꽃배달로 사업을 시작하려는 사람에게 필요한 모든 단계를 한 권의 가이드북으로 정리합니다.

| 대상 | 진입점 | 특징 |
| --- | --- | --- |
| 사람 | `index.html` | 브라우저에서 열면 바로 가이드북 |
| AI 에이전트 | [`AGENTS.md`](AGENTS.md) + [`system.json`](system.json) | 1–2 파일 read로 모든 쿼리 해결 |
| 기여자 | [`CLAUDE.md`](CLAUDE.md) | 3계층 작업 원칙 · 수정 워크플로 |

---

## 빠른 시작

```bash
start index.html         # Windows
open index.html          # macOS
```

외부 서버 불필요. 이 한 파일이 전체 사이트입니다.

GitHub Pages 배포 후에는 다음 URL로 접속할 수 있습니다.
**https://dohoon0505.github.io/flower_dictionary/**

---

## 8개 챕터 구성

| # | 챕터 | 다루는 내용 |
|---|------|----------|
| 01 | 시작하기 | 시장 구조, 사업 형태, 자격·신고 |
| 02 | 시장 분석 & 컨셉 설정 | 타겟·경쟁사·USP·브랜드 톤 |
| 03 | 상품 구성 & 가격 정책 | 카테고리·시즌·원가 기반 가격 |
| 04 | 공급망 & 재고 관리 | 도매시장·산지·자재·재고 회전 |
| 05 | 판매 채널 운영 | 오프라인·자사몰·플랫폼 |
| 06 | 마케팅 & 고객 확보 | SNS·검색광고·리뷰·단골 |
| 07 | 주문 · 배송 운영 | 접수→제작→배송→CS SOP |
| 08 | 재무 · 법규 · 세무 | 손익분기·세무·인허가 |

각 챕터는 학습 목표 + 여러 아티클로 구성됩니다.

---

## 폴더 구조

```
flower_dictionary/
├── index.html                  ← 운영 진본 (단일 진입점)
├── assets/
│   ├── css/main.css
│   └── js/main.js
│
├── system.json                 ← 루트 매니페스트 (챕터 + 릴리즈)
├── analyses/                   ← 챕터 콘텐츠 데이터
│   └── {chapter-id}/chapter.json
│
├── scripts/validate.mjs        ← 무결성 검증
├── AGENTS.md                   ← AI 에이전트 진입점
├── CLAUDE.md                   ← 기여 가이드라인
└── README.md                   ← 이 파일
```

---

## 릴리즈 노트

버전별 변경 내역은 `#changelog` 라우트에서 확인하거나, `system.json.releases[]` 배열을 직접 참고하세요.

---

## 기여

1. [CLAUDE.md](CLAUDE.md) 의 3계층 작업 원칙 준수
2. 수정 후 `node scripts/validate.mjs` 실행
3. `index.html`을 브라우저에서 열어 라이트/다크 모드 확인

---

## 라이선스

운영 관리: **/DH** · 2026 · MIT
