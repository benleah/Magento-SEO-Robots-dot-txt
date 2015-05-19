# Magento Robots.txt boilerplate

A starter template for your Magento installation's Robots.txt file. Promotes a better SEO ready behaviour for Magento stores by helping to (conserve crawl budget)[http://searchengineland.com/how-i-think-crawl-budget-works-sort-of-59768] and reduce scope for search bots indexing (light or duplicate content)[https://moz.com/blog/fat-pandas-and-thin-content].

### Installation

Simply save this file to your Magento web root and update with any additional routes, directories and files created by your installed plugins for pages that don't add specific search value according to your content strategy (for example, pages that are largely just forms or perhaps have only thin and generic system content).

### Robots.txt Gotchas

In pretty much all cases you will want to allow robots full access to the `/skin/`, `/js/` and `/lib/` directories so they can access your static frontend assets. Google have long noted that blocking Googlebot from your CSS and JavaScript files will have a detrimental impact on how your site is indexed and ultimately SERP performance.

### Image Crawling

The user agent `Googlebot-Image` is only granted access to crawl the `/media/wysiwyg/` and `/media/catalog/` directories (i.e. content images traditionally uploaded via the CMS or Manage Product pages) to prevent crawling of UI images and any structural images store in `/skin/` that might otherwise waste crawl budget.