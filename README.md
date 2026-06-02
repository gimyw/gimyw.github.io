# 포트폴리오 사이트

단일 HTML/CSS 정적 페이지. GitHub Pages 무료 호스팅.

## 로컬 미리보기

`index.html`을 브라우저로 더블클릭하면 끝. (빌드·서버 불필요)

## 수정할 곳

`index.html` 안의 `<!-- TODO -->` 주석을 모두 채우면 됩니다:

- 이름 / 이니셜 (title, brand, hero, footer)
- 프로필 사진 → `assets/profile.jpg`
- GitHub URL (hero, projects, contact)
- Experience 타임라인 (인턴·해커톤 등 추가)
- 프로젝트 카드 (복제해서 늘리기, 이미지 `assets/`에)
- Awards / Certification (AWS SAA 등)
- Contact 링크 (블로그·LinkedIn 등)

이미지 권장 크기: 프로필 280×280, 프로젝트 썸네일 400×260.

## GitHub Pages 배포 (username: gimyw)

1. GitHub → New repository → 이름 **`gimyw.github.io`** → Public → Create
   (README·.gitignore 체크 없이 빈 repo로)
2. 이 폴더를 push:
   ```bash
   cd portfolio
   git init
   git add .
   git commit -m "feat: 포트폴리오 초안"
   git branch -M main
   git remote add origin https://github.com/gimyw/gimyw.github.io.git
   git push -u origin main
   ```
3. 1~2분 뒤 **`https://gimyw.github.io`** 접속.

> repo 이름이 `gimyw.github.io`면 Pages가 자동 활성화됨.
> 혹시 안 뜨면 Settings → Pages → Source를 `main` 브랜치 `/ (root)`로 지정.

## 커스텀 도메인 (선택)

repo Settings → Pages → Custom domain에 도메인 입력 후, 도메인 DNS에 CNAME 레코드 추가.
