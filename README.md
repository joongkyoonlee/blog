# 1페이지 Markdown 정적 블로그

웹 페이지는 `index.html` 하나뿐이며, 게시글 본문은 Markdown(`.md`) 파일로 관리합니다.

## 폴더 구조

```text
index.html
posts.json
sitemap.xml
robots.txt
posts/
  2026-08-10-welcome.md
```

## 새 글 작성 방법

1. `posts/` 폴더에 `.md` 파일을 만듭니다.
2. `posts.json`에 글의 메타데이터와 `file` 경로를 추가합니다.
3. GitHub에 push합니다.
4. 연결된 Vercel/Netlify가 자동 재배포합니다.

### posts.json 예시

```json
{
  "slug": "my-post",
  "title": "새 글 제목",
  "summary": "목록에 보일 요약",
  "date": "2026-08-10",
  "category": "AI",
  "tags": ["ChatGPT", "자동화"],
  "published": true,
  "file": "posts/my-post.md"
}
```

## 현재 최초 게시글

- `posts/2026-08-10-welcome.md`
- 제목: `블로그를 시작하며`

## 배포 주소 확정 후

`index.html`, `sitemap.xml`, `robots.txt` 안의 `https://example.com`을 실제 Vercel/Netlify 또는 커스텀 도메인 주소로 변경하세요.
