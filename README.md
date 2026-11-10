# knitup 뜨개동네 홈페이지

https://app.knitup.co.kr — GitHub Pages(main 브랜치 루트)로 배포.

- `index.html` : 홈페이지 (시안: Claude Design 캔버스 '뜨개동네 홈페이지 시안')
- `fonts/` : 털실체(Teolsil-Bold)
- `privacy.html` · `terms.html` · `guidelines.html` · `support.html` · `delete-account.html` : 앱 저장소(knit-neighbors/docs) 법적 문서 사본 — 원본이 바뀌면 여기도 함께 갱신할 것
- `CNAME` : app.knitup.co.kr (카페24 DNS CNAME app → yesbeyesnono.github.io)

## 문서 5개는 여기서 고치지 않는다 (2026-11-10)
`privacy.html` · `terms.html` · `guidelines.html` · `support.html` · `delete-account.html` 의 원본은 앱 저장소
[yesbeyesnono/knit-neighbors](https://github.com/yesbeyesnono/knit-neighbors) 의 `docs/` 이다.
이 저장소에서는 `.github/workflows/sync-legal.yml` 이 매일 한 번(03:10 KST) 가져와 덮어쓴다. 바로 맞추려면
`gh workflow run sync-legal.yml -R yesbeyesnono/knitup-home`.
홈페이지를 다시 만들어 올릴 때도 이 5개 파일은 건드리지 말 것(옛 사본으로 덮어쓰면 다시 어긋난다).
홈페이지 파일 수정·올리기는 앱 코딩 세션 한 곳에서만 한다.
