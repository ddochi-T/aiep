# AIEP 학교관리자 실습실

교사·학생·학적관리 업무를 가상 데이터로 연습하는 사이트입니다.
별도 설치, 빌드, 서버, API 키가 필요 없는 HTML/CSS/JavaScript 파일입니다.

## GitHub에 올리기

1. GitHub에서 새 저장소를 만듭니다. 이름 예: `aiep-practice`.
2. 내려받은 ZIP 파일을 컴퓨터에서 압축 해제합니다.
3. 저장소의 **Add file → Upload files**에서 압축을 푼 폴더 **안의 파일과 폴더**를 모두 올립니다.
   - `index.html`, `student.html`, `academic.html`, `assets`, `downloads`가 저장소 최상위에 있어야 합니다.
   - ZIP 파일 자체를 올리거나, 이 파일들을 상위 폴더 하나에 넣어 올리지 마세요.
   - `assets`, `downloads`의 폴더 구조와 파일 이름을 유지합니다.
4. **Commit changes**로 저장합니다.
5. **Settings → Pages → Build and deployment**에서 다음과 같이 설정합니다.
   - Source: **Deploy from a branch**
   - Branch: **main** (파일을 올린 브랜치가 다르면 해당 브랜치)
   - Folder: **/(root)**
   - **Save**
6. 배포가 완료되면 Pages 설정에 표시된 주소로 접속합니다.
   - 예: `https://사용자이름.github.io/aiep-practice/`

GitHub Free에서는 공개(Public) 저장소에서 Pages를 사용할 수 있습니다.
`.nojekyll`도 포함했습니다. 숨김 파일이 업로드 목록에 나타나지 않아도 현재 파일 구조는 기본 Pages 빌드에서 사용할 수 있습니다.

공식 안내: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## 포함된 실습

| 화면 | 파일 | 주요 내용 |
| --- | --- | --- |
| 교사 실습 | `index.html` | 승인, 반려 사유 입력·확인, 회원 정보 수정, 비밀번호 초기화 |
| 학생 실습 | `student.html` | 개별·일괄 등록, 아이디 생성·수정, 비밀번호 변경, 엑셀 다운로드, 전출·삭제 |
| 학적관리 | `academic.html` | 진급, 전출·졸업, 실패 건 재실행, 전입, 처리 결과 확인 |

- 서울연습초등학교의 가상 계정으로 진행합니다.
- 실제 AIEP 시스템이나 NEIS에 연결하지 않습니다.
- 진학관리 중1 절차는 포함하지 않았습니다.
- 엑셀 연습 파일 9개가 `downloads/`에 포함되어 있습니다.
- 노란색 안내를 따라 실습하며, 각 화면의 ‘처음부터’ 버튼으로 해당 실습을 초기화합니다.
- 실습 진행은 사용한 기기의 해당 브라우저에 저장됩니다. 기기·브라우저가 다르면 별도로 진행합니다.
- 기존 사이트에서 진행한 기록은 새 GitHub Pages 주소로 자동 이전되지 않습니다.

## 컴퓨터에서 바로 실행

폴더 구조를 유지한 상태에서 `index.html`을 Chrome 또는 Edge로 열면 됩니다.
학생·학적관리 탭과 엑셀 다운로드도 함께 사용할 수 있습니다.

## 파일 구성

- `index.html`, `student.html`, `academic.html`: 실습 화면
- `assets/`: 스타일 및 실행 코드, 포함된 JSZip 라이브러리
- `downloads/`: 가상 학생·학적 연습용 XLSX 파일
- `.nojekyll`: GitHub Pages 정적 파일 배포 설정

JSZip v3.10.1은 원본 저작권·라이선스 안내를 포함한 상태로 동봉했습니다.
https://github.com/Stuk/jszip
