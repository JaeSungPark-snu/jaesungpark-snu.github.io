# Jaesung Park — 개인 홈페이지

간결한 학술 홈페이지입니다. GitHub Pages가 Markdown을 웹페이지로 변환합니다.
일상적인 내용 수정에는 프로그램 설치가 필요하지 않습니다.

홈페이지 주소: <https://jaesungpark-snu.github.io/>

## 내용을 수정하는 방법

GitHub 저장소에서 아래 파일을 열고 **연필 아이콘(Edit this file)**을 누릅니다.
내용을 수정한 뒤 **Commit changes**를 누르면 저장됩니다.
상단의 `---` 사이에 있는 설정은 그대로 두고 그 아래 본문을 수정하세요.

| 바꾸려는 내용 | 수정할 파일 |
| --- | --- |
| 소개, 연구 관심사, 소식 | `index.md` |
| 논문 목록 | `papers.md` |
| 발표 목록 | `talks.md` |
| 강의 목록 | `teaching.md` |
| CV 페이지의 내용 | `cv.md` |
| 이름, 소속, 이메일, 사진 경로, 외부 링크 | `_config.yml` |
| 메뉴 이름과 순서 | `_data/navigation.yml` |
| 글꼴, 색상, 여백 | `assets/css/style.css` |

각 목록에는 작성 예시가 HTML 주석(`<!-- ... -->`) 안에 들어 있습니다.
예시를 복사해서 주석 밖에 붙이고 실제 내용으로 바꾸세요.
주석 안의 예시는 화면에 표시되지 않지만 **공개 저장소의 소스에서는 누구나 볼 수 있습니다**.

## 프로필 사진 넣기

1. 사진 파일을 `assets/img/profile.jpg`로 업로드합니다.
2. `_config.yml`에서 `profile_image: ""`를 아래처럼 바꿉니다.

```yaml
profile_image: "/assets/img/profile.jpg"
```

세로 사진(가로:세로 약 4:5)이 잘 맞습니다. 사진을 설정하지 않으면 이니셜이 표시됩니다.
다른 확장자를 사용하면 설정에도 실제 파일명을 적으세요. 파일명은 대소문자를 구분합니다.

## CV PDF 넣기

1. PDF를 `assets/files/cv.pdf`로 업로드합니다.
2. `_config.yml`을 아래처럼 수정합니다.

```yaml
cv_pdf: "/assets/files/cv.pdf"
```

CV 페이지에 PDF 링크가 표시됩니다. 파일을 넣기 전에는 안내 문장만 표시됩니다.
Google Scholar나 ORCID 주소도 `_config.yml`에 넣으면 홈 화면에 링크가 나타납니다.

## 처음 GitHub Pages에 올리기

1. `JaeSungPark-snu` 계정에서 **Public** 저장소 `jaesungpark-snu.github.io`를 만듭니다.
2. 이 폴더 안의 파일과 폴더를 저장소 최상위에 업로드합니다.
   `_config.yml`, `index.md`, `_layouts`, `_data`, `assets`가 같은 단계에 있어야 합니다.
   ZIP 파일 자체를 업로드하지 마세요. 먼저 압축을 풀어야 합니다.
3. 저장소의 **Settings → Pages**로 이동합니다.
4. **Source: Deploy from a branch**, **Branch: main**, **Folder: / (root)**를 선택하고 **Save**를 누릅니다.
5. **Actions**에서 Pages 배포가 성공하면 홈페이지 주소를 엽니다.
   배포에 최대 10분 정도 걸릴 수 있습니다.

이 홈페이지는 Jekyll을 사용하므로 `.nojekyll` 파일을 추가하지 마세요.
`README.md`와 `Gemfile`은 웹페이지에 포함되지 않습니다.

## Markdown 간단 예시

```markdown
## 2026

### Paper title
**Jaesung Park** and Coauthor. *Journal*, year.

[arXiv](https://arxiv.org/abs/실제논문번호) · [Code](https://github.com/실제저장소)
```

## 내 컴퓨터에서 미리 보기 (선택)

Ruby와 Bundler가 설치되어 있다면 이 폴더에서 실행합니다.

```bash
bundle install
bundle exec jekyll serve
```

브라우저에서 <http://localhost:4000>을 엽니다.
GitHub 웹에서 내용만 수정할 때는 이 과정이 필요하지 않습니다.

디자인 참고: <https://cherrrycooky.github.io/>. 레이아웃과 스타일은 새로 작성했습니다.
타인의 사진, 논문 목록, 추적 코드, 사이트 인증 정보는 포함하지 않았습니다.

GitHub 공식 안내: <https://docs.github.com/en/pages/quickstart>
