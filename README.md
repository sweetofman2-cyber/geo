# 애니워터 — AI 검색 미노출 문제점 & 해결방안

풀페이지 슬라이드 방식의 프레젠테이션 웹사이트입니다.

## 로컬 실행

```bash
# 그냥 index.html을 브라우저로 열거나
open public/index.html

# 또는 간단한 서버로
npx serve public
```

## Vercel 배포

### 방법 1 — Vercel CLI

```bash
npm i -g vercel
vercel
```

### 방법 2 — GitHub 연동

1. GitHub에 이 폴더를 올리기
   ```bash
   git init
   git add .
   git commit -m "첫 커밋"
   git remote add origin https://github.com/내아이디/anywater-site.git
   git push -u origin main
   ```
2. [vercel.com](https://vercel.com) → New Project → GitHub 저장소 선택
3. **Root Directory**: `public` 으로 설정
4. Deploy 클릭 → 자동 배포 완료!

## 폴더 구조

```
anywater-site/
├── public/
│   ├── index.html      ← 메인 사이트
│   └── images/
│       ├── 1.jpg  (문제점 5)
│       ├── 2.jpg  (타이틀)
│       ├── 3.jpg  (문제점 1)
│       ├── 4.jpg  (문제점 2)
│       ├── 5.jpg  (문제점 3)
│       └── 6.jpg  (문제점 4)
└── vercel.json
```

## 조작 방법

| 동작 | 설명 |
|------|------|
| 마우스 휠 | 다음/이전 슬라이드 |
| ← → 방향키 | 다음/이전 슬라이드 |
| 화면 좌우 버튼 | 다음/이전 슬라이드 |
| 우측 점(dot) | 특정 슬라이드로 이동 |
| 터치 스와이프 | 모바일에서 좌우 스와이프 |
