# 국영규 포트폴리오

화면과 서버, 기기와 데이터를 연결하고 그 연결을 믿을 수 있게 만드는 개발자 국영규의 포트폴리오입니다.

- 사이트: https://younggyu01.github.io/
- 메일: monst0104@naver.com

## 구성

빌드 과정이 없는 정적 사이트입니다. `index.html` 한 파일에 마크업, 스타일, 스크립트가 함께 들어 있고 외부 라이브러리를 쓰지 않습니다.

| 경로 | 내용 |
| --- | --- |
| `index.html` | 본문. 첫 화면의 케이블, 프로젝트별 시연 장면, 쉬운 말/기술 용어 전환 |
| `404.html` | 없는 주소로 들어왔을 때 보이는 화면 |
| `assets/` | 글꼴, 실제 화면 이미지, 시연 영상, 공유 미리보기 이미지(`og.png`) |
| `.nojekyll` | GitHub Pages가 Jekyll 처리 없이 파일을 그대로 올리게 하는 빈 파일 |

## 로컬에서 보기

```bash
python -m http.server 8000
```

실행한 뒤 http://localhost:8000 을 엽니다.

## 내용 고치기

- 실제 화면, 시연 영상, 저장소 링크: `index.html` 스크립트의 `MEDIA`에서 `src`, `href`를 고칩니다. 값이 비어 있는 항목은 화면에 나오지 않습니다.
- 이력서: PDF를 `assets/`에 넣고 `RESUME`에 경로(예: `./assets/resume.pdf`)를 적으면 상단과 연락 칸에 이력서 버튼이 생깁니다.
- 사이트 주소: 주소가 바뀌면 `index.html` 머리말의 `https://younggyu01.github.io/` 네 곳과 `404.html`의 두 곳을 함께 바꿉니다.

## 글꼴

[Wanted Sans](https://github.com/wanteddev/wanted-sans)를 SIL Open Font License 1.1에 따라 함께 배포합니다. 라이선스 전문은 `assets/WantedSans-OFL.txt`에 있습니다.
