# 💻 코다리 (시니어 풀스택 엔지니어) 개인 메모리

_코다리 에이전트만 읽고 쓰는 개인 노트. 학습·교훈·자주 쓰는 패턴이 누적됩니다._

## 학습 기록

- [2026-05-28] PICTO LAB의 핵심 기술 스택과 개발 환경을 최종 확정하고, Mock-up 단계에서 넘어온 API Spec Mockup을 기반으로 실제 개발에 필요한 초기 프로젝트 구조(폴더링, 필수 라이브러리, 기본 설정 파일)를 설계하고 Git 저장소 초기화 작업을 진행하세요. 백엔드/프론트엔드 분리 구조를 명확히 하고, 개발자 자신을 위한 테스트 코드를 포함하여 최소한의 코드를 작성해야 합니다. → 산출물 sessions/2026-05-28T11-50/developer.md
- [2026-05-28] 최신 의사결정 로그(테스트 시나리오, API 매트릭스)를 기반으로, PICTO LAB MVP의 'Mock Backend API' 구축에 착수하세요. 백엔드(FastAPI/Python)의 필수 엔드포인트 3가지(`search`, `get_svg`, `get_style_sheet`)에 대한 기본 구조와 더미(Dummy) 데이터를 포함한 Mock-up 코드를 작성하고, Git 저장소에 커밋하여 공유하세요. 이는 프론트엔드 개발을 위한 기술적 기반이 됩니다. → 산출물 sessions/2026-05-28T12-50/developer.md
- [2026-05-28] 디자이너가 정의한 MVP 화면 구조를 기반으로 웹 서비스 구현에 필요한 컴포넌트 구조, 파일 구성, 그리고 핵심 SVG 생성 로직의 초안을 설계하세요. → 산출물 sessions/2026-05-28T13-50/developer.md
- [2026-05-28] PICTO LAB의 MVP 웹 애플리케이션 구현을 시작합니다. src/app/page.tsx, src/components/InputPanel.tsx, src/components/ResultPanel.tsx, src/lib/svg-renderer.ts, src/lib/style-manager.ts, src/lib/download.ts 파일을 정의하고, 명시된 MVP 기능(키워드 입력, 용도 선택, 스타일 선택, 후보 4개 SVG 표시, SVG/PNG 다운로드)을 구현하세요. 외부 AI API 사용을 배제하고, 파일 구조와 컴포넌트 분
- [2026-05-28] PICTO LAB의 MVP 기능을 구현하기 위한 전 과정(src/app/page.tsx, src/components/InputPanel.tsx, src/components/ResultPanel.tsx, src/lib/svg-renderer.ts, src/lib/style-manager.ts, src/lib/download.ts)에 걸친 전체적인 파일 구조 및 로직을 작성하고, 실제 코드를 수정하는 것을 시뮬레이션하세요. 이 과정에서 외부 AI API 호출은 절대 사용하지 않고, 모든 로직은 클라이언트 측(React/TypeScrip
- [2026-05-28] src/lib/svg-renderer.ts를 완전한 TypeScript 코드로 재구성하여 generateSvgCandidates가 keyword, purpose, style 기반으로 4개의 SVG 문자열을 반환하도록 수정하세요. 기존 코드에서 발견된 깨진 문자열(="num"> 등)을 전 코드 범위에서 제거합니다. → 산출물 sessions/2026-05-28T15-47/developer.md
- [2026-05-28] src/app/page.tsx에서 generateSvgCandidates를 import해 키워드/용도/스타일 기반으로 4개의 SVG 후보를 상태에 저장하는 로직 구현하세요. → 산출물 sessions/2026-05-28T15-51/developer.md
- [2026-05-28] src/lib/svg-renderer.ts에서 자기 import 제거하고, generateSvgCandidates 함수를 export function으로 작성해 키워드, 용도, 스타일을 반영한 4개의 SVG 문자열 반환하도록 수정하세요. → 산출물 sessions/2026-05-28T15-51/developer.md
- [2026-05-28] src/lib/download.ts에서 downloadSvg(svg: string, fileName: string): void와 downloadPng(svg: string, fileName: string): Promise 시그니처 구현해, SVG 문자열을 Blob URL로 로드 후 canvas에 그린 뒤 PNG로 다운로드하는 로직 추가하세요. → 산출물 sessions/2026-05-28T15-51/developer.md
- [2026-05-28] src/components/ResultPanel.tsx에서 index 대신 실제 SVG 문자열을 downloadSvg/downloadPng에 전달하도록 수정하고, PNG 다운로드 시 SVG to PNG 변환 로직을 포함해야 합니다. → 산출물 sessions/2026-05-28T15-51/developer.md
- [2026-05-28] 모든 수정 파일에서 "num">, "kw">, span 같은 깨진 문자열을 완전히 제거하고, src/lib/style-manager.ts에서 불필요한 import 제거해 코드 정리하세요. → 산출물 sessions/2026-05-28T15-51/developer.md
- [2026-05-28] npm run build 실행 후 발생한 에러 로그 원문을 그대로 기록하고, 수정된 파일 경로와 내용을 정리해 보고서에 포함하세요. → 산출물 sessions/2026-05-28T15-51/developer.md
- [2026-05-28] package.json, next.config.js, src/app/page.tsx 등 9개 파일 원문 그대로 제공. 깨진 문자열, 프레임워크 구분, 다운로드 기능 구현 여부를 포함한 정확한 파일 내용을 보여줘. → 산출물 sessions/2026-05-28T16-00/developer.md
- [2026-05-28] 리서처가 설계한 추천 규칙을 반영한 SVG 생성 로직 수정 작업을 진행해주세요. 사용자 선호 데이터를 DB에 저장하고, 추천 시스템과 연동하는 API 엔드포인트를 추가해야 합니다. → 산출물 sessions/2026-05-28T16-00/developer.md
- [2026-05-28] AI_DEVELOPMENT_GUIDELINE.md에 명시된 코드 스타일, API 연동 규칙, 파일 구조, 버전 관리 정책을 기반으로 프로젝트 초기화 스크립트와 .gitignore, .env.example 파일을 생성하세요. → 산출물 sessions/2026-05-28T16-17/developer.md
- [2026-05-28] 리서처가 분석한 데이터를 바탕으로 PICTO LAB 추천 로직의 기술적 구현 방안을 제안하세요. SVG 생성 로직과의 통합, 사용자 선택 데이터 저장 구조, 실시간 추천 프로토타입 개발을 포함해야 합니다. → 산출물 sessions/2026-05-28T16-30/developer.md
- [2026-05-28] researcher가 제안한 추천 규칙을 기반으로, SVG 생성 로직에 새로운 유사도 계산 모듈을 통합하는 코드 구현 계획을 세우고, git commit 메시지 구조를 안내해주세요. → 산출물 sessions/2026-05-28T16-59/developer.md
- [2026-05-28] 리서처가 제안한 추천 규칙을 기반으로 SVG 생성 로직에 데이터 기반 필터링 기능을 추가하세요. 사용자 선호도에 따른 스타일 가중치 계산 로직을 구현해 주세요. → 산출물 sessions/2026-05-28T19-32/developer.md
- [2026-05-28] 실제 코드에서 확인해야 할 주요 파일과 수정 주의사항을 정리해주세요. .env.local 파일은 외부 공유/업로드 시 제외해야 한다고 명시하고, 코드 수정 시 에러 가능성 있는 부분을 사전에 지적해주세요. → 산출물 sessions/2026-05-28T19-52/developer.md
- [2026-05-28] 디자이너가 제안한 추천 시스템 흐름을 기반으로 SVG 생성 로직에 데이터 기반 스타일 변환 알고리즘을 통합하세요. 사용자 선호 데이터를 저장하고 추천 결과를 동적으로 업데이트하는 API 엔드포인트를 구현해야 합니다. → 산출물 sessions/2026-05-28T20-40/developer.md
- [2026-05-28] 리서처가 제안한 추천 규칙을 기반으로 SVG 생성 로직에 동적 권장 알고리즘을 통합하는 코드 구조를 설계하세요. → 산출물 sessions/2026-05-28T21-10/developer.md
- [2026-05-28] 리서처가 분석한 선호 규칙을 기반으로 SVG 생성 로직에 추천 알고리즘을 통합하는 코드 구현을 시작하세요. → 산출물 sessions/2026-05-28T21-25/developer.md
- [2026-05-28] src/utils/api.js에 동적 스타일 추천 로직 구현 → 산출물 sessions/2026-05-28T21-55/developer.md
- [2026-05-28] 연구자에게 제공된 선호도 규칙을 기반으로 SVG 생성 로직에 추천 알고리즘을 통합하세요. 사용자 세션별 스타일 변동을 감지하는 감지 로직도 추가해야 합니다. → 산출물 sessions/2026-05-28T23-10/developer.md
- [2026-05-29] 다음 마일스톤을 기술해 주세요. 예상되는 기능 추가, 테스트 단계, 배포 준비 일정을 포함한 구체적인 계획을 제안해 주세요. → 산출물 sessions/2026-05-29T00-37/developer.md
- [2026-05-29] 리서처가 제시한 분석 결과를 바탕으로, 법규 데이터와 사용자 선호 패턴을 결합한 추천 로직 구현을 위한 API 연동 및 파일 구조 설계를 진행하세요. → 산출물 sessions/2026-05-29T00-55/developer.md
- [2026-05-29] 리서처가 정리한 데이터 기반 추천 로직을 기반으로 SVG 생성 로직에 통합 가능한 모듈을 개발하세요. 사용자 선호도에 따른 가중치 적용 방식을 구현해 주세요. → 산출물 sessions/2026-05-29T01-10/developer.md
- [2026-05-29] PICTO LAB MVP의 테스트 환경을 구성하고, 단어 입력창, 스타일 선택 메뉴, 결과 출력 영역, SVG/PNG 다운로드 버튼을 포함한 임시 링크를 생성해 주세요. 로컬 서버에서 테스트 가능한 주소를 제공해야 합니다. → 산출물 sessions/2026-05-29T01-11/developer.md
- [2026-05-29] 현재 웹사이트 UI/UX 구조를 분석해 복잡 요소를 식별하고, 모듈화/레이아웃 최소화를 통한 사용자 경험 개선 방안을 제안하세요. 다국어 지원을 위한 언어 모델 구현 기술적 로드맵도 함께 정리해주세요. → 산출물 sessions/2026-05-29T01-25/developer.md
- [2026-05-29] PICTO_LAB_FINAL_SPEC.md의 기술 구현 부분에 HANDOVER_KTERRA.md의 API 연동 방안, 파일 관리 규칙, 자동화 도구 개발 로직을 추가하세요. 디자이너의 스타일 규칙을 기반으로 SVG 생성 로직 구체화와 프론트엔드·백엔드 연동 방안을 명시적으로 기술합니다. → 산출물 sessions/2026-05-29T01-39/developer.md
- [2026-05-29] 컬러 시스템 #2A3B5A를 프론트엔드 코드에 적용하고, SVG 생성 로직과 연동된 다운로드 버튼 기능을 구현하세요. 버튼 클릭 시 PNG/SVG 파일 생성 및 다운로드 처리 로직을 포함해야 합니다. → 산출물 sessions/2026-05-29T02-06/developer.md
- [2026-05-29] 리서처가 정리한 추천 규칙을 바탕으로 SVG 생성 로직에 추천 알고리즘을 통합해보세요. 사용자 선호도에 따른 동적 스타일 적용 기능을 구현 가능한 구조로 설계해주세요. → 산출물 sessions/2026-05-29T02-12/developer.md
- [2026-05-29] 리서처가 제안한 추천 로직을 기반으로 SVG 생성 알고리즘에 사용자 선호도 가중치를 반영하는 코드 수정을 진행하고, A/B 테스트 환경 구성을 제안하세요. → 산출물 sessions/2026-05-29T02-42/developer.md
- [2026-05-29] 디자이너가 만든 벡터 데이터를 기반으로 SVG 코드를 자동 생성해 주세요. stroke-width, stroke-color, path 데이터 등을 정확히 반영한 깔끔한 SVG 파일로 변환해 주세요. → 산출물 sessions/2026-05-29T03-53/developer.md
- [2026-05-29] "코다리, 츄가 넘겨주면 SVG 코드들을 모아서 우리만의 CustomIconDB를 구축해. 그리고 외국인들도 쓸 수 있게, 일본어나 영어로 단어를 검색해도 찰떡같이 찾아지도록 다국어 자동 번역/매핑 파이프라인 초안을 짜 와!" → 산출물 sessions/2026-05-29T03-56/developer.md
- [2026-05-29] 리서처가 정리한 추천 규칙을 기반으로 SVG 생성 로직에 데이터 기반 스타일 추천 기능을 통합하세요. 사용자 선호 데이터를 저장하고, 로그 기반 개선안을 반영한 API 엔드포인트를 구현해 주세요. → 산출물 sessions/2026-05-29T04-42/developer.md
- [2026-05-29] 데이터 분석 결과를 API로 연동하여 실시간 규칙 업데이트 시스템을 구현하세요. 실패 로그 자동 수집, 규칙 변경 사항 반영 로직, 버전 관리 시스템을 포함해야 합니다. → 산출물 sessions/2026-05-29T05-48/developer.md
- [2026-05-29] App.tsx와 index.css를 수정해 Toast UI 라이브러리 통합, Framer Motion 트랜지션 추가, Pretendard 폰트 적용, Glassmorphism 패널 구현, Empty State 애니메이션 코드 작성 작업을 진행하세요. → 산출물 sessions/2026-05-29T06-03/developer.md
- [2026-05-29] 리서처가 정리한 추천 규칙을 기반으로 SVG 생성 로직에 동적 필터링 함수를 추가하세요. 사용자 로그 기반 '추천 사항 제시' 기능을 구현할 때, 기존 스타일 선택 UI를 최소 변경으로 통합해야 합니다. → 산출물 sessions/2026-05-29T06-07/developer.md
- [2026-05-29] 리서처가 만든 추천 규칙을 기반으로 SVG 생성 로직에 맞춤형 스타일 추천 기능을 추가하고, 사용자 선호 데이터 저장 구조를 설계하세요. → 산출물 sessions/2026-05-29T06-22/developer.md
- [2026-05-29] "우리의 핵심 경쟁사인 pictographic.ai를 완벽하게 뛰어넘기 위해 전면적인 서비스 업그레이드를 진행할 거야. 카리나(researcher), 현빈(business), 코다리(developer), 츄(designer) 모두 집중해 줘.  [1단계: 시장 분석 및 약점 타격 (카리나 & 현빈)] Pictographic.ai의 특징(방대한 라이브러리, 웹 에디터, 피그마 플러그인)을 인지한 상태에서, 그들이 못하고 있는 **'우리만의 무기'**를 기획해 줘. 예를 들어, 단순 검색을 넘어 문맥을 완벽히 이해하는 'AI 문장 분석
- [2026-05-29] 기능적 버그나 기술적 한계를 검토해주세요. 예상치 못한 에러 발생 시나리오나, 데이터 처리에서의 문제점을 파악하고, 개선 방향을 제안해주세요. → 산출물 sessions/2026-05-29T07-00/developer.md
- [2026-05-29] picto-lab-project/src/App.tsx 파일을 완전히 덮어쓰고 하이브리드 결제 모달 컴포넌트를 구현하세요. 기존 코드는 삭제하고 크레딧 차감 로직, UI 스타일, 상태 관리를 통합해 최종 코드를 작성해 주세요. → 산출물 sessions/2026-05-29T07-21/developer.md