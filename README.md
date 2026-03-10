# GitHub Pages 배포 가이드 (dduonthetop)

## 1) 업로드할 파일
- `index.html`

## 2) GitHub 저장소 준비
1. GitHub에서 `dduonthetop` 계정으로 새 저장소 생성 (예: `automatic-dangjik-web`)
2. 저장소 루트에 `index.html` 업로드

## 3) Pages 활성화
1. 저장소 `Settings` -> `Pages`
2. `Build and deployment`에서 `Deploy from a branch` 선택
3. Branch를 `main` / folder는 `/ (root)` 선택 후 Save
4. 몇 분 뒤 배포 URL 확인 (예: `https://dduonthetop.github.io/automatic-dangjik-web/`)

## 4) 커스텀 도메인 연결
1. `Settings` -> `Pages` -> `Custom domain`에 도메인 입력 후 Save
2. 도메인 DNS에서 아래 중 해당 방식 설정
- 루트 도메인(`example.com`) 사용 시: A 레코드를 GitHub Pages IP로 설정
- 서브도메인(`app.example.com`) 사용 시: CNAME을 `dduonthetop.github.io`로 설정
3. `Enforce HTTPS` 활성화

## 5) 주의사항
- GitHub Pages는 정적 호스팅이라 서버 실행은 불가합니다.
- 현재 구현은 브라우저(클라이언트)에서 직접 xlsx를 처리합니다.
- 원본 엑셀 스타일/서식은 일부 유지되지 않을 수 있습니다.
