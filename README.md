# P-Racing

평택대학교 자작자동차 동아리 P-Racing 웹사이트.

[웹사이트](https://p-racing.github.io/P-racing-web/)

## 로컬 실행

Node.js가 설치된 환경에서 실행합니다. 별도 패키지 설치는 필요하지 않습니다.

```sh
node server.mjs
```

http://127.0.0.1:4173 에서 확인할 수 있습니다.

## 구성

- `dist/`: HTML, CSS, JavaScript 및 배포 파일
- `server.mjs`: 로컬 미리보기 서버
- `tests/`: 탐색 동작, 서버 요청 처리, 화면 크기별 검사

## 테스트

```sh
node tests/navigation.cjs
node tests/security.cjs
```

화면 크기별 검사는 Playwright와 Edge가 설치된 환경에서 로컬 서버 실행 후 `node tests/responsive.cjs`로 진행합니다.

## 배포

main 브랜치에 사이트 변경을 푸시하면 GitHub Actions가 dist 폴더를 GitHub Pages에 자동 배포합니다. 별도 배포 브랜치는 사용하지 않습니다.

