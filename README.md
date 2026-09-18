# 일영역 · 교외선 통합안내 웹페이지

GitHub Pages에 바로 올릴 수 있는 정적 웹페이지입니다.

## 폴더 구성
- `index.html` : 메인 페이지
- `assets/` : 국문/영문 포스터 이미지 및 시간표 이미지
- `.nojekyll` : GitHub Pages에서 정적 파일 그대로 서비스하기 위한 빈 파일

## GitHub Pages 배포
1. GitHub에서 새 저장소(repository)를 만듭니다.
2. 이 폴더의 `index.html`, `assets` 폴더, `.nojekyll` 파일을 저장소 최상위에 업로드합니다.
3. 저장소의 **Settings → Pages**로 이동합니다.
4. **Build and deployment → Deploy from a branch**를 선택합니다.
5. Branch를 `main`, Folder를 `/(root)`로 선택하고 Save 합니다.
6. 잠시 후 표시되는 `https://계정명.github.io/저장소명/` 주소로 접속합니다.

## 의견보내기 연결
`index.html` 하단 `<script>`에서 아래 두 값 중 하나를 입력하세요.

```js
const FEEDBACK_EMAIL = '받을메일@example.com';
const FEEDBACK_URL = ''; // Google Forms 등을 쓸 경우 여기에 링크
```

Google Forms를 이용하려면 `FEEDBACK_URL`에 폼 주소를 넣고 `FEEDBACK_EMAIL`은 비워두면 됩니다.

## 포함된 미디어 링크
- BTS `Spring Day` 공식 MV: https://www.youtube.com/watch?v=xEeFrLSkMm8
- 촬영지 참고: 양주시 공식 안내 페이지

## 참고
- 현재 시간표는 제공받은 이미지 그대로 사용합니다. 운행 변경 시 `assets/timetable-uijeongbu.png`, `assets/timetable-daegok.png` 파일만 같은 이름으로 교체하면 됩니다.
- 국문/영문 전환 시 운임·관광·안전 포스터가 자동으로 전환됩니다.
