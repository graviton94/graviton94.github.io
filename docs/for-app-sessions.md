# 앱 담당 세션에게: graviton94.github.io 에 맞출 것

이 저장소는 앱 4종의 공식 홈페이지 **당신의 하루 · Your Day** (https://graviton94.github.io/) 예요.
GitHub Pages 가 `main` 을 그대로 보여 줘요. 작업 브랜치에서 고치고 PR 로 `main` 에 합쳐요.

## 공통 틀 (모든 페이지)
- `<link rel="stylesheet" href="(위로)/style.css">` 를 쓴다. 색 · 글꼴은 style.css 한 곳에서.
- `<main>` 바로 안 맨 위에 사이트 머리:
  `<div class="site"><a href="(사이트 맨 위)"><b>당신의 하루 · Your Day</b></a><span><a href="mailto:ruahn49@gmail.com">문의 · Contact</a></span></div>`
- `</main>` 바로 앞에 꼬리:
  `<footer>문의 · Contact <a href="mailto:ruahn49@gmail.com">ruahn49@gmail.com</a> · <a href="(사이트 맨 위)about/">운영 원칙 · About</a></footer>`
- 한국어 먼저, 그 아래 `id="en"` 영어. 이모지 없이, 짧게.
- 첫 화면(index.html)의 앱 줄: 아이콘(`icons/<앱>.png`, 128px) · 이름 · 한 줄 소개 · 링크(소개 · 개인정보처리방침 · 이용약관 · 출처 · Google Play 중 있는 것만).
- 운영 원칙(`about/`)에 앱별 원칙이 생기면 그 앱 이름을 붙여 한 줄 더한다.

## 앱별로 할 일
### 하루의 정원 · Carpe Diem (CARPEDIEM 세션)
- 개인정보처리방침은 `/carpediem/privacy/` 로 옮겼다. 옛 주소 `/privacy/` 는 새 주소로 넘겨 주는 페이지로 남아 있어 Play Console 주소가 깨지지 않지만, 앱 안 링크 · Play Console 은 새 주소로 바꾼다.
- 소개 페이지 `/carpediem/` (2026-10-18, 1.1.8 기준): 대표 그림 · 화면 넷 (`carpediem/img/`, 앱 저장소 `docs/store/` 에서) · 기능 · 응원하기 가격 · 출처. 첫 화면에 소개 · Google Play 링크.
- 기능 · 가격 · 마음 가짓수가 바뀌면 `/carpediem/` 도 같이 고친다.
- 아이콘이 바뀌면 `icons/carpediem.png` (128px) 를 바꾼다.

### 하루의 성경 · Bible by Hand (TODAYBIBLE 세션)
- 아이콘은 사용자가 준 펜촉 · 십자가 그림으로 바꿨다 (`icons/todaybible.png`). 앱 아이콘과 다르면 앱 쪽을 확인.
- 유료 기능이 생기면 이용약관 `/todaybible/terms/` 를 만들고 첫 화면 링크에 더한다.
- 스토어에 공개되면 Google Play 링크 (`…?id=io.github.graviton94.todaybible`).

### 방구뿡 · Pocket Toot (bgbb 세션)
- 앱 저장소: `graviton94/bgbb` · 패키지 `io.github.graviton94.bgbb`.
- 소개 `/bgbb/` · 개인정보처리방침 `/bgbb/privacy/` (2026-10-20, 1.0.0 기준). 화면 · 대표 그림은 앱 저장소 `docs/store/` 에서 `bgbb/img/` 로 (432×768 webp).
- 앱 설정 화면의 링크가 `/bgbb/privacy/` 와 `/bgbb/#credits` 를 가리킨다. 주소를 바꾸면 앱도 같이 바꾼다.
- 스토어에 공개되면 첫 화면 · 소개 페이지에 Google Play 링크 (`…?id=io.github.graviton94.bgbb`).
- 권한 · 수집 정보가 바뀌면 개인정보처리방침을 먼저 고친다 (지금: 마이크는 녹음 버튼을 누를 때만, 전송 없음).

### 언어 미술관 · Lingua Museum (todayletters 세션이 맡음)
- 출처 페이지 `todayletters/index.html` 의 표시 사이(`<!-- sources:… -->`)는 앱 저장소의 `scripts/site_sources.py` 가 다시 쓴다. 손으로 고치지 않는다.
