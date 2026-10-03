# 홈페이지 미리 보기와 GitHub 게시

## 미리 보기

압축을 풀고 `index.html`을 더블클릭하면 메인 홈페이지를 볼 수 있습니다. 상단 **CV** 탭에서 전체 이력 페이지(`cv.html`)로 이동합니다. 별도의 프로그램 설치가 필요 없습니다. `styles.css`, `cv.css`, `assets` 폴더는 `index.html`과 같은 폴더에 두세요. 현재 홈페이지에는 프로필 사진, 두 핵심 연구의 그림, GT·SNU 로고를 표시합니다.

## GitHub에 게시하기

1. GitHub에 `yerinkim-yk` 계정으로 로그인합니다.
2. `yerinkim-yk.github.io` 저장소가 이미 있는지 확인합니다. 기존 홈페이지가 있다면 먼저 백업하세요.
3. 없다면 이름을 `yerinkim-yk.github.io`로 지정하고 **Public** 저장소를 만듭니다.
4. 저장소에서 파일 업로드를 선택하고, 압축을 푼 폴더 **안의 파일들**을 올립니다. ZIP이나 상위 폴더 자체를 올리지 마세요. `index.html`, `cv.html`, `styles.css`, `cv.css`, `assets` 폴더가 저장소 첫 화면에 보여야 합니다. `assets` 폴더도 통째로 업로드해야 사진과 그래프가 표시됩니다.
5. 숨김 폴더인 **`.github`**도 빠짐없이 업로드합니다. Mac Finder에서 **Command + Shift + .**으로 숨김 파일을 표시할 수 있습니다. `.github/workflows/pages.yml`은 홈페이지 게시에 사용됩니다. 기본 브랜치는 `main`으로 설정합니다.
6. **Settings → Pages → Build and deployment → Source**에서 **GitHub Actions**를 선택합니다.
7. **Actions → Publish homepage → Run workflow**를 선택합니다. 두 작업이 모두 성공하면 Pages 설정의 **Visit site**에서 홈페이지를 확인합니다. 이후 파일 변경 시 홈페이지가 다시 게시되며 인용 수는 자동으로 바뀌지 않습니다.

게시 성공 후 사용할 주소: `https://yerinkim-yk.github.io/`

현재 전달된 파일은 게시 준비가 된 초안이며, 실제 GitHub 업로드나 공개 배포가 완료된 상태는 아닙니다.

## 포함된 내용

- 흰 배경·파란 링크·작은 프로필 사진으로 구성한 간결한 학술형 디자인
- 산세리프 글꼴로 약간 키운 이름, 소속 바로 아래 프로필 링크, 오른쪽 사진으로 구성한 2열 상단과 그 아래 넓게 배치한 영어 자기소개
- ABB Robotics, Blux, Georgia Tech의 대표 프로젝트
- 이력서와 완전히 일치하는 연구 프로젝트명, 이력서에 근거한 설명과 최근 경험의 핵심 기여
- SLAM, 선박 충돌 회피, 크레인 MPC 제어 사례
- 연구 경험, 논문 5편, 경력·학력, 기술 역량
- 제어·ML 관련 대학원 과목, 조교·AI 교육 경험, 주요 수상과 장학금
- MILCOM·IEIE 논문의 구두 발표 표시
- 학교 이메일, GitHub, Google Scholar, LinkedIn 프로필 링크
- 모바일에서도 바로 보이는 텍스트 메뉴와 화면 크기에 맞춰 조정되는 레이아웃

첨부 이력서의 전화번호와 원본 PDF는 웹사이트에 포함하지 않았습니다. Home은 연구 정체성, 최근 연구 두 건의 짧은 설명과 그림, 논문, 업데이트를 앞에 두도록 구성했습니다. Industry Experience와 Education은 간결하게 정리했고, Teaching·Honors·Coursework·Skills는 CV에서 확인할 수 있습니다.

## 확인 상태

HTML 구조, 페이지 내 이동 링크, 파일 연결, Scholar 프로필 주소와 논문별 인용 수 연결을 점검했습니다. 연구 5개·산업체 경력 3개·논문 5편이 유지되며, Research 제목 5개를 이력서와 대조했습니다. MILCOM 논문 제목과 IEEE Xplore 링크를 연결했고, 공동저자 2명의 논문 목록에서 동일한 주소를 확인했습니다. IEEE 페이지 자체는 JavaScript 확인을 요구해 전체 화면 검증은 하지 못했습니다. JavaScript 없이 작동합니다. 브라우저의 접근 제한으로 실제 화면 및 모바일 상호작용의 자동 검증은 완료하지 못했습니다. 공개 전 브라우저에서 직접 화면을 확인해 주세요.

Google Scholar 링크는 자기소개·논문·연락처 영역에 연결했습니다. 프로필 직접 조회가 제한되어 사용자가 제공한 목록으로 논문 4편을 대조했습니다. 인용 수는 사용자가 제공한 Google Scholar 기록으로 유지합니다. MILCOM 9회, regularized policy optimization 7회, linear-quadratic control 3회이며 기록 날짜는 2026년 10월 2일입니다. 수치가 제공되지 않은 크레인 논문에는 인용 수를 표시하지 않습니다. 2021년 SVM 논문은 이력서에 근거한 별도 항목으로 유지했습니다.

자세한 수정 방법과 출처는 `README.md`에 있습니다.

[GitHub Pages 공식 안내](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site)

## 인용 수 유지

요청에 따라 인용 수 자동 갱신은 껐습니다. 매일 또는 매주 실행되는 예약 작업은 없습니다. GitHub에 게시하거나 홈페이지 파일을 수정해도 Google Scholar의 기존 9·7·3회가 다른 출처의 숫자로 바뀌지 않습니다. 인용 수를 수정할 때에는 Google Scholar에서 새 수치를 확인한 뒤 기록 날짜와 함께 직접 변경합니다.

DSVM 링크는 Publications 제목·DBpia 링크에만 연결했습니다. Research 제목은 일반 텍스트로 표시합니다.

`Resume (9).pdf`에서 연구·로보틱스·ML 커리어와 관련된 항목을 선별했습니다. CREATION상은 중복 없이 한 번 기재하고, 중복 항목의 날짜가 일치하지 않는 Eminence 장학금과 일반 봉사·체육 활동은 제외했습니다. 새 이력서의 원본 PDF는 포함하지 않았습니다.

활동 섹션은 제외했습니다. Honors & Awards의 CREATION·Wonjang·Merit-based 3개 항목을 같은 제목·기간·설명 형식으로 맞췄고, 대학원 수강 과목은 Methods & Tools 다음의 독립 섹션에서 Control·Machine learning·Optimization·Reinforcement learning별로 과목명만 표시합니다. Eminence는 이력서상 성적 우수 장학금이 맞지만 중복 기재된 수혜 학기가 달라 아직 추가하지 않았습니다.

Education의 각 학력 항목 왼쪽에 학교 공식 사이트의 로고를 추가했습니다. 로고 파일도 `assets` 폴더에 포함되어 있습니다.

## 메인 / CV 구분

- **Home (`index.html`)**: 연구 정체성, 핵심 연구 프로젝트, 논문, 업데이트, 간결한 산업체 경력과 학력. Skills는 표시하지 않습니다.
- **CV (`cv.html`)**: 간결한 연구·경력 설명, 논문, 학력, 교육·아웃리치, 수상·장학금, 분야별 대학원 수강 과목, 연락처가 포함됩니다. 이름·소속·사진·프로필 링크는 남기고 소개글은 뺐습니다.

상단 Home/CV 탭으로 두 페이지를 이동할 수 있습니다. 공유되는 논문·학력·기간 등을 수정할 때에는 두 페이지를 함께 반영해 주세요. GitHub 게시 시 두 HTML 파일을 모두 올려야 합니다.

Home과 CV의 Industry Experience 왼쪽에 ABB·Blux·DSME 로고를 추가했습니다. DSME는 근무 당시 회사명에 맞는 로고를 사용하며, 로고 파일은 `assets` 폴더에 함께 들어 있습니다.
