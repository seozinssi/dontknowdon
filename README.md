# DON'T KNOW MONEY Magazine

DON'T KNOW MONEY의 매거진형 정적 HTML 사이트입니다.  
어두운 배경, 큰 브랜드 타이포, 노란 포인트 컬러, 미니멀한 피드 리스트를 기준 디자인으로 사용합니다.

## 실행 방법

1. `index.html`을 브라우저에서 엽니다.
2. 또는 VS Code Live Server로 `tossfeed-edition-clone/` 폴더를 실행합니다.

## 주요 페이지

- `index.html`  
  메인 매거진 페이지입니다. 상단 히어로, 머리 일러스트, ABOUT US 링크 칩, FEED 리스트가 포함되어 있습니다.

- `about.html`  
  DON'T KNOW MONEY 소개 페이지입니다. 브랜드 워드마크, 01~06 소개 섹션, 인스타그램/Threads 링크가 포함되어 있습니다.

- `feeds/1_etf_vs_stock_column.html` ~ `feeds/13.why_interest_rates_move_stocks.html`  
  개별 아티클 페이지입니다. 공통 헤더, 우측/좌측 사이드바, 본문 섹션, 표, KEY INSIGHT, 교육용 고지문, 푸터를 사용합니다.

## 폴더 구조

```text
tossfeed-edition-clone/
  index.html
  about.html
  assets/
    humanhead.png
  feeds/
    1_etf_vs_stock_column.html
    2_how_to_buy_and_sell_stocks.html
    ...
    13.why_interest_rates_move_stocks.html
```

## 디자인 기준

- 배경: `#17171d`
- 본문 텍스트: `#f2f2f4`
- 보조 텍스트: `#9b9ba4`
- 포인트 컬러: `#ffe65b`
- 최대 콘텐츠 폭: `--max-width: 1200px`
- 헤더 높이: `--header-height`

## 레이아웃 규칙

- 데스크톱 메인/ABOUT은 같은 사이트 그리드와 헤더 폭을 공유합니다.
- 모바일에서는 헤더 우측에 `MENU / CLOSE` 토글 메뉴를 사용합니다.
- 메인 FEED는 `DON'T KNOW MONEY FEED` 워드마크와 에피소드 리스트로 구성합니다.
- 피드 제목은 `EP.01` 형식의 번호와 제목 사이 간격을 고정해 정렬감을 유지합니다.
- 아티클 페이지 상단 제목에는 이모지를 사용하지 않습니다.
- 아티클 본문 소제목은 과하게 크지 않게 맞추고, 본문은 가독성을 위해 양쪽 정렬을 사용합니다.

## 수정 포인트

- 브랜드/헤더: `.site-header`, `.header-inner`, `.brand`, `.nav`, `.menu-toggle`
- 메인 히어로: `.hero-money`, `.hero-title`, `.hero-subcopy`, `.hero-art`, `.keyword-cloud`
- 메인 피드: `.magazine-layout`, `.intro-panel`, `.edition-list`, `.edition-title`, `.edition-ep`
- ABOUT 페이지: `.about-layout`, `.about-aside`, `.about-wordmark`, `.about-section`, `.social-links`
- 아티클 공통: `feeds/` 내부 각 아티클 HTML의 `:root`, `.site-header`, `.article`, `.section`, `.key-insight`, `.footer-note`

## 소셜 링크

- Instagram: `https://www.instagram.com/dont.knowdon/`
- Threads: `https://www.threads.com/@dont.knowdon?hl=ko`

## 고지문 기준

개별 아티클 하단에는 다음 취지의 교육용 고지문을 공통으로 사용합니다.

> 본 콘텐츠는 금융과 투자 개념을 쉽게 이해하기 위한 교육용 자료이며, 특정 금융상품이나 종목의 매수·매도를 권유하지 않습니다. 모든 투자 판단과 그에 따른 책임은 투자자 본인에게 있습니다.

## 푸터

모든 아티클 하단 푸터 표기는 다음으로 통일합니다.

```text
© DON'T KNOW MONEY
```
