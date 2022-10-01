# Why the Robots file is important

The robots.txt file, also known as the robots exclusion protocol or standard, is a text file that tells web robots (most often search engines) which pages on your site to crawl.


It also tells web robots which pages not to crawl.

The standard specifies how to inform the web robot about which areas of the website should not be processed or scanned.
Robots are often used by search engines to categorize websites. Not all robots cooperate with the standard; email harvesters, spambots, malware and robots that scan for security vulnerabilities may even start with the portions of the website where they have been told to stay out. The standard can be used in conjunction with Sitemaps, a robot inclusion standard for websites.


Let’s say a search engine is about to visit a site. Before it visits the target page, it will check the robots.txt for instructions.

## Disallowing user agents
The format for disallowing user agents is as follows: `User-agent: <user-agent-name> Disallow: <url-string-to-disallow>`

You can use a wildcard(`*`) for the **user-agent-name** in order to match any and all user-agents. If you leave the **disallow string** blank, you're giving the web-crawler permission to crawl through the entirety of your website. Therefore, the most open rule would be `User-agent: * Disallow: `, and the most restrictive rule would be `User-agent: * Disallow: /`

You can restrict different parts of your website by specifying a url/directory within your website. For example, having: `User-agent: googlebot Disallow: /_hidden` in your robots.txt file, would prohibit Googlebot from crawling any content within your site's `/_hidden` directory.

Your robots.txt file is valid as long as it has at least one user-agent rule, although you can add as many rules as you like. Each user-agent can have multiple disallows, and each robots.txt can include multiple user-agent rules. User-agent rules must be separated by a line break, but disallows can go directly below the previous.


```
User-agent: agent-1
Disallow: /sites/secrets
Disallow: /site/some-other-secrets

User-agent: agent-2
Disallow: /

User-agent agent-3
Disallow:

```


