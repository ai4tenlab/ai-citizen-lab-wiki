# AI시민연구소 블로그

AI시민연구소의 공익형 AI 리터러시 GitHub Pages 블로그입니다.

- **운영 원칙:** 매일 AI 관련 후보 주제 5개를 조사하고, 시민에게 가장 유익한 1개를 선정해 발행
- **글쓰기 기준:** AEO·GEO·AIO·SGE·EEAT, High-Entity, 일반인 눈높이, AI 냄새 제거
- **브랜드 철학:** AI는 인간 잠재력을 가속하는 도구이며, 정보 격차를 줄이는 공익 인프라
- **배포:** GitHub Pages

## 자동 발행 흐름

1. 매일 08:00 KST Hermes cron 실행
2. 최근 24~48시간 내 공식·신뢰 출처 조사
3. 후보 주제 5개 생성
4. 공익성·시민성·실용성·시의성 기준으로 1개 선정
5. `_posts/YYYY-MM-DD-slug.md` 작성
6. Git commit/push
7. GitHub Pages URL 검증
