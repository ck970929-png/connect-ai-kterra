# 💻 코다리 (시니어 풀스택 엔지니어) 개인 메모리

_코다리 에이전트만 읽고 쓰는 개인 노트. 학습·교훈·자주 쓰는 패턴이 누적됩니다._

## 학습 기록

- [2026-05-28] PICTO LAB의 핵심 기술 스택과 개발 환경을 최종 확정하고, Mock-up 단계에서 넘어온 API Spec Mockup을 기반으로 실제 개발에 필요한 초기 프로젝트 구조(폴더링, 필수 라이브러리, 기본 설정 파일)를 설계하고 Git 저장소 초기화 작업을 진행하세요. 백엔드/프론트엔드 분리 구조를 명확히 하고, 개발자 자신을 위한 테스트 코드를 포함하여 최소한의 코드를 작성해야 합니다. → 산출물 sessions/2026-05-28T11-50/developer.md
- [2026-05-28] 최신 의사결정 로그(테스트 시나리오, API 매트릭스)를 기반으로, PICTO LAB MVP의 'Mock Backend API' 구축에 착수하세요. 백엔드(FastAPI/Python)의 필수 엔드포인트 3가지(`search`, `get_svg`, `get_style_sheet`)에 대한 기본 구조와 더미(Dummy) 데이터를 포함한 Mock-up 코드를 작성하고, Git 저장소에 커밋하여 공유하세요. 이는 프론트엔드 개발을 위한 기술적 기반이 됩니다. → 산출물 sessions/2026-05-28T12-50/developer.md
- [2026-05-28] 디자이너가 정의한 MVP 화면 구조를 기반으로 웹 서비스 구현에 필요한 컴포넌트 구조, 파일 구성, 그리고 핵심 SVG 생성 로직의 초안을 설계하세요. → 산출물 sessions/2026-05-28T13-50/developer.md
- [2026-05-28] PICTO LAB의 MVP 웹 애플리케이션 구현을 시작합니다. src/app/page.tsx, src/components/InputPanel.tsx, src/components/ResultPanel.tsx, src/lib/svg-renderer.ts, src/lib/style-manager.ts, src/lib/download.ts 파일을 정의하고, 명시된 MVP 기능(키워드 입력, 용도 선택, 스타일 선택, 후보 4개 SVG 표시, SVG/PNG 다운로드)을 구현하세요. 외부 AI API 사용을 배제하고, 파일 구조와 컴포넌트 분