# 길상 블로그

정보처리, IT 토픽 및 트렌드를 정리하고 공유하는 기술 블로그입니다.

## 🚀 블로그 포팅 가이드 (새 계정/저장소 이관)

본 블로그 소스를 새로운 GitHub 계정이나 별도 저장소로 포팅하는 방법은 다음과 같습니다.

### 1. 새 GitHub 저장소 생성 및 코드 업로드
1. GitHub에서 새로운 저장소(Repository)를 생성합니다. (예: `tech-blog`)
2. 본 소스코드를 새 저장소로 푸시(Push)합니다.
   ```bash
   git init
   git remote add origin https://github.com/사용자계정명/저장소명.git
   git branch -M main
   git add .
   git commit -m "Initial commit: port tech blog"
   git push -u origin main
   ```

### 2. 블로그 환경 설정 수정 (`_config.yml`)
`_config.yml` 파일에서 아래 설정 항목을 새 저장소 환경에 맞게 변경합니다.
```yaml
# 예: https://<github-username>.github.io
url: "https://사용자계정명.github.io"

# 저장소 이름 (계정 기본 페이지인 <username>.github.io 저장소라면 빈 값 "" 사용)
# 예: /<repository-name> -> /tech-blog
baseurl: "/저장소명"

github:
  username: 사용자계정명 # 포팅할 GitHub 계정명

social:
  name: 사용자계정명 # 화면에 표시될 소유자 이름
  links:
    - https://github.com/사용자계정명 # 프로필 링크
```

### 3. GitHub Pages 배포 설정 활성화
1. 새 GitHub 저장소 웹페이지로 이동합니다.
2. **Settings** -> **Pages** 메뉴를 클릭합니다.
3. Build and deployment의 **Source** 설정을 **GitHub Actions**로 변경합니다.
4. 코드 푸시 시 자동으로 `.github/workflows/pages-deploy.yml` 액션이 동작하며 수 분 이내로 사이트가 배포됩니다.
5. 배포가 완료되면 `https://사용자계정명.github.io/저장소명` 주소로 접속할 수 있습니다.

---

## ✍️ 블로그 글(포스트) 작성 방법

글을 수동으로 작성하여 업로드하고 싶을 때는 아래 과정을 따르면 됩니다.

1. **마크다운 파일 생성**: `_posts` 폴더 내에 `YYYY-MM-DD-제목.md` 형식의 이름으로 새 파일을 생성합니다.
   * 예시: `_posts/2026-06-22-온디바이스-AI-기술-동향.md`
2. **머리말(Front Matter) 작성**: 파일 최상단에 Jekyll 설정 정보를 입력합니다.
   ```markdown
   ---
   layout: post
   title: "온디바이스 AI 기술 동향 및 기술사 출제 관점"
   date: 2026-06-22
   categories: AI데이터분석
   tags: [On-Device-AI, Edge-AI, LLM]
   ---
   ```
   * **categories**: 카테고리 목록 중 **반드시 1개만** 지정합니다. (소프트웨어공학, 데이터베이스, 네트워크, 정보보안, IT경영, 시스템구조, AI데이터분석, 신기술융합 중 택1)
   * **tags**: 글과 관련된 핵심 기술 키워드를 자유롭게 배열 형태로 지정합니다.
3. **본문 작성**: 마크다운 문법으로 자유롭게 내용을 작성하고 저장한 뒤 Git Push하면 배포가 자동으로 반영됩니다.