# CPR Response Plus

CPR 교육/응급 대응 안내용 정적 웹사이트입니다.

## 파일 구조

```text
.
├── index.html
└── assets
    ├── css
    │   └── style.css
    └── images
        ├── hero-heart.png
        ├── heartbeat.png
        ├── protocol-steps.png
        ├── step-01.png
        ├── step-02.png
        ├── step-03.png
        ├── step-04.png
        ├── training-map.png
        ├── logo-symbol.png
        └── main-logo.png
```

제작 과정 & 수정 히스토리
v0.1 — 초기 구축 (2026-05-03)
커밋: Add CPR response landing page

프로젝트 최초 생성
index.html 기본 구조 작성 (Hero / Overview / Process / Pulse / CTA / Footer 섹션)
assets/css/style.css 스타일 전체 초안 작성 (1,500줄+)
이미지 에셋 추가:
hero-heart.png — 히어로 섹션 메인 이미지
heartbeat.png — 심박 아이콘
step-01~04.png — CPR 4단계 프로세스 아이콘
training-map.png — 교육센터 위치 지도
logo-symbol.png, main-logo.png — 로고
v0.2 — 캠페인 랜딩 페이지 개선 (2026-05-06)
커밋: Update CPR campaign landing page → PR #1 병합

전체 레이아웃 및 섹션 구성 전면 재작업
protocol-steps.png 이미지 추가 (CPR 프로토콜 스텝 통합 이미지)
CSS 대규모 리팩토링: 기존 대비 +1,040줄 순증가
HTML 마크업 재구성: 섹션 콘텐츠 및 카피 업데이트
v0.3 — 디자인 정제 (2026-06-01)
커밋: Design refinements: layout, typography, scroll snap, and animations

수정/개선 내용
항목	내용
스크롤 스냅	페이지 단위 스크롤 스냅(proximity) 적용
섹션 높이 버그 수정	고정 헤더(74px) 아래 섹션이 잘리던 문제 → calc(100svh - 74px)로 정확한 센터링
타이포그래피	eyebrow 텍스트 굵기 감소, 메인 타이틀과 간격 조정
Process 섹션	이미지 크기 확대, 컬럼 폭 통일, 단계 텍스트 계층 정리
Pulse 섹션	중앙 정렬 2열 레이아웃으로 변경, 여백 균형 조정
지도 애니메이션	mapPulse 위치를 실제 CPR 교육센터 핀 위치에 맞게 재조정
텍스트 색상	overview-command, process subtitle 등 전반적 텍스트 밝기 조정
푸터	멀티 컬럼 레이아웃으로 확장, 응급 정보 영역 스타일링
v0.4 — 헤더 적응형 테마 (2026-06-01)
커밋: Add adaptive header theme and logo shadow

버그 수정 및 기능 추가
항목	내용
헤더 테마 자동 전환	스크롤 위치에 따라 헤더가 라이트/다크 모드 자동 전환
라이트 섹션	overview, process, training — 크림색 헤더 + 다크 네비
다크 섹션	hero, pulse, cta-band — 다크 헤더 + 흰색 네비
로고 가시성 버그 수정	밝은 배경에서 로고가 보이지 않던 문제 → 로고에 드롭 섀도 추가
헤더 하단 선 제거	불필요한 border-bottom 라인 삭제
v0.5 — 캠페인 배경 이미지 (2026-06-01)
커밋: Add campaign background image

수정/개선 내용
항목	내용
배경 이미지 추가	campaign-message-bg.png 신규 추가 (약 1.3MB)
CSS 배경 처리	캠페인 메시지 섹션에 배경 이미지 적용, 오버레이 스타일링
HTML 섹션 수정	캠페인 섹션 마크업 및 클래스 정리
