## Page Speed
Page speed for the purpose of SEO is the length of time it takes to display all content on a page. 
This includes all elements of a page, including code, images and videos. Server and network performance also contribute to page speed. Beginning in 2017, Google stated that page speed would have an even greater
effect on SEO for ranking factors in their search index. Google considers page speed as a practical indicator of user experience. 

### Here are some common causes that contribute to slow page speeds:
* Images and videos
* Web Application Firewalls
* Plugins and third-party apps/integrations
* Scripts
* Large files
* Hosting issues include network and DNS 

### Example site:
https://example.com

Our example site example.com is a WordPress install where blog posts are made on a daily basis. Each blog post includes multiple images, and some contain videos.
After one year has passed since launch, the site is tested on pingdom.com, and the home page takes over 5 seconds to load. Since the primary content is mainly blog posts
with images and videos, the first improvement should be to compress images. There are web applications where this can be done, but since this is a WordPress site, we can
use one of the many available image compression plugins. An image compression plugin is installed and configured to compress all of the images on the site.  

After images are compressed, we can improve performance even more by adding a Content Delivery Network (CDN) to our site. A CDN is a network of proxy servers spanning different
geographical locations that present specific site content. This allows images and videos to be cached and readily available for users to access from each of the geographical 
CDN server locations that are available. This improves speed for the end user and also improves system performance by reducing bandwidth.

After implementing these changes to our site, we find that Pingdom now shows it takes less than 2 seconds to load the home page.    

### Content Delivery Network
![Content Delivery Network](https://i.lensdump.com/i/061Oxz.jpg)   


### Why is it good for SEO?
Page speed is extremely important for SEO, and fast page speeds provide a great user experience. Google has prioritized page speed in the past and, in 2020, announced that the upcoming
[Page Experience](https://developers.google.com/search/docs/guides/page-experience) will be implemented at some point in 2021. Page Experience will measure performance by a set of signals outlined
by Google. Page speed is included under the Core Web Vitals as an essential component for SEO. Specifically, Google has defined a target metric Largest Contentful Paint (LCP), to be at <2.5 seconds. 
LCP is a user-centric metric that focuses on the perceived load time of the content.

### Testing sites:
* https://tools.pingdom.com
* https://www.thinkwithgoogle.com/feature/testmysite/

### Resources
* https://moz.com/blog/page-speed-optimization
* https://developers.google.com/web/tools/lighthouse
* https://developers.google.com/search/docs/guides/page-experience 




