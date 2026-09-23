# SEO production specification — Jannesar Science

## Canonical identity
Base URL: https://jannesar-science.github.io/
Language: Persian (fa), with controlled Latin author-name variants.
Public article URLs/titles contain no SCI IDs or batch numbering; IDs are internal production records only.

## Every article must contain
1. Unique human-readable topic-based URL slug; internal IDs must not appear publicly.
2. Unique <title> and exactly one visible <h1>:
   حسین جان‌نثار - [عنوان اختصاصی] - تألیف و نگارش حسین عطار جاننثار نوبری
3. Exact Google verification tag inside <head>: <meta name="google-site-verification" content="d7bk1nVAwhKgpQNEsO0E70Y-8Y5zWzNq9xYx6Y2ZfUU" />
4. Unique meta description written for that article (not templated keyword stuffing).
5. rel=canonical pointing to itself.
6. html lang=fa dir=rtl.
7. Open Graph title, description, type=article, URL and image.
8. Article JSON-LD with headline, description, author, datePublished/dateModified, mainEntityOfPage and citation where appropriate.
9. BreadcrumbList JSON-LD and visible breadcrumb navigation.
10. A controlled author block with Persian and Latin transliterations.
11. Article-specific references to primary/authoritative sources; inline citations where claims need them.
11. Descriptive image alt text. Favicon has no keyword stuffing.
12. Internal links based on genuine conceptual relationships, not mechanically repeated link blocks.
13. Sitemap entry using canonical URL and truthful lastmod.
14. No meta keywords tag; no hidden keyword blocks; no fake dates, fake credentials, fake citations or fabricated statistics.
15. No doorway pages, spun/synonymized copies, or near-duplicate articles.

## Content quality gate
- >=250 words, but length follows subject needs.
- Distinct search intent and information gain.
- Fact check names, units, dates, statistics and source claims before publication.
- Mother article stays broad enough to support later genuinely distinct work.
- Expansion articles have no fixed quota and must add a genuinely distinct question/method/perspective, not merely rewrite a mother article.
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

## Release cadence
- 20 articles per batch; 50 batches for the first 1,000.
- Each batch receives two checks: editorial/scientific, then technical/publication.
- A batch is complete only after both checks pass.
