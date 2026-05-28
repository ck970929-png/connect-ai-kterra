# 📺 레오 (Head of YouTube) 개인 메모리

_레오 에이전트만 읽고 쓰는 개인 노트. 학습·교훈·자주 쓰는 패턴이 누적됩니다._

## 학습 기록

- [2026-05-28] picto-lab-project/docs/picto-lab-direction.md 파일을 PICTO LAB의 최상위 기획 기준서로 사용해줘.  기존 루트에 있는 PICTO_LAB_FINAL_SPEC.md, Project_Core_Summary.md보다 이 문서의 방향성을 우선해서 반영해줘.  우선 MVP 1단계만 구현해줘: - 키워드 입력 - 용도 선택 - 스타일 선택 - 후보 4개 표시 - SVG 다운로드 - PNG 다운로드  로그인, 결제, 구독, 팀 기능, 관리자 페이지, 고급 추천 알고리즘은 아직 구현하지 마. → 산출물 s
- [2026-05-28] 보고 확인했어.  다만 현재 보고는 “실제 실행 완료”가 아니라 “구현 구조 설명/시뮬레이션”에 가까워 보여.  이제는 설명이 아니라 실제 파일과 실행 결과 기준으로 검증해줘.  먼저 현재 구조를 아래 기준으로 정리해줘.  1. 컴포넌트는 반드시 src/components/ 아래에 둬.     * src/components/InputPanel.tsx    * src/components/ResultPanel.tsx  2. SVG 생성/다운로드 로직은 반드시 src/lib/ 아래에 둬.     * src/lib/svg-renderer.
- [2026-05-28] 지금 작업이 PICTO LAB MVP 범위에서 벗어났어.  이번 세션에서는 YouTube, PayPal, 결제, 매출 분석, 관리자 페이지, 외부 연결, 자격증명, my_videos_check.py 관련 작업을 전부 중단해.  PICTO LAB MVP 1단계와 무관한 내용:  * YouTube 채널 분석 * PayPal 매출 분석 * Client ID / Secret 입력 * 결제 ID 입력 필드 * 관리자 페이지 * 외부 API 연결 * my_videos_check.py 실행 * auto_planner.py 실행 * 시장/비즈니스