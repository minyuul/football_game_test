# World Football Legends

Phaser + Vite 기반 6 vs 6 웹 축구게임 프로토타입입니다.

## 실행
1. Node.js 20+ 설치
2. 프로젝트 폴더에서 `npm install`
3. `npm run dev`
4. 표시되는 로컬 주소 접속

## GitHub Pages 배포
1. 이 폴더 전체를 GitHub 저장소의 `main` 브랜치에 업로드
2. GitHub 저장소 → Settings → Pages → Source를 **GitHub Actions**로 설정
3. Actions의 배포가 완료되면 Pages URL로 실행

## 조작
- WASD: 이동
- Q: 조작 선수 변경
- J: 패스 / 태클
- K: 슛
- Space: 대시

## 현재 핵심 구현
- 2002 / 2006 / 2012 시대
- 시대별 8개 대표팀
- 6 vs 6 (GK 1, DF 2, MF 2, FW 1)
- 팀 단위 전진/후퇴, 압박자 1명 선정, 공간 커버
- GK 전용 possession state
- GK가 공을 잡으면 아군은 빌드업 위치로 확산, 상대는 박스에서 이탈해 패스길 마킹
- GK 안전도 기반 던지기, 압박 시 롱킥
- 패스 / 태클 / 슈팅 / 대시

현재 버전은 플레이 감각과 AI 구조 검증용 프로토타입입니다. 월드컵 토너먼트, 2P 키설정, 선수별 고유 스킬/정교한 능력치는 다음 확장 영역입니다.
