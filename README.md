# SKY STRIKER EVO — iPad 홈 화면 웹앱

이 프로젝트는 HTML5 Canvas + JavaScript로 만든 설치형 웹앱(PWA)입니다. 기체 3종, 서로 다른 발사 패턴, 파워 아이템 최대 5단계, 27초 주기의 스테이지 보스, 폭탄, 기기 내 TOP 5 랭킹을 포함합니다.

## iPad만으로 설치하기 (GitHub Pages)

1. Safari에서 github.com에 로그인하거나 무료 계정을 만듭니다.
2. 새 **Public** 저장소(예: `sky-striker-evo`)를 만듭니다.
3. 이 ZIP의 압축을 풀고 **index.html, game.js, manifest.webmanifest, sw.js, icons 폴더**를 저장소 최상위에 업로드합니다. GitHub 웹 화면에서 Add file → Upload files를 이용할 수 있으며, iPad에서는 Safari의 데스크톱 웹사이트 보기가 편할 수 있습니다.
4. 저장소 **Settings → Pages → Build and deployment → Deploy from a branch**에서 `main` 브랜치, `/(root)`를 선택하고 Save를 누릅니다.
5. 배포가 끝나면 `https://계정명.github.io/sky-striker-evo/` 주소를 Safari에서 엽니다. 실제 주소는 Pages 설정 화면에 표시됩니다.
6. Safari의 **공유 → 홈 화면에 추가 → 추가**를 누릅니다. 홈 화면의 Sky Striker 아이콘을 눌러 실행합니다.
7. 처음 온라인으로 열어 파일이 캐시되면 이후에는 오프라인에서도 실행할 수 있습니다(기기 저장소 정리 등으로 캐시가 제거될 수 있음).

## 주의

- ZIP을 파일 앱에서 단순히 열면 서비스 워커와 설치 기능이 동작하지 않습니다. HTTPS 호스팅이 필요합니다.
- 랭킹은 기기의 웹 저장소(localStorage)에 저장되며 다른 사람과 공유되지 않습니다.
- 게임 소리는 기본 꺼짐이며 게임 내 버튼으로 켤 수 있습니다.
- iOS 앱스토어용 IPA 파일이 아니라 홈 화면에서 독립 실행되는 PWA입니다.
