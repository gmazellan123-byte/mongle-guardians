# 몽글숲 가디언즈

귀여운 수호자들과 함께 몽글숲 12구역, 60개 Stage를 지나 마왕성의 마왕을 물리치는 HTML5 액션 게임입니다.
원스토어 웹게임(H5 Game SDK v1.1.0) 연동을 포함하고, 일반 브라우저에서도 SDK 없이 그대로 플레이할 수 있습니다.

- 플레이: https://gmazellan123-byte.github.io/mongle-guardians/
- `main`에 푸시하면 GitHub Actions로 GitHub Pages에 자동 배포됩니다 (`.github/workflows/pages.yml`).

## 구성

| 경로 | 내용 |
|---|---|
| `index.html` | 게임 전체 (HTML·CSS·JS 한 파일) |
| `vendor/three.min.js` | three.js r128 (MIT, `vendor/three.LICENSE.txt`) |
| `fonts/Jua.woff2` | Jua 글꼴, 자주 쓰는 한글 2,350자와 게임에 쓰인 글자만 담음 (SIL OFL 1.1, `fonts/Jua.OFL.txt`) |

## 원스토어 등록 메모

- 테스트 URL은 끝이 `/`인 주소로 등록 (`/`를 빼면 리다이렉트되어 로딩·SDK 통신이 실패할 수 있음)
- GitHub Pages는 iframe을 막는 헤더(`X-Frame-Options`, `frame-ancestors`)를 보내지 않아 원스토어 앱 안에서 열 수 있음
