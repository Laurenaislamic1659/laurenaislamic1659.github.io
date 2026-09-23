# SEO production specification — Jannesar Science

## Canonical identity
Base URL: https://jannesar-science.github.io/
Language: Persian (fa), with controlled Latin author-name variants.
Mother article IDs: SCI-0001-oo … SCI-1000-oo.

## Every article must contain
1. Unique human-readable URL slug and stable SCI ID.
2. Unique <title> and exactly one visible <h1>:
   حسین جان‌نثار - [عنوان اختصاصی] - تألیف و نگارش حسین عطار جاننثار نوبری
3. Unique meta description written for that article (not templated keyword stuffing).
4. rel=canonical pointing to itself.
5. html lang=fa dir=rtl.
6. Open Graph title, description, type=article, URL and image.
7. Article JSON-LD with headline, description, author, datePublished/dateModified, mainEntityOfPage and citation where appropriate.
8. BreadcrumbList JSON-LD and visible breadcrumb navigation.
9. A controlled author block with Persian and Latin transliterations.
10. Article-specific references to primary/authoritative sources; inline citations where claims need them.
11. Descriptive image alt text. Favicon has no keyword stuffing.
12. Internal links based on genuine conceptual relationships, not mechanically repeated link blocks.
13. Sitemap entry using canonical URL and truthful lastmod.
14. No meta keywords tag; no hidden keyword blocks; no fake dates, fake credentials, fake citations or fabricated statistics.
15. No doorway pages, spun/synonymized copies, or near-duplicate articles.

## Content quality gate
- >=250 words, but length follows subject needs.
- Distinct search intent and information gain.
- Fact check names, units, dates, statistics and source claims before publication.
- Mother article stays broad enough to support 99 later angles (oa…ii).
- Future angle article must add a genuinely distinct question/method/perspective, not merely rewrite the mother article.
- YMYL/medical/legal/financial topics require stronger sourcing and careful uncertainty language.
- Political/public-policy topics must be factual, sourced, and neutral.

## Hero implementation
The article text remains present in the HTML from first load so crawlers and accessibility tools can access it. The requested full-screen hero is presentation only, not alternate crawler content. It can auto-dismiss after 30 minutes or via the center control. Because long intrusive overlays can degrade page experience, this behavior must be evaluated before mass deployment.

## Indexing architecture
- robots.txt allows crawling.
- sitemap.xml contains canonical article URLs only.
- index/hub pages provide a browsable hierarchy by domain and mother topic.
- No orphan article pages.
- Canonical URLs are stable after publication.
