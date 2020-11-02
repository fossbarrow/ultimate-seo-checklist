# HTML Elements - SEO Checklist

Tags are small snippets of HTML coding that tell engines how to properly “read” your content. In fact, you can vastly improve search engine visibility by adding SEO tags in HTML.

When a search engine’s crawler comes across your content, it takes a look at the HTML tags of the site. This information helps engines like Google determine what your content is about and how to categorize the material.

Some of them also improve how visitors view your content in those search engines. And this is in addition to how social media uses content tags to show your articles.

In the end, it’s HTML tags for SEO that will affect how your website performs on the Internet. Without these tags, you’re far less likely to really connect with an audience.

## Use Title Tags

Perhaps one of the most important HTML tags for SEO is that of the title. This is the label of your content and how searches see your page in Google and Bing. Every result you see in a search engine is derived from the title tag.

```
<title>About | Fossbarrow</title>
<title>Home | Fossbarrow</title>
```

## The Meta Tag

In terms of SEO, the `<meta>` tag is the most important tag where search engines detect what type of content your site is actually offering. This tag defines the metadata about your HTML documents. 

For example, if my webpage contains data about languages like HTML, CSS, and JavaScript and I want to provide this information to my search engine, here's the syntax: 

`<meta name="keywords" content= "HTML, CSS, JavaScript">`

If I want to describe the viewport for my website (or how my website will appear on a mobile device, tablet, or computer screen), I can add the following syntax between the `<head>` tag:

```
<head>
<meta name="viewport" content ="width=device=width, initial-scale=1.0"> 
<head>
```  
  
## Use Meta Tags

HTML uses `<meta>` tags to define metadata about a HTML document. These tags are placed inside the `<head></head>`section. Metadata is the information about your website. Metadata is not displayed on the webpage but it is parsed by web crawlers and search engines.

It has a few Attributes:

| Attribute  | Description                                            |
| ---------- | ------------------------------------------------------ |
| name       | Describes the name for the metadata                    |
| content    | Describes the value of the metadata                    |
| charset    | Describes the character encoding for the HTML document |
| http-equip | Provides the HTTP header for information               |

<br>

### Description

Defines the description about the website. The description should be up to 160 characters.

`<meta name="description" content="This is a short description about your site." >`

<br>

## Use Open Graph Meta Tags

Open Graph meta tags are snippets of code that control how URLs are displayed when shared on social media.

These are the most basic meta tags that you should use for all content types:

| Tag            | Description                                                                                                                                        |
| -------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| og:url         | Describes The canonical URL for your page. This should be the undecorated URL, without session variables,user identifying parameters, or counters. |
| og:title       | Describes the The title of your article without any branding such as your site name.                                                               |
| og:description | Describes the A brief description of the content, usually between 2 and 4 sentences.                                                               |
| og:image       | The URL of the image that appears when someone shares the content to Social media                                                                  |
| og:type        | Describes The type of media of your content.                                                                                                       |
| og:locale      | Describes The The locale of the resource.                                                                                                          |

Twitter has its own `<meta>` tags that are similar to the Open Graph protocol, but uses the “twitter” prefix instead of “og”. As with Facebook, only a few are required. The type of display format we’re requesting from Twitter is also specified:

| Tag                 | Description                                                                                                                                                                                      |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| twitter:title       | Title of content (max 70 characters)                                                                                                                                                             |
| twitter:description | Description of content (maximum 200 characters) Used with summary, summary_large_image, player cards                                                                                             |
| twitter:image       | URL of image to use in the card. Images must be less than 5MB in size. JPG, PNG, WEBP and GIF formats are supported. Only the first frame of an animated GIF will be used. SVG is not supported. |
| twitter:site        | @username of website. Either `twitter:site` or `twitter:site:id` is required.                                                                                                                    |
| twitter:card        | The card type ,Used with all cards                                                                                                                                                               |
| twitter:image:alt   | A text description of the image conveying the essential nature of an image to users who are visually impaired. Maximum 420 characters.                                                           |

<br>


## Use Robots Tag

It informs search engines which pages on your site should be indexed and which should not. Can use it to save your rankings in case you have to block some pages from indexing.

<meta name="robots" content="index, follow">

### Use of Robots Tag's Parameters

Noindex — prevents search engines from indexing a page;

Nosnippet — prevents a description of the page to appear in search results as well as prevents caching of the page;

Noarchive — prevents a cached copy of the page to appear in search results;

Nofollow — prevents the search engine from following ALL the links on the page (that's why it is different from the nofollow attribute that is applied on an individual URL level);

None — the same as "noindex, nofollow".

## Use Schema Markup
Schema markup is an information you can add to your website in microdata HTML, RDFa, or JSON-LD formats (semantic vocabulary) that helps the search engines return more informative results for users. Schema tells the search engines what your data means, not just what it says.

[Schema.org](https://schema.org/) is the centralized home on the web for the Schema project, a collaboration between Google, Bing, Yahoo! and Russian search engine Yandex to standardize structured markup.

Here is an example of a [LocalBusiness](https://schema.org/LocalBusiness):
* Without markup:
```
<h1>Beachwalk Beachwear & Giftware</h1>
A superb collection of fine gifts and clothing to accent your stay in Mexico Beach.
3102 Highway 98
Mexico Beach, FL
Phone: 850-648-4200
```

* With Microdata:
```
<div itemscope itemtype="https://schema.org/LocalBusiness">
  <h1><span itemprop="name">Beachwalk Beachwear & Giftware</span></h1>
  <span itemprop="description"> A superb collection of fine gifts and clothing
  to accent your stay in Mexico Beach.</span>
  <div itemprop="address" itemscope itemtype="https://schema.org/PostalAddress">
    <span itemprop="streetAddress">3102 Highway 98</span>
    <span itemprop="addressLocality">Mexico Beach</span>,
    <span itemprop="addressRegion">FL</span>
  </div>
  Phone: <span itemprop="telephone">850-648-4200</span>
</div>
```

* With RDFa:
```
<div vocab="https://schema.org/" typeof="LocalBusiness">
  <h1><span property="name">Beachwalk Beachwear & Giftware</span></h1>
  <span property="description"> A superb collection of fine gifts and clothing
  to accent your stay in Mexico Beach.</span>
  <div property="address" typeof="PostalAddress">
    <span property="streetAddress">3102 Highway 98</span>
    <span property="addressLocality">Mexico Beach</span>,
    <span property="addressRegion">FL</span>
  </div>
  Phone: <span property="telephone">850-648-4200</span>
</div>
```

* With JSON-LD:
```js
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "LocalBusiness",
  "address": {
    "@type": "PostalAddress",
    "addressLocality": "Mexico Beach",
    "addressRegion": "FL",
    "streetAddress": "3102 Highway 98"
  },
  "description": "A superb collection of fine gifts and clothing to accent your stay in Mexico Beach.",
  "name": "Beachwalk Beachwear & Giftware",
  "telephone": "850-648-4200"
}
</script>
```

### Author

Defines the author of the website.

`<meta name="author" content="Foo Bar" >`

### Keywords

Defines the keywords for search engines.

`<meta name="keywords" content="HTML, CSS, Javascript">`

### Viewport

Defines the viewport to make sure the website looks good on all devices.

`<meta name="viewport" content="width=device-width, initial-scale=1.0" >`

### Charset

Defines the Charset (Character Encoding) which your website uses.

`<meta charset="UTF-8" >`

## Use Body Tags

The `<body>` tag defines the document's body.
The `<body>` element contains all the contents of an HTML document, such as headings, paragraphs, images, hyperlinks, tables, lists, etc.

## Use Semantic Tags

Semantics in HTML means "role" or "purpose". When we use `<div></div>` tags they hold no meaning which is saying they are generic tags. They can hold any content inside of them but it does not provide us enough information.

Semantic Tags clearly describe the meaning of the content they contain to everyone and make it easier for search engines and web crawlers to search for information effectively.

Here are some common Semantic Tags:

| Attribute                   | Description                                                 |
| --------------------------- | ----------------------------------------------------------- |
| `<article></article>`       | describes independent, self-contained content               |
| `<aside></aside>`           | describes indirectly related content like sidebars          |
| `<code></code>`             | describes code snippets contained in web documents          |
| `<figcaption></figcaption>` | describes the content of the parent `<figure>` element      |
| `<figure></figure>`         | describes content like illustrations and diagrams           |
| `<footer></footer>`         | represents a footer for the parent element                  |
| `<header></header>`         | contains introductory content like images or heading        |
| `<main></main>`             | represents most of the content in the `body` section        |
| `<nav></nav>`               | contains navigation links to the same or any other document |
| `<section></section>`       | describes a section in a document for a particular topic    |
| `<table></table>`           | describes a table containing various types of data          |
| `<time></time>`             | represents a specific period in time                        |
| `<details></details>`       | provides additional content details for the user to view    |
| `<summary></summary>`       | describes a visible heading under the `<details>` element   |



## The href Attribute

In HTML 5, the <a> tag defines hyperlinks to locations on the same page or other pages on the Web.

The href attribute is the most important attribute of the <a> tag. The href attribute specifies a URL or URL fragment that provides the destination of the hyperlink. A URL fragment is a name preceded by a hash mark (#), which specifies an internal target location (an ID) within the current document.

For example, for creating a link back to the top of the page, you can use the special fragment "top":
`<a href="#top">Back to top</a>`
 If in HTML 5 the href attribute is not specified, the anchor element <a> represents a placeholder hyperlink.

All the time when you link to another website, your linked page gives that website some amount of rank credits. To prevent that, you need to add the rel=“nofollow” attribute to your <a> tag in HTML code. 

The “nofollow” attribute “specifies the relationship between the current document and the linked document” , namely blocks rank credits that your page might give another website. The rel=“nofollow” attribute is only used if the href attribute is present in <a> tag.

Browsers do not use “nofollow” attribute in any way; however, search engines use it to get more information about a link and to specify that the search spider should not follow that link. “Google does not transfer PageRank or anchor text across these links. Essentially, using nofollow causes us to drop the target links from our overall graph of the web.
When you are creating your website’s internal links, the “nofollow” attribute helps you to set a crawling way of your pages to Googlebot that allows you to manage rank credits from page to page within your website and prevent a crawling recirculation. 

You should make decision when to use the "nofollow" attribute for your links and when to allow search engines to follow your links. The primarily cases in which you might want to consider using “nofollow” attribute are:

 * Paid links
 * Forums
 * Comments
 * Pages you don’t want to give rank credits
 * Other “untrusted content” 4

Links is an important attribute of your website, regardless of their “follow” `<a href="www.example.com" rel="follow">Example</a>` or “nofollow” `<a href="www.example.com" rel="nofollow">Example</a>` status. Even if "nofollow" links don't boost the PageRank and don't help with a page’s placement in the search engine results, “nofollow” links still provide referral traffic.


## The src Attribute

The src attribute identifies an image by a URL. The image defined by the URL is retrieved by the browser and inserted into the document when the page loads.

There are three different kinds of URLs that can be used in the src attribute:
* Absolute URLs
This is the most straightforward, and is the only way to go if you want to link to an external image (an image hosted on another site).
`<img src="https://pt.wikipedia.org/wiki/Píton-reticulada#/media/Ficheiro:Python_reticulatus_сетчатый_питон-2.jpg">`

* Relative URLs
A relative URL does not include the domain name, and is relative to either the current page, or the current domain. If you begin the URL without a slash ( / ), it will be relative to the current page. If you begin with a slash, it will be relative to the domain.

It is almost always the best idea to use source URLs which are relative to the domain, not the page. They will not break if the page content is moved or copied.

Additionally, when linking to images on your own site, it is almost always best to use relative URLs rather than absolute URLs. This way, the URLs won’t break when you change domains which will happen automatically if you use a development or staging server in addition to your production one.
`<img src="/wp-content/uploads/piton.jpg">`

* Data URIs
It is possible to encode content into a URI string. You then use the string as if it were a URL, and then the browser simply interprets it as if it were a file.
You need a special encoding program to turn images or other files into Data URIs.
Data URIs are not usually a great solution. Most meaningful images are going to create insanely long strings  and they actually don’t load as fast as external files.
They do cut down on HTTP requests to the server, which you may (or may not) care about. They can also be useful in situations where external images might not get loaded, such as in emails or in self-contained documents to be read offline.



## Use Alt tags in Images

The alt attribute provides an “alternative description” for the image. This description is normally not presented to the user, but will be under certain circumstances:

* Assistive technology — If the user is visually impaired, and is using a screen reader, the screen reader will read the alt description to the user.
* Images turned off — Some users prefer to surf the web with images turned off (to save bandwidth or to minimize distraction). These users will normally see the alt description instead of the image.
* Image failure — If an image fails to load for any reason (bad file name, connection problems), the user will usually see the alt description in place of the image.
    
The alt description is also very helpful for search engines. Search engines have a hard time figuring out what the content of an image actually is. They are getting better at it, but identifying the subject of a photo or picture is extremely difficult. So search engines rely on the alt description to know what is actually in a picture (they also use the file name and other attributes). Additionally, in Google Image Search, the alt description is actually shown to the user.
### Example
`<img src="not-a-real-file-name.jpg" alt="Depending on your browser, you might see this message in place of the failed image.">`


## Use Header Tags

Header tags are often used to break up the content to make it easier to read. In reality, about 55% of visitors will only spend [15 seconds at most skimming your content.](https://buffer.com/resources/55-visitors-read-articles-15-seconds-less-focus-attention-not-clicks/)

Headers make it easier for these people to find what they’re looking for quickly.

Here’s an example; what if I have a reader on this blog who is merely interested in Open Graph tags? He or she can then scroll down to find the header for it and get the information.

Otherwise, the reader can simply leave the page without engaging the content at all.

In terms of SEO, header tags are also what search engines use to help determine segments of content and create [featured rich snippets](https://www.greengeeks.com/blog/why-should-you-want-your-site-to-be-in-the-google-featured-snippet/).

Here is the hierarchy of header tags:

- `<h1></h1>` – usually reserved for webpage titles.
- `<h2></h2>` – highlights the topic of the title.
- `<h3></h3>` – reflects points in regards to the topic.
- `<h4></h4>` – supports points from `<h3>`.
- `<h5></h5>` – not often used, but great for supporting points of `<h4>`.

## Using Descriptive Anchor Text

For better seo, it is better to use descriptive anchor text for internal links, instead of very short call to action links like "click here" or "this page".

`<a href="http://example.com">Good descriptive anchor text</a>`

For example you are creating a Portfolio site and you want to link to your twitter page or facebook page, make your anchor text be something like "My twitter page" or "My facebook page" or just something similar but descriptive.

If your in a situation where you need to add a particular link in multiple places, it is thought a best practice to mix up the internal link anchor text quite a bit. Something like "facebook home page" and "my Facebook page" even though they might have different anchor text names, they still link to the same page.

What is explained above comes in really handy when you have two pages that share the same link. It is very good practice to give them seperate anchor text. [You can know more here](https://backlinko.com/hub/seo/internal-links)

## Put Important Information in Lists

Lists (`<li>`) tags are a great way to break up blocks of text and highlight important content.

We have three types of lists: `<ul>`, `<ol>`, and `<dl>`.

Creating an unordered list (`<ul>`) puts them in a bullets. 
For example, the following HTML code:
```
<ul>
  <li>Milk</li>
  <li>Tea</li>
</ul>
```
will create this: 
 - Milk
 - Tea
 
Creating an ordered list (`<ol>`) on the other hand puts the items in that list in a sequential or hierarchical system.
For example, the following HTML code:
```
<ol>
  <li>Coffee</li>
  <li>Tea</li>
</ol>
```
will create this: 
1. Coffee
2. Tea

Creating a description list (`<dl>`) create a list of terms, with a description of each term immediately after it.
For example, the following HTML code:
```
<dl>
  <dt>Coffee</dt>
  <dd>black hot drink</dd>
</dl>
```
will create this: 
<dl>
  <dt>Coffee</dt>
  <dd>black hot drink</dd>
</dl>
List tags make it easier for users scanning the page to notice important information, and lists are a cue for both assistive-technology users and search engines about the significance of the content.
It is better to create true lists instead of symbols, such as dashes or hyphens as it is easier for the search engine bots to easily recognize them.

