# 🔧 SELENE 랩원들을 위한 업데이트 가이드

랩 홈페이지는 GitHub Pages와 Jekyll로 관리됩니다.
아래 절차에 따라 홈페이지 내용을 수정하고 Pull Request(PR)를 보내주세요.

---

## 1. 저장소 Fork 생성

1. 랩 홈페이지 저장소로 이동
   👉 [https://github.com/ku-selene/ku-selene.github.io](https://github.com/ku-selene/ku-selene.github.io)
2. 우측 상단의 **Fork** 버튼을 클릭하여
   본인 GitHub 계정으로 저장소를 포크합니다.
   → `<본인ID>/ku-selene.github.io` 형태의 개인 저장소가 생성됩니다.

---

## 2. 로컬 환경에서 사이트 실행

### 2.1 저장소 클론

```bash
git clone https://github.com/<본인ID>/ku-selene.github.io.git
cd ku-selene.github.io
```

### 2.2 (선택) Upstream 설정

원본 저장소를 `upstream`으로 등록해두면 동기화가 편합니다.

```bash
git remote add upstream https://github.com/ku-selene/ku-selene.github.io.git
```

### 2.3 로컬 서버 실행

[필요한 패키지](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll#prerequisites)를 설치하고 Jekyll 서버를 실행합니다.

```bash
bundle install
bundle exec jekyll serve
```

아래 주소로 접속하면 로컬 미리보기가 가능합니다.
👉 [http://localhost:4000](http://localhost:4000)

---

## 3. 내용 수정하기

다음 위치에서 필요한 파일을 편집합니다.

* `index.md` : 메인 페이지
* `_publications/` : 논문 목록
* `members.md` 및 `/members/` 폴더 : 멤버 페이지
* `_posts/` : 새 소식/공지
* 기타 페이지 파일들

##### 추천: 새 브랜치에서 작업하기

```bash
git checkout -b update-members
```

수정 후 로컬 서버를 새로고침하여
레이아웃이나 링크가 깨지지 않았는지 확인합니다.

##### 팁: 테마(Minima)의 원본 소스 코드 확인 및 수정 방법

랩 홈페이지는 Jekyll 기본 테마인 **Minima**를 기반으로 하고 있으며,
일부 템플릿 파일은 프로젝트 저장소에 직접 보이지 않을 수 있습니다.
이 경우, 다음 명령을 통해 **테마의 실제 소스 코드 경로**를 확인할 수 있습니다.

```shell
bundle info --path minima
```

위 명령을 실행하면 Minima 테마가 로컬에 설치된 위치가 출력됩니다.
수정하고자 하는 파일이 현재 저장소에 없더라도, 해당 경로에서 소스 파일을 확인할 수 있습니다.

만약 테마 내부 파일을 커스터마이징하고 싶다면 다음과 같이 합니다:

1. Minima 테마 경로에서 원하는 파일을 확인
2. **해당 파일을 그대로 프로젝트 저장소에 복사**

   * 예: `_layouts/default.html`, `_includes/header.html` 등
3. 복사한 파일을 원하는 대로 수정하면 프로젝트 내 파일이 테마 파일보다 **우선 적용**되어 변경 사항이 반영됩니다.

이를 통해 테마 레이아웃, 헤더/푸터, 포스트 스타일 등
원하는 부분을 자유롭게 커스터마이징할 수 있습니다.

---

## 4. 변경 사항 커밋 후 Push

```bash
git add <변경/추가/삭제된 파일들>
git commit -m "Update members page" # 예시
git push origin update-members
```

---

## 5. Pull Request(PR) 생성

1. 본인 GitHub 저장소로 이동
   (`<본인ID>/ku-selene.github.io`)
2. “**Compare & pull request**” 버튼 클릭
   또는 **Pull Requests → New pull request**
3. 다음 설정 확인
   * **base repository:** `ku-selene/ku-selene.github.io`
   * **base branch:** `main`
4. 제목과 설명을 작성하고 **Create pull request** 클릭

PR이 승인되고 병합되면 홈페이지([https://ku-selene.github.io](https://ku-selene.github.io))에 자동 반영됩니다.

---

## 6. (옵션) 원본 저장소 업데이트 가져오기

여러 번 작업하는 경우, conflict을 방지하기 위해 주기적으로 upstream 변경 사항을 반영해주세요.

```bash
git checkout main
git fetch upstream
git merge upstream/main
git push origin main
```
