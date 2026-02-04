# GraphAI.io SEO 및 사이트 점검 리포트

**점검일:** 2026년 2월 4일
**대상 URL:** https://graphai.io/
**플랫폼:** WordPress (All in One SEO v4.9.3)

---

## 📊 종합 점수

| 항목 | 상태 | 점수 |
|------|------|------|
| 기본 SEO 설정 | ✅ 양호 | 75/100 |
| 기술적 SEO | ✅ 양호 | 80/100 |
| 소셜 미디어 최적화 | ⚠️ 개선 필요 | 50/100 |
| 크롤링/인덱싱 | ✅ 양호 | 90/100 |

---

## 1. 메타 태그 분석

### 메인 페이지 (https://graphai.io/)

| 항목 | 상태 | 내용 |
|------|------|------|
| **Title** | ✅ | "그래파이 \| 기업 AI를 위한 풀스택 데이터 솔루션" |
| **Meta Description** | ✅ | "그래파이는 Akasic 시리즈를 통해 차세대 DB 엔진과 AI 에이전팅 엔진을 완벽하게 통합 최적화합니다..." |
| **H1** | ✅ | "데이터에서 의사결정까지 책임지는, 기업 AI 내재화를 위한 최적의 선택" |
| **lang 속성** | ✅ | ko-KR |
| **Viewport** | ✅ | 설정됨 |
| **Favicon** | ✅ | 512x512px PNG |

### 서브 페이지 상태

| 페이지 | Title | Meta Description | H1 |
|--------|-------|------------------|-----|
| /about/ | ✅ "About - 그래파이" | ❌ 미설정 | ✅ |
| /contact/ | ✅ "CONTACT - 그래파이" | ❌ 미설정 | ✅ |
| /products/ | ⚠️ 확인 필요 | ⚠️ 확인 필요 | ⚠️ |
| /solutions/ | ⚠️ 확인 필요 | ⚠️ 확인 필요 | ⚠️ |

---

## 2. Open Graph & 소셜 미디어 태그

### 현재 상태

| 항목 | 메인 페이지 | 서브 페이지 |
|------|-------------|-------------|
| og:type | ✅ WebPage | ✅ |
| og:url | ✅ 설정됨 | ✅ |
| og:title | ✅ 설정됨 | ✅ |
| og:description | ✅ 설정됨 | ⚠️ 일부 미설정 |
| og:image | ⚠️ 확인 필요 | ⚠️ 확인 필요 |
| og:site_name | ⚠️ 확인 필요 | ⚠️ |

### Twitter Card 태그

| 항목 | 상태 |
|------|------|
| twitter:card | ❌ 미설정 |
| twitter:title | ❌ 미설정 |
| twitter:description | ❌ 미설정 |
| twitter:image | ❌ 미설정 |

---

## 3. 구조화 데이터 (JSON-LD)

### ✅ 설정된 스키마

```
- Organization (회사 정보, 로고, LinkedIn 프로필)
- WebSite (사이트 정보)
- WebPage (페이지별 정보)
- BreadcrumbList (탐색 경로)
```

### 권장 추가 스키마

- `LocalBusiness` - 회사 위치/연락처 정보
- `FAQPage` - FAQ 페이지가 있다면
- `Product` - 제품 페이지에 제품 스키마

---

## 4. robots.txt 분석

**URL:** https://graphai.io/robots.txt

```
User-agent: *
Disallow: /wp-admin/
Allow: /wp-admin/admin-ajax.php

Sitemap: https://graphai.io/sitemap.xml
Sitemap: https://graphai.io/sitemap.rss
```

| 항목 | 상태 | 비고 |
|------|------|------|
| 기본 설정 | ✅ 양호 | 모든 크롤러 허용 |
| wp-admin 차단 | ✅ 양호 | 보안상 적절 |
| Sitemap 등록 | ✅ 양호 | XML + RSS 모두 등록 |

---

## 5. Sitemap 분석

**URL:** https://graphai.io/sitemap.xml

### Sitemap 구조

| 파일 | 마지막 수정 | 용도 |
|------|-------------|------|
| page-sitemap.xml | 2026-02-04 | 정적 페이지 (10개) |
| post-sitemap.xml | 2026-02-04 | 블로그 포스트 (12개) |
| category-sitemap.xml | 2026-02-04 | 카테고리 |

### 등록된 페이지 (page-sitemap.xml)

| URL | Priority | Change Freq |
|-----|----------|-------------|
| / (메인) | 1.0 | always |
| /products/akasicon/ | 0.7 | weekly |
| /products/akasicin/ | 0.7 | weekly |
| /products/akasicdb/ | 0.7 | weekly |
| /products/akasicai/ | 0.7 | weekly |
| /products/ | 0.7 | weekly |
| /solutions/ | 0.7 | weekly |
| /about/ | 0.7 | weekly |
| /contact/ | 0.7 | weekly |
| /news/ | 0.7 | weekly |

### ⚠️ 발견된 이슈

1. **중복 콘텐츠 의심**: `/news/` 와 `/main02_news/` 경로에 동일한 콘텐츠가 중복 존재
   - 예: `한국경제신문-그래파이-기사-보도` vs `한국경제신문-그래파이-기사-보도-2`

2. **URL에 한글 사용**: 일부 뉴스 URL에 한글이 인코딩 없이 사용됨
   - SEO에는 영향 없으나 공유 시 URL이 길어질 수 있음

---

## 6. 페이지 속도 (Core Web Vitals)

> ⚠️ **주의**: 실시간 측정 데이터는 직접 확인이 필요합니다.

### 확인 방법

**Google PageSpeed Insights에서 직접 테스트:**
```
https://pagespeed.web.dev/analysis?url=https%3A%2F%2Fgraphai.io%2F
```

### 주요 측정 항목

| 지표 | 설명 | 권장 기준 |
|------|------|----------|
| **LCP** (Largest Contentful Paint) | 최대 콘텐츠 렌더링 | < 2.5초 |
| **FID** (First Input Delay) | 첫 입력 지연 | < 100ms |
| **CLS** (Cumulative Layout Shift) | 누적 레이아웃 이동 | < 0.1 |
| **FCP** (First Contentful Paint) | 첫 콘텐츠 렌더링 | < 1.8초 |
| **TTFB** (Time to First Byte) | 첫 바이트 시간 | < 800ms |

### 확인된 최적화 요소

- ✅ 이미지 Lazy Loading 적용
- ✅ 반응형 이미지 (srcset) 사용
- ⚠️ JavaScript/CSS 최적화 확인 필요

---

## 7. 모바일 친화성

| 항목 | 상태 |
|------|------|
| Viewport 메타 태그 | ✅ 설정됨 |
| 반응형 디자인 | ✅ 적용됨 |
| 터치 타겟 크기 | ⚠️ 직접 확인 필요 |
| 폰트 크기 | ⚠️ 직접 확인 필요 |

**확인 도구:** https://search.google.com/test/mobile-friendly

---

## 8. 보안 (HTTPS)

| 항목 | 상태 |
|------|------|
| HTTPS 적용 | ✅ |
| HTTP → HTTPS 리다이렉트 | ✅ (확인 필요) |
| Mixed Content | ⚠️ 직접 확인 필요 |

---

## 🔴 긴급 개선 필요 사항

### 1. 서브 페이지 Meta Description 추가
- `/about/` 페이지
- `/contact/` 페이지
- 모든 제품 페이지

### 2. Twitter Card 태그 전체 추가
```html
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:site" content="@graphai">
<meta name="twitter:title" content="페이지 제목">
<meta name="twitter:description" content="페이지 설명">
<meta name="twitter:image" content="https://graphai.io/og-image.png">
```

### 3. og:image 최적화
- 1200x630px 전용 소셜 공유 이미지 제작
- 각 주요 페이지별 맞춤 이미지 설정

---

## 🟡 권장 개선 사항

### 1. Canonical URL 명시
- 모든 페이지에 `<link rel="canonical">` 태그 추가
- 중복 콘텐츠 이슈 방지

### 2. 중복 콘텐츠 정리
- `/main02_news/` 경로의 중복 게시물 정리
- 또는 canonical 태그로 원본 지정

### 3. 구조화 데이터 확장
- 제품 페이지에 `Product` 스키마 추가
- Contact 페이지에 `LocalBusiness` 스키마 추가

### 4. 이미지 Alt 텍스트 점검
- 모든 이미지에 설명적인 alt 텍스트 확인
- 키워드 포함하되 자연스럽게

### 5. 내부 링크 구조 최적화
- 주요 페이지 간 상호 링크 확인
- Breadcrumb 네비게이션 시각적 구현

---

## 📋 체크리스트

### 필수 항목
- [ ] 모든 페이지 Meta Description 추가
- [ ] Twitter Card 태그 설정
- [ ] og:image 1200x630px 이미지 제작
- [ ] Canonical URL 태그 추가
- [ ] Google Search Console 등록 확인
- [ ] Google Analytics 설치 확인

### 권장 항목
- [ ] PageSpeed Insights 90+ 달성
- [ ] 중복 콘텐츠 (/main02_news/) 정리
- [ ] 제품 페이지 Product 스키마 추가
- [ ] 404 페이지 커스터마이징
- [ ] XML Sitemap Google Search Console 제출

---

## 📚 참고 도구

| 도구 | URL | 용도 |
|------|-----|------|
| Google Search Console | https://search.google.com/search-console | 인덱싱 관리 |
| PageSpeed Insights | https://pagespeed.web.dev | 속도 측정 |
| Mobile-Friendly Test | https://search.google.com/test/mobile-friendly | 모바일 테스트 |
| Rich Results Test | https://search.google.com/test/rich-results | 구조화 데이터 |
| Schema Markup Validator | https://validator.schema.org | 스키마 검증 |

---

*리포트 생성: Claude Code*
*https://claude.ai/code/session_0157SEQu2Mja9Q7Uxmrm9U8j*
