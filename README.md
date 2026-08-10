# 1페이지 정적 블로그

웹 페이지는 `index.html` 하나뿐입니다.

## 파일
- index.html : 유일한 웹 페이지
- posts.json : 게시글 목록 + 본문 관리
- sitemap.xml : 검색엔진 제출용
- robots.txt : 검색로봇 설정

## 새 글 추가
`posts.json` 배열 안에 아래 형식으로 한 건을 추가합니다.

```json
{
  "slug": "my-post",
  "title": "새 글 제목",
  "summary": "목록에서 보여줄 요약",
  "date": "2026-08-10",
  "category": "AI",
  "tags": ["ChatGPT", "자동화"],
  "published": true,
  "content": "<p>여기에 HTML 본문을 작성합니다.</p>"
}
```

## 배포
GitHub 저장소에 이 파일들을 올린 후 Netlify 또는 Vercel과 연결하면 됩니다.

## 꼭 수정할 것
배포 주소가 확정되면 `index.html`, `sitemap.xml`, `robots.txt` 안의
`https://example.com`을 실제 도메인으로 바꾸세요.
