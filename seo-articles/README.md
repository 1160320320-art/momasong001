# MOMASONG SEO Article Library

This folder stores publication-ready English SEO drafts for [momasong.com](https://momasong.com/).

## Topic folders

- `product/` — product spotlights, collection guides, wholesale assortment and OEM/ODM content
- `education/` — UPF, materials, sizing, care, quality, sourcing and buyer education
- `lifestyle/` — family beach, pool, travel and seasonal lifestyle content
- `stories/` — factory, design, retailer and brand stories

## File naming and rotation

Each draft is named `YYYYMMDD.md`. One article is generated per calendar day in Asia/Shanghai time. Categories rotate in this order:

1. Product
2. Education
3. Lifestyle
4. Stories

The rotation uses the last two digits of the date modulo four: `00` goes to Product, `01` to Education, `02` to Lifestyle, and `03` to Stories. This makes the destination deterministic for both manual and scheduled runs.

If a file for the current date already exists, do not overwrite it. Review the existing draft and report that no duplicate was created.

## Draft standard

Every article should:

- be written in natural, useful English for MOMASONG's B2B audience;
- normally be 700-1,000 words, with no filler added merely to reach a word count;
- include YAML metadata with title, slug, description, keywords, date, category, canonical URL, image and alt text;
- use one clear H1, descriptive H2/H3 headings, a short FAQ and a relevant call to action;
- open with a specific hook or buyer problem, then move quickly to practical takeaways and a clear next step;
- balance search intent with human appeal: use the primary keyword naturally in the title, introduction, one heading and conclusion, without keyword stuffing;
- use short paragraphs, concrete examples, benefit-led subheadings and a distinct point of view so the article feels useful rather than generic;
- link naturally to the MOMASONG shop, OEM/ODM, quality, size guide or contact pages;
- use only product facts and claims supported by the live website or current project data;
- use 1-3 relevant existing MOMASONG website images when they improve the article, each with descriptive alt text and placed beside the section it illustrates;
- match image type to topic: product/gallery images for Product, fabric/testing/factory images for Education, beach or accessory scenes for Lifestyle, and factory/design/team/process images for Stories;
- avoid repeating near-identical images, unrelated stock photos, decorative images with no editorial purpose, or alt text that merely repeats keywords;
- download displayed images into `assets/YYYYMMDD/` and use relative Markdown paths so they render in GitHub;
- stay a draft until a person reviews facts, target keyword, links and final URL before publishing.

## Core internal links

- Shop: https://momasong.com/shop
- OEM/ODM: https://momasong.com/oem-odm
- Quality: https://momasong.com/quality
- Size guide: https://momasong.com/size-guide
- Blog: https://momasong.com/blog
- Contact: https://momasong.com/contact

## Image storage

Keep the original website URL in YAML metadata for publishing reference. For the visible images inside the Markdown body, save a verified copy under `seo-articles/assets/YYYYMMDD/` and reference it from a category article as `../assets/YYYYMMDD/filename.webp`. Commit the article and its image files together.
