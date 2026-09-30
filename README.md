# 문법 트레이너

토익 왕초보용 영어 문법 27강 + 단어 플래시카드 웹앱입니다.
`index.html` 하나에 모든 데이터가 들어 있어서 서버 없이 GitHub Pages로 바로 쓸 수 있습니다.

## GitHub Pages로 올리기

1. GitHub에서 새 저장소를 만듭니다. (예: `grammar-trainer`, Public)
2. 이 폴더 안의 파일을 모두 저장소 루트에 올립니다. (`index.html`이 맨 위에 있어야 합니다)
   - 웹에서 올릴 때: 저장소 화면의 **Add file → Upload files**에 폴더 안 파일들을 끌어다 놓고 **Commit changes**
3. 저장소의 **Settings → Pages**에서
   - Source: **Deploy from a branch**
   - Branch: **main**, 폴더 **/(root)** 선택 후 **Save**
4. 1~2분 뒤 `https://<내 아이디>.github.io/grammar-trainer/` 주소로 접속합니다.

## 휴대폰에서 앱처럼 쓰기

- 안드로이드(크롬): 주소창 메뉴 → **홈 화면에 추가**
- 아이폰(사파리): 공유 버튼 → **홈 화면에 추가**

## 학습 기록 저장

- 학습 기록(푼 문제, 오답노트, 북마크, 단어 카드 알아요/암기 필요)은 **그 기기의 브라우저**에 저장됩니다.
- 기기나 브라우저가 바뀌면 기록이 따로 쌓입니다. 브라우저 데이터를 지우면 기록도 지워집니다.

## 파일 구성

| 경로 | 내용 |
| --- | --- |
| `index.html` | 앱 본체 (문법·단어 데이터 포함) |
| `data/english_grammar_toeic.json` | 문법 27강, 확인 문제, 부록 원본 데이터 |
| `data/toeic_vocab.json` | 해커스 토익 단어장, 구동사 단어장, 토익 빈출 단어장 데이터 |
| `manifest.webmanifest`, `icons/` | 홈 화면 추가용 앱 정보와 아이콘 |
| `.nojekyll` | GitHub Pages가 파일을 그대로 서비스하도록 하는 설정 |

`data/` 폴더의 JSON은 참고·수정용 원본입니다. 앱은 `index.html` 안에 넣어 둔 데이터를 사용하므로, JSON을 고쳐도 앱에 자동으로 반영되지는 않습니다.
