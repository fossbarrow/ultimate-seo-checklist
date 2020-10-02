# What is GoogleBot?

Googlebot is a web crawler (a.k.a., robot or spider) that scrapes data from webpages.

Googlebot is just one of many web crawlers. Every search engine has their own branded spider. In the SEO world, we refer to these branded bot names as “user agents.”

We will get into user agents later, but for now, just understand that we’re referring to user agents as a specific web crawling bot. Some of the most common user agents include:

* Googlebot – Google
* Bingbot – Bing
* Slurp Bot – Yahoo
* Alexa Crawler – Amazon Alexa
* DuckDuckBot – DuckDuckGo

# How Does Googlebot Work?

We can’t start to optimize for Googlebot until we understand how it discovers, reads, and ranks webpages.

## How Google’s Crawler Discovers Webpages?
**Short answer:** Links, sitemaps, and fetch requests.
<br>

**Long answer:** The fastest way for you to get Google to crawl your site is to create a new property in Search Console and submit your sitemap. However, that’s not the whole picture.

While sitemaps are a great way to get Google to crawl your website, this does not account for PageRank.

Internal linking is a recommended method for telling Google which pages are related and hold value. There are many great articles published across the web about page rank and internal linking, so I won’t get into it now.

Google can also discover your webpages from Google My Business listings, directories, and links from other websites.

This is a simplified version of how Googlebot works. To learn more, you can read [Google’s documentation](https://support.google.com/webmasters/answer/70897?hl=en) on their crawler.

## How Googlebot Reads Webpages?
Google has come a long way with their site rendering. The goal of Googlebot is to render a webpage the same way a user would see it.

To test how Google views your page, check out the Fetch and Render tool in Search Console. This will give you a Googlebot view vs. User view. This is useful for finding out how Googlebot views your webpages.

## Technical Ranking Factors
Just like traditional SEO, there is no silver bullet to technical SEO. All [200+ ranking factors](https://www.searchenginejournal.com/google-200-ranking-factors-facts/265085/) are important!

If you’re a technical SEO professional thinking about the future of SEO, then the biggest ranking factors to pay attention to revolve around user experience.

## Why Should We Think Like Googlebot?
When Google tells us to make a great site, they mean it. Yes, that’s a vague statement from Google, but at the same time, it’s very accurate.

If you can satisfy users with an intuitive and helpful website, while also appeasing Googlebot’s requirements, you may experience more organic growth.

### User Experience vs. Crawler Experience
When creating a website, who are you looking to satisfy? Users or Googlebot?

**Short answer**: Both!
<br>

**Long answer**: This is a hot debate that can cause tension between UX designers, web developers, and SEO pros. However, this is also an opportunity for us to work together to better understand the balance between user experience and crawler experience.

UX designers typically have users’ best interest in mind, while SEO professionals are looking to satisfy Google. In the middle, we have web developers trying to create the best of both worlds.

As SEO professionals, we need to learn the importance of each area of the web experience.

Yes, we should be optimizing for the best user experience. However, we should also optimize our websites for Googlebot (and other search engines).

Luckily, Google is very user-focused. Most modern SEO tactics are focused at providing a good user experience.

The following 10 Googlebot optimization tips should help you win over your UX designer and web developer at the same time.

## 1. Robots.txt
<hr>
The robots.txt is a text file that is placed in the root directory of a website. These are one of the first things that Googlebot looks for when crawling a site. It’s highly recommended to add a robots.txt to your site and include a link to your sitemap.xml.

There are many ways to optimize your robots.txt file, but it’s important to take caution doing so.

A developer might accidentally leave a sitewide disallow in robots.text, blocking all search engines from crawling sites when moving a dev site to the live site. Even after this is corrected, it could take a few weeks for organic traffic and rankings to return.

There are many tips and tutorials on how to optimize your robots.txt file. Do your research before attempting to edit your file. Don’t forget to track your results!

## 2. sitemap.xml
<hr>
Sitemaps are a key method for Googlebot to find pages on your website and are considered an important ranking factor.

Here are a few sitemap optimization tips:

* Only have one sitemap index.
* Separate blogs and general pages into separate sitemaps, then link to those on your sitemap index.
* Don’t make every single page a high priority.
* Remove 404 and 301 pages from your sitemap.
* Submit your sitemap.xml file to Google Search Console and monitor the crawl.

## 3. Site Speed
<hr>
The quickness of loading has become one of the most important ranking factors, especially for mobile devices. If your site’s load speed is too slow, Googlebot may lower your rankings.

An easy way to find out if Googlebot thinks your website loads too slow is to test your site speed with any of the free tools out there.

Many of these tools will provide recommendations that you can send to your developers.

## 4. Schema
<hr>
Adding structured data to your website can help Googlebot better understand the context of your individual web pages and website as a whole. However, it’s important that you follow Google’s guidelines.

For efficiency, it’s recommended that your use JSON-LD to implement structured data markup. Google has even noted that JSON-LD is their preferred markup language.

## 5. Canonicalization
<hr>
A big problem for large sites, especially ecommerce, is the issue of duplicate webpages.

There are many practical reasons to have duplicate webpages, such as different language pages.

If you’re running a site with duplicate pages, it’s crucial that you identify your preferred webpage with a canonical tag and hreflang attribute.

