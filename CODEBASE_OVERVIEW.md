# Codebase Overview

이 저장소는 GitHub Pages + Jekyll(Minima) 기반의 정적 기술 블로그입니다.

## 핵심 파일/디렉터리

- `_config.yml`: 사이트 전역 메타데이터/플러그인/테마 설정
- `index.markdown`: 홈 화면 (`layout: home`) + 최신 글 목록
- `about.markdown`: 소개 페이지
- `_posts/`: 날짜 기반 게시물 저장소 (`YYYY-MM-DD-title.md`)
- `404.html`: 기본 에러 페이지
- `Gemfile`, `Gemfile.lock`: 로컬 빌드/서빙용 Ruby 의존성

## 렌더링 구조

1. Jekyll가 `_config.yml`을 읽고 사이트 설정을 로드
2. Minima 테마 레이아웃 적용
3. `_posts/`의 게시물을 시간 역순으로 홈 목록에 노출
4. 각 게시물은 개별 permalink로 상세 페이지 렌더링
