# KSY's 첫 포트폴리오 웹사이트

> 2026학년도 초급프로젝트 과제 1: Hugo와 GitHub Actions를 활용한 개인 포트폴리오 웹사이트 구축

- **공개 배포 URL**: [https://fragile-creator.github.io/MyWebPage/](https://fragile-creator.github.io/MyWebPage/)
- **GitHub 저장소**: [https://github.com/fragile-creator/MyWebPage](https://github.com/fragile-creator/MyWebPage)

---

## 📌 프로젝트 소개

Hugo를 기반으로 구축한 개인 소개 및 활동 기록 포트폴리오 웹사이트임.  
GitHub Pages 및 GitHub Actions 기반의 자동 배포 파이프라인 구축, PC·태블릿·모바일에서의 웹 접근성을 고려함.

---

## 🛠️ 개발 및 실행 환경

- **정적 사이트 생성기**: Hugo extended v0.167.0
- **기본 언어**: Python 3.15.2
- **테마**: [Sans Hugo Theme](https://github.com/psugam/sans) (MIT License)
- **실행 환경**: Google Chrome 130.0

### 로컬 실행 및 빌드 명령어

1. 저장소 클론:
   ```bash
   git clone https://github.com/fragile-creator/MyWebPage.git
   cd MyWebPage

## 📜 출처 및 라이선스 고지

### 1. 원본 오픈소스 테마 정보
- **테마명**: Sans Hugo Theme
- **원본 저장소**: [https://github.com/psugam/sans](https://github.com/psugam/sans)
- **원저작자**: Sugam Pokharel
- **라이선스**: MIT License

### 2. 사용 이미지 출처
- **이미지 원작자**: [https://x.com/sa_nal__](https://x.com/sa_nal__) (@sa_nal__)

### 3. 저작 및 기여 구분
- **본인 직접 작성 및 수정**:
  - 자기소개(`site/content/pages/about.md`) 및 학습 목표·관심 분야(`site/content/doc/Interests_and_Goals.md`) 콘텐츠 작성
  - 대표 활동(`site/content/doc/featured_project.md`) 프로젝트 개요, 수행 과정, 결과 분석
  - 레이아웃 중앙 정렬, 표 가독성 개선, 메뉴 여백 등 css 커스터마이징
- **AI(어시스턴트) 협업 및 활용**:
  - `hugo.toml` 및 `_index.md`의 TOML 문법 오류 디버깅
  - 목차 소제목 앵커 링크 ID 매핑 자문
  - 마크다운 표 숙련도 열 줄바꿈 방지(`white-space: nowrap`) CSS 조언
  - 그 외 많은 조언과 도움을 받음(Thanks for Google & Anthropic!)
