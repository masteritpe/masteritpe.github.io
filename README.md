# 기술사 뉴스 블로그

정보관리기술사 출제분야 관점의 IT 뉴스 토픽 및 트렌드를 정리하고 공유하는 기술 블로그입니다.
이 저장소는 자동화 빌드 배치 및 외부 종속성을 완전히 걷어내고, 사용자가 `_posts` 폴더에 마크다운(MD) 파일만 작성해 넣으면 GitHub Pages를 통해 자동으로 웹사이트가 구성되는 단순하고 깔끔한 정적 블로그 템플릿입니다.

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
    - https://cafe.naver.com/kpcitpe
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
   * **categories**: 8개 출제 분야 중 **반드시 1개만** 지정합니다. (소프트웨어공학, 데이터베이스, 네트워크, 정보보안, IT경영, 시스템구조, AI데이터분석, 신기술융합 중 택1)
   * **tags**: 글과 관련된 핵심 기술 키워드를 자유롭게 배열 형태로 지정합니다.
3. **본문 작성**: 마크다운 문법으로 자유롭게 내용을 작성하고 저장한 뒤 Git Push하면 배포가 자동으로 반영됩니다.

---

## 💻 로컬에서 블로그 실행 및 미리보기

블로그에 글을 쓰고 로컬 컴퓨터에서 변경사항을 미리 확인하고 싶을 때 사용하는 방법입니다.

### 방법 1. Docker 사용 (가장 추천 - Ruby 설치 필요 없음)
로컬에 Ruby나 Jekyll을 직접 설치하지 않고도 Docker를 이용해 간단히 실행할 수 있습니다.
```bash
docker run --rm \
  --volume="$PWD:/srv/jekyll" \
  -p 4000:4000 \
  -it jekyll/jekyll:4.2.0 \
  jekyll serve
```
웹 브라우저를 열고 `http://localhost:4000/저장소명/`에 접속하여 실시간 변경사항을 확인합니다.

### 方法 2. Ruby 및 Jekyll 직접 설치 시
로컬 환경에 Ruby 3.x와 Bundler가 설치되어 있다면 아래 명령어를 사용하여 실행합니다.
```bash
bundle install
bundle exec jekyll serve
```
웹 브라우저를 열고 `http://localhost:4000/저장소명/`로 확인합니다.
