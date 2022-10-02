# What is GoogleBot?

[Googlebot](https://developers.google.com/search/docs/crawling-indexing/googlebot) is a web crawler (a.k.a., robot or spider) that scrapes data from webpages.

Googlebot is just one of many web crawlers. Every search engine has its own branded spider.

In the SEO world, these branded bots are referred to as “user agents”.

User agents will be discussed later; just understand that user agents refer too specific web crawling bots.

Some of the most common user agents include:

- Googlebot – Google
- Bingbot – Bing
- Slurp Bot – Yahoo
- Alexa Crawler – Amazon Alexa
- DuckDuckBot – DuckDuckGo

# How Does Googlebot Work?

To optimize for Googlebot, one must understand how it discovers, reads and ranks web pages.

## How Google’s Crawler Discovers Webpages?

**Short answer:** Links, sitemaps, and fetch requests.
<br>

**Long answer:** The fastest way to get Google to crawl a website is to create a new property in Search Console and submit the sitemap.

However, while sitemaps are a great way to get Google to crawl your website, this does not account for PageRank.

Internal linking is a recommended method for telling Google which pages are related and hold value.

Google can also discover your webpages from Google My Business listings, directories, and links from other websites.

This is a simplified version of how Googlebot works. To learn more, see the [Google’s documentation](https://support.google.com/webmasters/answer/70897?hl=en).

## How Googlebot Reads Webpages?

The goal of Googlebot is to render a webpage the same way a user would see it.

To test how Google views a page, check out the Fetch and Render tool in Search Console. This provides a "Googlebot view" vs. "User view" which is useful for finding out how Googlebot views your web pages.

## Technical Ranking Factors

Just like traditional SEO, there is no silver bullet to technical SEO. All [200+ ranking factors](https://www.searchenginejournal.com/google-200-ranking-factors-facts/265085/) are important!

If you are a technical SEO professional thinking about the future of SEO, then the biggest ranking factors to pay attention to revolve around user experience.

## Why Should We Think Like Googlebot?

For Google to recommend a website, the latter has proved to have passed a number of GoogleBot requirements; this usually equates to a high quality website.

Most users do not browse through multiple pages of search results; they only look at the highest rated results.

As such, a website that satisfies both users with intuitive User Interface (UI) and User Experience (UX) while also satisfying GoogleBot requirements will experience more organic growth compared to one that does not.

### User Experience vs. Crawler Experience

When creating a website, who are you looking to satisfy? Users or Googlebot?

**Short answer**: Both!
<br>

**Long answer**: This is a hot debate that can cause tension between UI/UX designers, web developers, and SEO professionals. However, this is also an opportunity to work together to better understand the balance between user experience and crawler experience.

UI/UX designers typically have users’ best interests in mind, while SEO professionals are looking to satisfy GoogleBot requirements. Somwehere in the middle, web developers are trying to create the best of both worlds.

As SEO professionals, we need to learn the importance of each area of the web experience.

Yes, we should be optimizing for the best user experience. However, we should also optimize our websites for Googlebot (and other search engines).

Why? Because often times, new users are referred to the website via a search engine such as Google but the user will only remain on the website if the user experience is without issues.

Luckily, Google is very user-focused. Most modern SEO tactics are focused on providing a good user experience.

The following 10 Googlebot optimization tips should help win over UX designers and web developers at the same time.

## 1. Robots.txt

<hr>
The `robots.txt` is a plain text file placed in the root directory of a website. These are one of the first things that Googlebot looks for when crawling a site. It is highly recommended to add a robots.txt to websites and to include links to `sitemap.xml`.

There are many ways to optimize your robots.txt file, but it is important to take caution in doing so.

A developer may accidentally leave a sitewide disallow in robots.txt, blocking all search engines from crawling sites when moving a dev site to the live (production) site; even after correction, it may take a few weeks before a crawler tries again and eventually indexes the website. This hurts traffic and site rankings.

There are many tips and tutorials available online, on how to optimize robots.txt. Do your research before attempting to edit it. Don’t forget to track the results!

## 2. sitemap.xml

<hr>
Sitemaps are a key method for Googlebot to find pages on your website and are considered an important ranking factor.

Here are a few sitemap optimization tips:

- Only have one sitemap index.
- Separate blogs and general pages into separate sitemaps, then link to those on your sitemap index.
- Don’t make every single page a high priority.
- Remove 404 and 301 pages from your sitemap.
- Submit your sitemap.xml file to Google Search Console and monitor the crawl.

## 3. Site Speed

<hr>
The quickness of loading has become one of the most important ranking factors, especially for mobile devices. If the load speed of a website is too slow, Googlebot may lower its rankings.

An easy way to find out if Googlebot thinks your website loads too slow is to test your site speed with any of the free tools out there.

Many of these tools will provide recommendations that may be passed onto developers for implementing changes.

## 4. Schema

<hr>
Adding structured data to your website can help Googlebot better understand the context of your individual web pages and website as a whole. However, it’s important that you follow [Google’s guidelines](https://developers.google.com/search/docs/appearance/structured-data/sd-policies).

For efficiency, it is recommended that to use [JSON-LD](https://json-ld.org/) to implement structured data markup. Google has even noted that JSON-LD is their preferred markup language.

## 5. Canonicalization

<hr>
A big problem for large sites, especially e-commerce, is the issue of duplicate web pages.

There are many practical reasons to have duplicate web pages, such as different language pages.

If you’re running a site with duplicate pages, it’s crucial that you identify your preferred webpage with a canonical tag and hreflang attribute.
