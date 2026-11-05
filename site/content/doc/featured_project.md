---
title: "대표 활동: 개인 포트폴리오 웹사이트 구축"
date: 2026-11-04
draft: false
type: "page"
showFrontMatter: false
---

## 1. 활동 개요

- **활동명**: Hugo와 GitHub Actions를 활용한 반응형 개인 포트폴리오 사이트 제작
- **수행 기간**: 2026년 10월 ~ 2026년 11월
- **진행 상태**: 배포 완료 / 기능 개선·문서화 진행 중
- **수행 형태**: 개인 프로젝트

---

## 2. 활동 목적

- **정적 사이트 아키텍처 실습**: 오픈소스 정적 사이트 생성기(Hugo)의 동작 원리를 이해하고 실제 구동 가능한 사이트 제작.
- **배포 자동화(CI/CD) 파이프라인 경험**: 소스 코드 수정 후 GitHub에 push하면 자동으로 빌드되어 웹에 반영되는 파이프라인 구축.
- **반응형 웹 UI 최적화**: 다양한 화면 해상도에서 안정적으로 동작하도록 CSS를 직접 디버깅하고 커스터마이징.

---

## 3. 수행 과정 및 기술적 의사결정

### ① 오픈소스 테마 분석 및 환경 설정
- Hugo 테마(`SANS`)를 선정하고 저장소 구조 분석.
- `hugo.toml`의 `baseURL`을 GitHub Pages 환경(`https://fragile-creator.github.io/MyWebPage/`)에 맞춰 설정하고 기본 언어를 한국어(`ko`)로 변경.

### ② 오류 해결 및 배포 정상화
- **TOML 문법 오류 해결**: `hugo.toml`의 title 속성값 내 작은따옴표 충돌 문제를 큰따옴표로 수정하여 빌드 실패(Exit code 1) 해결.
- **이미지 경로 규명**: Hugo의 에셋 파이프라인(`assets/`)과 정적 복사 폴더(`static/`)의 차이를 분석하여, 프로필 이미지가 정상 노출되도록 `site/static/images/` 경로로 배치.

### ③ 레이아웃 및 스타일 커스터마이징
- 데스크톱 환경(1440px)에서 본문 `<main>` 영역이 좌측으로 치우쳐 있던 문제를 발견하고, `site/assets/css/main.css`를 생성하여 `margin: auto`를 부여함으로써 중앙 정렬 달성.
- 상단 헤더 메뉴바와 제목 간격 조정을 위해 `.header-nav`에 여백 추가.

---

## 4. 수행 결과물 및 배운 점

### 🔗 결과물 링크
- **배포 사이트**: [https://fragile-creator.github.io/MyWebPage/](https://fragile-creator.github.io/MyWebPage/)
- **GitHub 저장소**: [https://github.com/fragile-creator/MyWebPage](https://github.com/fragile-creator/MyWebPage)

### 💡 배운 점 및 향후 개선 방향
- **배운 점**:
  - 도구의 임시 파일(`.swp` 등)이 협업 저장소에 미치는 영향을 이해하고 `.gitignore` 규칙을 체계화.
  - 빌드 로그와 LLM을교차 검증하며 문제 원인을 추적하는 디버깅 역량 체득.
- **향후 개선 방향**:
  - 계속해서 학습한, 또는 학습할 내용들 정리할 공간 제작.
  - AI에 너무 의존하지 않고  문제사항을 이해하는 능력 배양.

