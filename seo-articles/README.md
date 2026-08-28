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
- link naturally to the MOMASONG shop, OEM/ODM, quality, size guide or contact pages;
- use only product facts and claims supported by the live website or current project data;
- use 1-3 relevant existing MOMASONG website images when they improve the article, each with descriptive alt text;
- avoid unrelated stock images and avoid adding images only to fill space;
- stay a draft until a person reviews facts, target keyword, links and final URL before publishing.

## Core internal links

- Shop: https://momasong.com/shop
- OEM/ODM: https://momasong.com/oem-odm
- Quality: https://momasong.com/quality
- Size guide: https://momasong.com/size-guide
- Blog: https://momasong.com/blog
- Contact: https://momasong.com/contact
