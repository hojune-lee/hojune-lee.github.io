# Hojune Lee — personal website

홈페이지: <https://hojune-lee.github.io/>  
블로그: <https://hojune-lee.github.io/blog/>

GitHub Pages와 Jekyll로 운영합니다. `main`에 push하면 자동으로 빌드·배포됩니다.

## 새 글 작성

1. `_drafts/post-template.md`를 복사합니다.
2. `_posts/2026-10-09-my-first-post.md`처럼 **날짜-영문주소.md** 형식으로 저장합니다.
3. 맨 위의 제목·소개·언어를 바꾸고, 그 아래에 Markdown으로 글을 작성합니다.
4. 커밋해서 `main`에 push합니다. 빌드가 끝나면 블로그 목록과 글 페이지에 자동으로 나타납니다.

```markdown
---
layout: post
title: "글 제목"
description: "목록에 표시할 짧은 소개"
lang: ko
---

본문을 여기에 작성합니다.

## 소제목

글 내용...
```

- `description`는 선택 사항입니다. 생략하면 목록에는 제목과 날짜만 표시됩니다.
- 영어 글은 `lang: en`으로 설정합니다.
- 이미지는 `assets/images/`에 넣고 `![설명](/assets/images/example.png)`으로 연결합니다.
- 글 주소는 `/blog/2026/10/09/my-first-post/` 형식입니다. 공개 후 파일명이나 날짜를 바꾸면 주소도 바뀝니다.
- 미래 날짜의 글은 빌드 시점에 공개되지 않습니다. 해당 날짜 이후 커밋을 push하거나 GitHub Actions에서 배포를 다시 실행하면 공개됩니다.
- `_drafts/`의 초안은 사이트에 표시되지 않습니다. 다만 이 저장소 자체는 공개되어 있습니다.

브라우저에서도 [GitHub의 새 글 작성 화면](https://github.com/hojune-lee/hojune-lee.github.io/new/main/_posts)에서 파일명과 내용을 입력하고 커밋할 수 있습니다.

## 파일 안내

- `index.html`: 소개, 논문, 학력
- `_config.yml`: 연락처, Google Scholar 등 외부 링크, 사이트 설정
- `blog/index.html`: 블로그 글 목록
- `_layouts/default.html`: 공통 머리말·꼬리말
- `_layouts/post.html`: 글 페이지
- `assets/style.css`, `assets/blog.css`: 스타일

## 로컬 미리보기

Ruby와 Bundler가 설치된 환경에서:

```sh
bundle install
bundle exec jekyll serve
```

<http://127.0.0.1:4000/>에서 확인할 수 있습니다. 초안까지 미리 보려면 `bundle exec jekyll serve --drafts`를 사용하세요. 로컬 미리보기는 공개 배포에 영향을 주지 않습니다.
