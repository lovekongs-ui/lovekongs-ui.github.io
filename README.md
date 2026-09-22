# 김서연 AI/ML 포트폴리오

HTML·CSS·JavaScript로 동작하는 정적 사이트입니다. 외부 폰트·라이브러리·API·유료 서비스·백엔드·빌드 명령이 필요하지 않으며, AGAMI 로고와 시연 영상은 같은 폴더의 로컬 파일을 사용합니다.

## 업로드할 파일

- `index.html`: 실제 사이트. 파일명은 소문자로 유지합니다.
- `아가미로고.png`: AGAMI 프로젝트 로고입니다.
- `시연영상_아가미.mp4`: AGAMI 실제 서비스 시연 영상입니다.
- `portfolio-preview.png`: 링크 공유 시 표시되는 포트폴리오 첫 화면 미리보기입니다.
- `README.md`: 이 안내서. 함께 업로드해도 됩니다.
- `.nojekyll`: Jekyll 처리를 건너뛰는 빈 파일. 함께 업로드하는 것을 권장합니다.

`portfolio-source.md`, `CODEX-PROMPT.txt`, `qa/`는 사이트 실행에 필요하지 않습니다. `qa/`에는 로컬 검증 기록이 있으며 업로드 대상이 아닙니다. 한글 파일명 두 개는 `index.html`과 같은 위치에 그대로 업로드합니다.

## GitHub에 직접 업로드하고 Pages 설정하기

공개 사이트: https://lovekongs-ui.github.io/ · 저장소: https://github.com/lovekongs-ui/lovekongs-ui.github.io

2026-09-22에 GitHub 공식 안내를 확인했습니다. 현재 사이트는 `main` 브랜치의 루트에서 게시됩니다. 아래는 직접 다시 업로드하거나 별도 저장소를 만들 때의 안내입니다.

1. GitHub에 로그인하고 **New repository**를 선택합니다. 원하는 저장소 이름을 입력합니다. 무료 계정으로 이 방식의 Pages를 사용하려면 **Public**을 선택합니다. **Add README**를 켜고 저장소를 생성합니다. 기존 저장소도 사용할 수 있습니다. [공식 사이트 생성 안내](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site)
2. 저장소의 **Code → Add file → Upload files**에서 위 파일을 올립니다. 폴더 전체가 아니라 **폴더 안의 파일**을 올려 `index.html`이 저장소 최상위에 보이게 합니다. 커밋 설명을 작성하고 **Commit changes**로 저장합니다. 기존 README를 업로드본으로 교체해도 됩니다. 숨김 파일이 보이지 않으면 `.nojekyll`은 **Add file → Create new file**로 같은 이름의 빈 파일을 만들 수 있습니다. [공식 파일 업로드 안내](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository)
3. **Settings → Pages → Build and deployment**에서 **Source: Deploy from a branch**를 선택합니다.
4. 파일을 올린 브랜치(일반적으로 `main`)와 **/(root)**를 선택하고 **Save**를 누릅니다. 별도 Actions 설정 파일이나 빌드 명령은 필요하지 않습니다. [공식 게시 소스 설정 안내](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
5. 저장소 **Actions**에서 Pages 실행 결과를 확인합니다. 완료 후 **Settings → Pages**가 표시하는 실제 사이트 주소를 엽니다. 주소는 계정·저장소 설정에 따라 달라지므로 여기서 배포 주소를 추정하지 않습니다.
6. 배포된 주소에서 메뉴, 프로젝트 상세, 연락처 링크를 다시 확인합니다. 이후 `index.html` 수정본을 같은 브랜치에 업로드하면 다시 게시됩니다.

## 배포가 안 될 때

- **404**: 파일명이 정확히 `index.html`인지 확인합니다. `Index.html`, `index.html.txt` 또는 저장소 안에 한 단계 더 들어간 폴더는 이 설정과 맞지 않습니다. Pages에서 선택한 브랜치와 `/(root)`에 실제 파일이 있어야 합니다. [공식 404 점검 안내](https://docs.github.com/en/pages/getting-started-with-github-pages/troubleshooting-404-errors-for-github-pages-sites)
- **게시 실패**: Actions에서 가장 최근 Pages 실행의 실패 단계와 로그를 확인합니다. Settings의 Pages 권한·게시 소스·브랜치를 확인하고, GitHub 이메일 인증과 저장소 관리 권한을 확인합니다. 서비스 장애는 [GitHub Status](https://www.githubstatus.com/)에서 확인할 수 있습니다.
- **예전 화면**: 최신 커밋의 배포 완료 여부를 확인한 뒤 새로고침하거나 캐시를 비우고 확인합니다. 저장소 파일 보기 주소 대신 Pages 설정에 표시된 주소를 사용합니다.
- **하위 경로**: 내부 `#앵커`와 상대 경로의 로고·영상으로 저장소 하위 경로에서도 동작합니다. 공유 미리보기 메타데이터는 현재 공개 사이트의 절대 URL을 사용하므로 다른 주소로 옮기면 함께 변경합니다.
- **외부 링크만 실패**: GitHub 프로필과 AGAMI는 별도 서비스입니다. 주소가 원고와 같은지, 해당 서비스가 운영 중인지 별도로 확인합니다. 이메일·전화는 기기의 메일·전화 앱 설정에 따라 열립니다.

## 내용과 조작

- 사실 기준은 `portfolio-source.md`입니다. 6개 프로젝트의 역할·기간·팀 규모를 유지했습니다.
- 99.16% = Flashlight 3-Round Bot Block Rate, 88.04% = Flashlight 단일 모델 Accuracy, 5.94% → 0.53% = Emotion CAPTCHA Qwen Attack Pass Rate입니다.
- DART 개인 기여는 파싱·구조화·공통 스키마·정정공시 연결 로직으로 한정했습니다.
- 첫 화면은 `MAKE DATA. MAKE SENSE.`의 큰 타이포그래피와 원색 CSS 도형 디자인입니다. AGAMI에는 실제 서비스 시연 영상을 사용하며, 상세 페이지의 기여 설명과 프로젝트 맥락을 담은 기술 소개는 유지합니다.
- 프로젝트 제목/상세 버튼은 클릭, Enter, Space로 펼치거나 닫습니다. Tab으로 링크와 버튼을 이동하며, 첫 번째 포커스는 본문 바로가기입니다.
- **애니메이션 끄기** 버튼이 눌린 상태(`aria-pressed=true`)이면 움직임이 꺼집니다. 시스템의 `prefers-reduced-motion: reduce`가 우선이며 이때 버튼은 현재 상태를 보여주고 변경하지 않습니다. 시스템 설정을 해제하면 페이지 내 수동 설정으로 돌아갑니다. 수동 설정은 새로고침 시 초기화됩니다.
- 도형의 진입·스크롤 회전과 버튼 이동은 제거했습니다. 모션을 끄면 제한된 포인터 반응과 부드러운 스크롤을 멈춥니다. 읽기 진행선과 상세 열림 아이콘은 상태 표시로 즉시 갱신됩니다.
- JavaScript를 꺼도 내용·링크·상세 펼침은 사용할 수 있습니다.

## 검증 기록

로컬 작업 폴더의 `qa/DESIGN-REVIEW.md`에 화면 진단표, 편집 내역, 프로젝트별 확인 필요 자료와 검증 범위를 기록했습니다. `qa/`는 공개 저장소 업로드에서 제외합니다. 사이트는 더블클릭으로 열어도 되며 검증에는 로컬 HTTP 서버를 사용했습니다. 실제 휴대전화에서도 최종 확인하세요.
