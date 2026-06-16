# BigValue Design System Web Document

정적 웹 문서 형태의 BigValue Design System v0.1.1 초안입니다.

## 구성

- `index.html`: 공유 가능한 단일 웹 문서
- `tokens.css`: 제품 적용용 CSS 변수
- `tokens.json`: 디자인 토큰 JSON
- `assets/`: CI 가이드 PDF에서 추출한 참고 이미지

## 로컬에서 보기

브라우저에서 `index.html`을 열면 됩니다.

```bash
cd bigvalue-design-system
python3 -m http.server 8080
```

그 다음 `http://localhost:8080` 접속.

## 웹 공유 방법

1. 이 폴더를 GitHub 저장소에 업로드합니다.
2. GitHub Pages를 켜고 루트 폴더를 배포합니다.
3. 또는 Netlify/Vercel에 폴더를 드래그 앤 드롭합니다.

## 운영 전 체크

- PDF에서 추출한 로고 PNG는 임시 웹용입니다. 최종 운영 전 원본 SVG/PNG 로고로 교체하세요.
- 실제 Figma 컴포넌트 라이브러리와 연결하려면 컴포넌트명/Variant명을 문서와 맞춰 주세요.
- 접근성 기준은 WCAG 2.2 AA를 목표로 잡았습니다.


## Changelog
- 2026-06-16: Primary Logo를 사용자가 제공한 원본 PNG로 교체했습니다.


## v0.1.2

- `index.html` and `index-standalone.html` embed image assets as data URIs for reliable preview in ChatGPT sandbox links.
- The `assets/` folder is still included for normal web deployment and future asset replacement.
