# HTMLElements - SEO Checklist

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

## Use OpenGraph Meta Tags

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

`<meta name="keyword" content="HTML CSS Javascript" >`

### Viewport

Defines the viewport to make sure the website looks good on all devices.

`<meta name="viewport" content="width=device-width, initial-scale=1.0" >`

### Charset

Defines the Charset (Character Encoding) which your website uses.

`<meta charset="UTF-8" >`

## Use Body Tags

The <body> tag defines the document's body.
The <body> element contains all the contents of an HTML document, such as headings, paragraphs, images, hyperlinks, tables, lists, etc.

## Use Semantic Tags

Semantics in HTML means "role" or "purpose". When we use `<div></div>` tags they hold no meaning which is saying they are generic tags. They can hold any content inside of them but it does not provide us enough information.

Semantic Tags clearly describe the meaning of the content they contain to everyone and make it easier for search engines and web crawlers to search for information effectively.

Here are some common Semantic Tags :

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

The <a> tag defines a hyperlink. The href attribute specifies the URL of the page the link goes to: <a href="https://www.google.com">Google</a>

## The src Attribute

The <img> tag is used to embed an image in an HTML page. The src attribute specifies the path to the image to be displayed: <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" width="300" height="300">

## Use Alt tags in Images

 The alt attribute provides an “alternative description” for the image. This description is normally not presented to the user, but will be under certain circumstances:

    * Assistive technology — If the user is visually impaired, and is using a screen reader, the screen reader will read the alt description to the user.
    * Images turned off — Some users prefer to surf the web with images turned off (to save bandwidth or to minimize distraction). These users will normally see the alt description instead of the image.
    * Image failure — If an image fails to load for any reason (bad file name, connection problems), the user will usually see the alt description in place of the image.

    ### Example

        <img src="not-a-real-file-name.jpg" alt="Depending on your browser, you might see this message in place of the failed image.">

    ##### Reference
          https://www.w3.org/QA/Tips/altAttribute
          https://www.w3schools.com/tags/att_img_alt.asp

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

## The Meta tag

In terms of SEO ,<meta> tag is the most important tag which engines us to detect what kind a content your site is actually offering . <Meta> tag defines metadata about your html documents.
If my webpage contains the data about languages like html, css and javascript and i want to provide this information to my search engine then
Here is the syntax :-

<meta name="keywords" content= "HTML,CSS,JAVASCRIPT">
If i want to describe the viewport for my website (how my website will appear). Then i'll use the following syntax in my head tag:-
<head>
<meta name="viewport" content ="width=device=width, initial-scale=1.0"> 
<head>

## Using Descriptive Anchor Text

For better seo, it is better to use descriptive anchor text for internal links, instead of very short call to action links like "click here" or "this page".

`<a href="http://example.com">Good descriptive anchor text</a>`

For example you are creating a Portfolio site and you want to link to your twitter page or facebook page, make your anchor text be something like "My twitter page" or "My facebook page" or just something similar but descriptive.

If your in a situation where you need to add a particular link in multiple places, it is thought a best practice to mix up the internal link anchor text quite a bit. Something like "facebook home page" and "my Facebook page" even though they might have different anchor text names, they still link to the same page.

What is explained above comes in really handy when you have two pages that share the same link. It is very good practice to give them seperate anchor text. [You can know more here](https://backlinko.com/hub/seo/internal-links)

## Put Important Information in Lists

Lists <li> tags are a great way to break up blocks of text and highlight important content.

We have three types of lists: <ul> and <ol> and <dl>

Creating an unordered list [<ul>] puts them in a bullets. 
For example:
<ul>
  <li>Milk</li>
  <li>Tea</li>
</ul>

Creating an ordered list [<ol>] on the otherhand puts the items in that list in a sequential or hierarchical system.
For example:
<ol>
  <li>Coffee</li>
  <li>Tea</li>
</ol>

Creating a description list [<dl>] create a list of terms, with a description of each term immediately after it.
For example: 
<dl>
  <dt>Coffee</dt>
  <dd>- black hot drink</dd>
</dl>

Lists tags make it easier for users scanning the page to notice important information, and lists are a cue for both assistive-technology users and search engines about the significance of the content.
It is better to create true lists instead of symbols, such as dashes or hyphens as it is easier for the search engine bots to easily recognize them.
