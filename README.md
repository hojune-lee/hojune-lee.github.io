# Ho June Lee — 개인 웹사이트

KAIST 전산학부·수학과 개인 웹사이트 (GitHub Pages용)입니다.

## 구조

- **`index.html`** — 메인: 소개, CV 다운로드 버튼, GitHub·네이버 블로그 링크
- **`music/index.html`** — 좋아하는 음악·밴드 플레이리스트 스타일 목록
- **`courses/index.html`** — 관심 있게 들은 과목 정리
- **`assets/style.css`** — 공통 스타일

## 사용 전에 할 일

1. **CV**: 프로젝트 루트에 `cv.pdf` 파일을 넣으면 메인 페이지의 "CV 다운로드" 버튼으로 내려받을 수 있습니다.
2. **네이버 블로그**: `index.html`에서 `https://blog.naver.com/YOUR_BLOG_ID`를 본인 블로그 주소로 바꿔 주세요.
3. **소개·취미·연구 분야**: `index.html`의 괄호 안 안내 문구를 지우고 본인 내용으로 채워 주세요.
4. **음악·과목**: `music/index.html`, `courses/index.html`의 예시 카드를 지우고 원하는 항목으로 수정해 주세요.

## 로컬에서 확인

프로젝트 폴더에서 로컬 서버를 띄운 뒤 브라우저로 확인할 수 있습니다.

```bash
# Python 3
python3 -m http.server 8000
# 브라우저에서 http://localhost:8000 열기
```

GitHub에 푸시하면 `https://hojune-lee.github.io` 에서 자동으로 배포됩니다.
