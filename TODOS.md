# TODOS

## Deferred Features

### 댓글 시스템 (Giscus)
- **What:** 블로그 포스트에 댓글 기능 추가
- **Why:** 독자와 소통 채널. 검색으로 들어온 사람이 질문/피드백 남길 수 있음
- **How:** Giscus (GitHub Discussions 기반). PaperMod에서 partial 오버라이드로 추가. hugo.yaml에 giscus 설정
- **Depends on:** GitHub repo Settings에서 Discussions 활성화 필요
- **Added:** 2026-04-08 (eng review)

### 검색 기능 (Fuse.js)
- **What:** 사이트 내 전체 텍스트 검색
- **Why:** 글이 쌓이면 특정 주제 찾기 어려움. 10개+ 포스트부터 유용
- **How:** PaperMod 기본 지원. hugo.yaml에 `outputs.home`에 JSON 추가, `params.fuseOpts` 설정
- **Depends on:** 없음
- **Added:** 2026-04-08 (eng review)
