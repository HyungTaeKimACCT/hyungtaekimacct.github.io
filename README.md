# HyungTae Kim - Academic Homepage

개인 학술 홈페이지입니다. GitHub Pages로 호스팅됩니다.

## 🚀 시작하기

### 1단계: 파일 업로드
이 저장소에 다음 파일들을 업로드하세요:
- `index.html` - 메인 웹페이지
- `styles.css` - 스타일시트
- `script.js` - JavaScript 기능

### 2단계: GitHub Pages 활성화
1. GitHub 저장소 설정 (Settings) 이동
2. 왼쪽 메뉴에서 "Pages" 선택
3. Source를 "Deploy from a branch"로 설정
4. Branch를 "main" (또는 "master") 선택, 폴더는 "/ (root)" 선택
5. Save 클릭

5-10분 후 `https://[your-username].github.io`에서 사이트 확인 가능합니다.

## ✏️ 수정해야 할 부분

### index.html에서 업데이트:
1. **ResearchGate 링크**: 
   ```html
   <a href="https://www.researchgate.net/profile/Your-Profile" target="_blank">
   ```
   → 실제 ResearchGate 프로필 URL로 변경

2. **Google Scholar 링크**:
   ```html
   <a href="https://scholar.google.com/citations?user=Your-ID" target="_blank">
   ```
   → 실제 Google Scholar 프로필 URL로 변경

3. **Google Drive 링크**:
   ```html
   <a href="https://drive.google.com/drive/folders/your-folder-id" target="_blank">
   ```
   → 실제 공유 폴더 URL로 변경 (2곳)

4. **이메일 주소**:
   ```html
   <a href="mailto:your.email@csufresno.edu">your.email@csufresno.edu</a>
   ```
   → 실제 이메일 주소로 변경

5. **오피스 위치**:
   ```html
   <p><strong>Office:</strong> [Your Office Location]</p>
   ```
   → 실제 오피스 위치로 변경

### 사진 추가하기:
1. 프로필 사진을 `photo.jpg` 이름으로 저장소에 업로드
2. `index.html`에서 다음 부분 찾기:
   ```html
   <div class="placeholder-image">
       <p>Your Photo</p>
   </div>
   ```
3. 다음으로 교체:
   ```html
   <img src="photo.jpg" alt="HyungTae Kim" style="width: 250px; height: 250px; border-radius: 50%; object-fit: cover; border: 4px solid white; box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);">
   ```

## 💰 Google AdSense 추가하기

### 1단계: AdSense 승인 받기
1. [Google AdSense](https://www.google.com/adsense/) 가입
2. 사이트 URL 제출: `https://[your-username].github.io`
3. 승인 코드를 `index.html`의 `<head>` 섹션에 추가

### 2단계: 광고 삽입
승인 후 광고 코드를 받으면:
1. `index.html`에서 "Ad Space" placeholder 찾기
2. AdSense 코드로 교체

예시:
```html
<!-- 기존 placeholder -->
<div class="ad-placeholder">
    <p>📢 Ad Space</p>
</div>

<!-- AdSense 코드로 교체 -->
<script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-YOUR-ID"
     crossorigin="anonymous"></script>
<ins class="adsbygoogle"
     style="display:block"
     data-ad-client="ca-pub-YOUR-ID"
     data-ad-slot="YOUR-SLOT-ID"
     data-ad-format="auto"></ins>
<script>
     (adsbygoogle = window.adsbygoogle || []).push({});
</script>
```

## 📝 콘텐츠 업데이트 방법

### GitHub 웹 인터페이스 사용:
1. GitHub에서 `index.html` 클릭
2. 연필 아이콘 (Edit) 클릭
3. 내용 수정
4. 하단에 "Commit changes" 클릭
5. 몇 분 후 사이트에 자동 반영됨

### 로컬 편집 후 업로드:
```bash
git pull
# 파일 편집
git add .
git commit -m "Update content"
git push
```

## 🎨 색상 커스터마이징

`styles.css` 파일 상단의 색상 변수 수정:
```css
:root {
    --primary-color: #1e3a8a;      /* 메인 네이비 블루 */
    --secondary-color: #3b82f6;    /* 강조 파란색 */
    --text-dark: #1f2937;          /* 어두운 텍스트 */
    --text-light: #6b7280;         /* 밝은 텍스트 */
    --bg-light: #f9fafb;           /* 배경색 */
}
```

## 🔄 다음 단계: Jekyll로 업그레이드

이 HTML 버전이 만족스러우면 Jekyll로 마이그레이션할 수 있습니다:
- 더 쉬운 콘텐츠 관리 (Markdown 사용)
- 블로그 기능 추가 가능
- 더 많은 테마와 플러그인

자세한 가이드는 별도로 제공 예정입니다.

## 📞 문제 해결

### 사이트가 안 보여요
- GitHub Pages 설정 확인
- 저장소가 Public인지 확인
- 파일명이 정확히 `index.html`인지 확인
- 5-10분 기다려보세요 (배포 시간)

### 링크가 작동 안 해요
- URL에 `https://` 포함되어 있는지 확인
- Google Drive 링크가 "Anyone with the link" 권한인지 확인

---

만든 날짜: 2024년 4월
라이선스: MIT
