# STRUCTURE — ourstudio-today-sample

## 배포
- 레포: github.com/Daorl8/ourstudio-today-sample → Cloudflare 연결(사용자 단계) → ourstudio-today-sample.lgt3232.workers.dev
- 단일 파일 정적 사이트. `wrangler.toml`(name=ourstudio-today-sample, [assets] directory="./") + `.assetsignore`(실내용).

## 파일
- `index.html` — 전체 사이트(CSS·JS 인라인). 단일 파일.
- `os-hero.jpg` — 히어로 가족 컷(분할 히어로 우측).
- `os-01.jpg ~ os-34.jpg` — 갤러리/마퀴 공용 self-host 컷(다양한 색감·피사체). 매핑은 `_manifest.json`(원본 IG 파일명, 서빙 제외).
- `os-logo.png` — 투명 로고(초록 카메라+새싹, 헤더/모바일). `os-mark.png` — 카메라 마크 크롭(예비).
- `CHANGELOG.md` / `STRUCTURE.md` / `_manifest.json` — 문서(서빙 제외).

## 섹션 순서
헤더 → #top/히어로 → 마퀴 → #about → #gallery → #price → #info → #location → 푸터 → 모바일 퀵바.

## 폰트
- Nanum Myeongjo(디스플레이, Google CDN) + Pretendard(본문, jsdelivr CDN). 폴백=안전 산세리프(궁서 방지). 납품 확정 시 self-host 전환 예정.

## 색
- bg #F7F4ED / paper #fff / ink #24261F / green #5E7249(액센트) / green-d #495A38 / sage #9DB187.

## 원본 소스
- IG 원본 107장은 상위 폴더 `ourstudio_today/`에 보관, 레포엔 os-*만 커밋.
