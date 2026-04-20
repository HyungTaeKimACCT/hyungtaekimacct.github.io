# HyungTae Kim - Academic Homepage (Jekyll Version)

Jekyll 기반 학술 홈페이지입니다.

## 🎉 새로운 기능

### ✅ 블로그 포스팅
- Markdown으로 쉽게 글쓰기
- `_posts` 폴더에 파일 추가만 하면 자동으로 블로그에 나타남

### ✅ YouTube 비디오 임베드
- Teaching 페이지에서 Unlisted 비디오 재생
- 학생들이 홈페이지에 머무르면서 시청

### ✅ PDF 강의자료
- 홈페이지에서 바로 보기 + 다운로드
- `assets/course-materials` 폴더에 업로드

---

## 📝 블로그 포스트 작성 방법

### 1. 새 포스트 파일 만들기
`_posts` 폴더에 파일 생성:
```
_posts/2024-04-20-my-post-title.md
```

파일명 형식: `YYYY-MM-DD-title.md`

### 2. 포스트 작성
```markdown
---
layout: post
title: "포스트 제목"
date: 2024-04-20
---

## 첫 번째 섹션

내용을 여기에 작성...

### 하위 섹션

- 리스트 항목 1
- 리스트 항목 2

더 많은 내용...
```

### 3. GitHub에 업로드
```bash
git add _posts/2024-04-20-my-post-title.md
git commit -m "Add new post"
git push
```

5-10분 후 자동으로 사이트에 나타남!

---

## 🎥 YouTube 비디오 추가하기

### 1. YouTube에 Unlisted로 업로드
- 비디오 ID 복사 (예: `dQw4w9WgXcQ`)

### 2. teaching.md 파일 수정
```html
<iframe src="https://www.youtube.com/embed/YOUR-VIDEO-ID" ...></iframe>
```

`YOUR-VIDEO-ID`를 실제 비디오 ID로 교체

---

## 📄 PDF 강의자료 업로드하기

### 1. PDF 파일 준비
- PPT → PDF로 변환

### 2. 파일 업로드
```
assets/course-materials/acct162/week1-notes.pdf
```

### 3. teaching.md에서 링크 수정

---

## 🚀 GitHub에 업로드하기

### 처음 업로드 (모든 파일)
```bash
# 기존 index.html 삭제
rm index.html

# 모든 새 파일 추가
git add .
git commit -m "Convert to Jekyll"
git push
```

---

만든 날짜: 2024년 4월
