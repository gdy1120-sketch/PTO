# 2027 달력 (GitHub Pages)

2027년 1~12월을 이전/다음 버튼으로 탐색합니다. `dates.json`에 입력한 단일 날짜 및 날짜 범위(양 끝 포함)는 빨간색, 나머지는 초록색입니다.

## 날짜 수정
- `dates`: `"2027-01-15"` 같은 단일 날짜 목록
- `ranges`: `{ "start": "2027-04-10", "end": "2027-04-20" }` 같은 기간 목록
- 날짜는 `YYYY-MM-DD` 형식으로 입력합니다. 중복 또는 겹치는 범위도 표시에는 문제가 없습니다.
- `dates.json`은 공개 파일입니다. 민감한 정보를 넣지 마세요.

## GitHub Pages 배포
1. GitHub에서 새 **Public** 저장소를 만듭니다.
2. 이 ZIP 파일의 `index.html`과 `dates.json`을 저장소 최상위에 업로드합니다.
3. **Settings → Pages → Build and deployment → Deploy from a branch**를 선택합니다.
4. Branch는 `main`, Folder는 `/(root)`로 설정하고 저장합니다.
5. 잠시 후 Pages에 표시되는 주소로 접속합니다.

날짜를 바꾸려면 GitHub에서 `dates.json`을 편집하고 Commit changes를 누르세요. 배포가 갱신되면 방문자에게도 반영됩니다.

## 로컬 미리보기
파일을 더블클릭하여 `file://`로 열면 브라우저 보안 정책 때문에 JSON 로딩이 차단될 수 있습니다. 로컬 서버에서 확인하세요.

```bash
python -m http.server 8000
```

그다음 `http://localhost:8000`에 접속합니다.
