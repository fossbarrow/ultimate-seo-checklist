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

| Tag             | Description                                               |
| ----------      | ------------------------------------------------------    |
| og:url          | Describes The canonical URL for your page. This should be 
                    the undecorated URL, without session variables, 
                    user identifying parameters, or counters.                 |
| og:title        | Describes the The title of your article without any 
                    branding such as your site name.                          |
| og:description  | Describes the A brief description of the content, 
                    usually between 2 and 4 sentences.                        |
| og:image        | The URL of the image that appears when someone 
                    shares the content to Facebook                            |
| og:type         | Describes The type of media of your content.              |
| og:locale       | Describes The The locale of the resource.                 |

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

## The href Attribute

The <a> tag defines a hyperlink. The href attribute specifies the URL of the page the link goes to: <a href= www.Google.com>Google</a>

## The src Attribute

The <img> tag is used to embed an image in an HTML page. The src attribute specifies the path to the image to be displayed: <img src="Github_Logo.jpg">

## Use Alt tags in Images

Search engines cannot determine what images are trying to convey. That’s when the ALT tag comes into play. The ALT represents what the image is : <img src="Github_Logo.jpg" alt="Github Logo">