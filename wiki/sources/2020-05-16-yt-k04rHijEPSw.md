---
type: youtube-video
source_date: 2020-05-16
url: https://www.youtube.com/watch?v=k04rHijEPSw
channel: "@neilpatel"
ingested: 2026-07-19
tier: L2
domains: [seo]
tags: [site-audit, ubersuggest, technical-seo, redirects, backlinks, schema-markup, sitemaps, google-search-console]
---

# How To Do An SEO Site Audit - On-page SEO Part 3 - SEO Unlocked

## Summary
Neil Patel teaches how to run an SEO site audit, mostly through Ubersuggest so it doesn't have to be done manually, as part three of his on-page SEO series in the SEO Unlocked course. He starts with baseline checks — using the `site:yourdomain.com` Google operator to confirm indexation and gauge how many pages are indexed, then ensuring there's only one canonical version of the site (https over http, and a single www or non-www version handled by the CMS) — before moving into Ubersuggest's traffic overview and, centrally, its Site Audit report. He explains reading the audit by severity (critical errors first, then warnings, then recommendations) for the biggest "bang for buck," and walks through the specific issues it surfaces: duplicate/overlong title tags, redirect types (favoring 301 over 302 and avoiding redirect loops), HTTP error codes (400/403/404/500), thin content, missing image alt tags, unique meta descriptions, internal linking to top pages, and a backlinks/anchor-text review to spot and disavow spammy links. He closes on schema markup (via Google's Structured Data Markup Helper), sitemap submission and robots.txt review in Google Search Console, overall site structure, and a manual-actions penalty check, then points viewers to worksheets and templates at neilpatel.com/training. Throughout he reassures beginners not to feel overwhelmed and previews the next lesson on finding topic ideas that generate traffic.

## Key claims
- The starting point of a site audit is confirming indexation with the Google search operator `site:yourdomain.com`; ideally you see hundreds or thousands of results, whereas zero or a single result signals a problem (as of 2020-05-16).
- Google doesn't always index every page, so a very large site (e.g. a million pages) may only show a fraction (e.g. 100,000–200,000) indexed in the `site:` results (as of 2020-05-16).
- A site should have only one canonical version; because Google mainly ranks sites with SSL certificates for security reasons, only the https version should be visible, and the CMS should be configured to serve a single www or non-www version (as of 2020-05-16).
- Ubersuggest's traffic overview (traffic analyzer) shows traffic and keyword rankings over time and lets you compare against competitors; new sites with little SEO will show no results initially, which is expected (as of 2020-05-16).
- Ubersuggest's Site Audit report gives an overview of critical errors, warnings, and recommendations; green indicates healthy, while orange/pink/gray/black indicate problems needing fixes (gray redirects may be acceptable depending on redirect type) (as of 2020-05-16).
- You should audit the whole site rather than a subset of pages, because fixing only some pages limits ranking gains (as of 2020-05-16).
- Fix audit issues in priority order — critical errors first, then warnings, then recommendations — to get the biggest traffic gain per unit of effort (as of 2020-05-16).
- Title tags should be unique and not overly long; duplicative titles across many pages are bad because they don't tell Google which page is unique or which should rank for which keyword (as of 2020-05-16).
- Ubersuggest's audit includes a "What is this and how do I fix it?" link on errors that explains the issue and links to articles on how to fix it (as of 2020-05-16).
- 301 redirects are preferred; they tell Google a page has permanently moved and to transfer the links and equity, whereas 302s signal a temporary, uncertain move and give Google a "fuzzy answer" (as of 2020-05-16).
- Use only one redirect per page and avoid redirect loops (page A → page B → back to page A), which confuse users; 302s should not be used for longer than about three months (as of 2020-05-16).
- HTTP error codes to fix: a 400 means users can't reach the page, 403 means the page is not authorized, 404 means not found (redirect these with 301s), and 500 is an internal/server error to hand to a technical team member (as of 2020-05-16).
- Thin content (not enough text on a page) should be fixed where it makes sense, though some pages like about or contact pages legitimately have little text and don't need thousands of words (as of 2020-05-16).
- Every page reviewed should have unique title tags and unique meta descriptions, and images should have alt tags that describe the image so Google can understand it — important because image search is popular in niches like travel (as of 2020-05-16).
- Ubersuggest's top pages report shows the pages (yours or a competitor's) getting the most Google traffic, giving ideas for content to create and internal linking targets; you should link to your popular pages throughout the site so they rank even higher (as of 2020-05-16).
- Backlinks matter because more linking sites generally help rankings, but not all links are equal — links should be unique, relevant, within content, and beneficial to people; paying for links is bad, short-sighted, and can lead to penalties and ranking drops (as of 2020-05-16).
- In Ubersuggest's backlinks report you should review anchor text (the keyword in the link) to check it matches the linked page; spammy, unnatural links from unrelated sites (e.g. adult, casino, or pharmaceutical sites linking to an unrelated business) warrant investigation and possible removal (as of 2020-05-16).
- Mismatched anchor text is a signal to investigate the linking page further, not to remove the link immediately; if the site looks legitimate and relevant, keep it (as of 2020-05-16).
- For bad or broken links, reach out to the linking site and ask for removal; if they won't remove it after repeated attempts, use Google's Disavow tool to upload a disavow file telling Google to ignore those links (as of 2020-05-16).
- Schema markup supplies structured data (e.g. recipe images, review ratings, cook times) from your site's code so Google can display rich results; most sites can use structured data, and Google's Structured Data Markup Helper lets non-technical users generate the code via a WYSIWYG editor (as of 2020-05-16).
- In Google Search Console you should submit a sitemap listing all your pages to maximize the chance of indexing (though Google may still not index every page), and review robots.txt (viewable at yourdomain.com/robots.txt) to ensure no important pages are being blocked from crawling (as of 2020-05-16).
- Site structure matters: strong internal linking that connects related pages boosts rankings, and linking to top pages drives more traffic, social shares, and backlinks over time (as of 2020-05-16).
- Finally, check for penalties by reviewing manual actions in Google Search Console and fixing any issues detected (as of 2020-05-16).
- Neil Patel provides worksheets and templates at neilpatel.com/training, including an SEO audit checklist and Excel sheets for auditing your own and competitors' performance (as of 2020-05-16).

## Notable verbatim quotes
> today I'm going to teach you how to do an SEO site audit.

> go to Google and type in site, colon, and put in your domain .com.

> If you're using an SSL certificate, which I mention is previous lessons, that's very, very important because Google's mainly ranking sites that have SSL certificates, it's for security purposes, you should only see https version of your website.

> The green stuff is good, that's healthy, anything that is orange or pinkish in color, or gray or black is not good.

> Typically, when you're doing SEO, you want to fix the stuff on the critical errors tab first, then warnings, then recommendations. By going in that order, you're going to get the biggest bang for buck when it comes to increasing your traffic.

> 301s tell Google this page has moved, transfer all the links, transfer all the equity, rank this page really high in Google. 302 is like, "Hey, we're temporarily not right here right now, "but we don't know when we're coming back." That's giving Google a fuzzy answer

> Thin content means there's not enough text on a page, and you won't be able to fix every page that's thin in content because some of them, like your about page, you're not going to have 5000 words on your about page.

> Image alt tags tell Google, "Hey, this is what this image is about."

> Backlinks, really important factor because the more sites linking to you, the better you're going to do as well. But not all links are equal, some are bad, some are good.

> You don't want to pay people for links either, that's really bad. It's short-sighted, it can also lead to penalties and decreases in rankings if Google finds out you're doing that.

> In other words, you're telling Google, yes, I tried getting these sites to stop linking to me, they won't, but please ignore these links and don't count it against me.

> A sitemap tells Google, "Hey, here are all the pages on my website, "make sure you index as many as you can."

> That internal linking really helps boost your rankings. If you're not doing a ton of internal linking, you're not going to do as well.
