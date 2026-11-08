# 대림 · 오늘의 식탁

서비스: https://rnk2026.github.io/daerim/

이 저장소는 배포 설정만 관리합니다. 공통 코드와 대림 설정의 원본은 [RnK2026/menu](https://github.com/RnK2026/menu)입니다.

- 공유 기능 수정: 원본의 `app.js`, `core.js`, `index.html`, `style.css`
- 대림 전용 기능: 원본의 `services/daerim/extension.js`
- 대림 API 주소: 원본의 `services/daerim/config.json`
- 대림 정적 메뉴: 원본의 `services/daerim/menu.json`
- 저장 서버 설치: 원본 README의 대림 저장 서버 연결 안내

공통 저장소 main이 변경되면 원본의 Sync Daerim deployment 워크플로가 이 저장소의 `source-revision.txt`를 갱신합니다. 그 push가 Deploy Daerim from shared source 워크플로를 실행해 최신 공통 소스를 테스트·배포합니다. 연결에는 이 저장소의 쓰기 전용 Deploy Key와 원본 저장소의 `DAERIM_DEPLOY_KEY` Actions secret을 사용합니다. 정기 실행은 사용하지 않으므로 공개 저장소의 60일 예약 워크플로 비활성화 규칙이 적용되지 않습니다. 즉시 재배포하려면 Actions → Deploy Daerim from shared source → Run workflow를 실행하세요.

원본 저장소의 최신 main을 사용하며, 식단 데이터는 기존 RnK와 별도 Apps Script 프로젝트에 저장합니다. 이 저장소에 기능 코드를 복사해 수정하지 마세요.
