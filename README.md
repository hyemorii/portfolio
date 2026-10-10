# 이혜민 — Sports Event Portfolio

한국어 중심의 반응형 스포츠 이벤트 기획·운영 포트폴리오입니다. Vite와 기본 JavaScript/CSS로 구성했습니다.

## 실행

Node.js 20.19+ 또는 22.12+가 필요합니다. 현재 환경에서 Node.js 24.19.0으로 확인했습니다.

```sh
cd /workspace/portfolio
npm ci --cache /tmp/portfolio-npm-cache --no-audit --no-fund
npm run dev -- --port 5173
```

프로덕션 빌드: `npm run build`. 결과는 `dist/`에 생성됩니다. 정적 호스팅에 배포할 수 있으며 프로젝트 상세는 해시 경로를 사용하므로 별도 서버 라우팅이 필요 없습니다.

## 내용 수정

- `src/data.js`: 네 프로젝트의 내용·기간·규모·숫자·작업물 목록
- `src/main.js`: Hero, About, Experience, Contact 및 상세 화면 구성
- `src/style.css`: 레이아웃, 색상, 반응형 스타일

이미지는 현재 모두 #000000 Placeholder입니다. 실제 작업물을 추가할 때 `public/images/`에 파일을 넣고 `src/data.js`의 해당 media 항목 `src: null`을 `src: '/images/파일명.jpg'`로 바꿉니다. `label`도 실제 사진을 설명하는 내용으로 수정하세요. 추가 media 항목으로 사진을 더 넣을 수 있습니다. Hero 이미지는 `src/main.js`의 `hero-media` 항목에서 교체합니다.

## 내용 검토

근거 자료는 사용자가 제공한 제작 요청 문서입니다. 별도 이력서나 프로젝트 자료는 제공되지 않았습니다. 프로젝트 기간, 학력, 사용 도구, 언어 수준·자격, 이메일은 확인 후 보완해야 합니다. 전화번호와 미제공 SNS는 노출하지 않습니다. 대회 규모는 개인 성과와 구분했으며 동아리 +133%는 9명 대비 학기 말 21명의 증가율을 반올림한 수치입니다. 세계선수권 외 연령별 대회 의료 통역은 해당 대회·기간 확인 필요로 분리했습니다.

Google Fonts를 사용할 수 없는 환경에서는 시스템 글꼴로 표시됩니다. 실제 이미지는 포함하지 않았습니다.

## 검증

`npm run build` 통과. Chromium에서 1440, 768, 390, 320px 뷰포트의 4개 상세 페이지 이동·돌아가기·Contact 이동·가로 넘침 여부·검정 Placeholder 및 직접 상세 링크를 검증했습니다. 자동 검증 도구는 앱 의존성에 포함하지 않았습니다.
