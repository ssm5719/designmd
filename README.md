# 랩241 디자인 파일

제품별 디자인 규칙과 CSS를 모아 둔 저장소입니다. 제품마다 디자인이 다르므로, 작업할 제품의 폴더만 보면 됩니다.

| 폴더 | 제품 | 최신 버전 | 상태 |
| --- | --- | --- | --- |
| [`eseodang-admin/`](eseodang-admin/) | 이서당 관리자 | v1.0 | 인계 완료 |
| `kiosk/` | 키오스크 | — | 준비 중 |
| → [ssm5719/cl](https://github.com/ssm5719/cl) | 클라우드러닝 | — | 별도 저장소 |
| `lab241-home/` | 랩241 홈페이지 | — | 준비 중 |

클라우드러닝은 디자인 규칙(`design/`)과 화면 미리보기(`lab/`)를 같이 두느라 [`ssm5719/cl`](https://github.com/ssm5719/cl) 저장소를 따로 씁니다. 쓰는 법은 아래와 같고, 복사할 폴더는 그 저장소의 `design/` 입니다.

## 개발자가 쓰는 법

1. 이 저장소를 받습니다: `git clone https://github.com/ssm5719/designmd`
2. 작업할 제품 폴더의 내용을 앱 소스의 `design/` 폴더에 복사합니다.
   예: `eseodang-admin/` 안의 파일 전부 → 이서당 관리자 소스의 `design/`
3. 디자인이 바뀌었다는 연락을 받으면 `git pull` 후 2번을 다시 하고,
   그 제품 폴더의 `CHANGELOG.md`에서 무엇이 바뀌었는지 확인합니다.

Claude Code로 작업한다면 이렇게 시키면 됩니다:
"designmd 저장소를 최신으로 받아서 eseodang-admin 폴더를 design/에 반영하고, CHANGELOG의 최신 항목대로 화면을 고쳐 줘."

## 폴더 안에 있는 것

| 파일 | 내용 |
| --- | --- |
| `README.md` | 색 · 글자 · 여백 · 상태 표현 규칙. 가장 먼저 읽습니다 |
| `tokens.css` | 색 · 글자 · 여백 CSS 변수 |
| `bundle.css` | 버튼, 칩, 표, 설정 줄 같은 화면 구성 요소의 스타일 |
| `tokens.json` | `tokens.css`와 같은 값을 데이터로 정리한 것 |
| `components/*.md` | 화면 구성 요소별 사용 규칙 |
| `CHANGELOG.md` | 버전별 바뀐 내용 |

화면 모양(프로토타입)과 개발 인계 문서는 [랩241 디자인 자료 모음](https://claude.ai/code/artifact/e7e849e5-a58a-4750-8e29-2c4fae9a9e33)에 있습니다.
