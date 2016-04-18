# Socialmeta plugin for Joomla!
Social-meta is a system plugin for Joomla! which creates [open graph](http://og.me) and [twitter](https://dev.twitter.com/cards/overview) meta tags in the head of the document. The idea is to allow the writer to configure properly the way his article will appear in the social streams.
## Installation
Download the project zip and install it like any other extension. Go to extensions > plugins and find System - Socialmeta, publish it.

> IMPORTANT  
> Open and save the configuration of the plugin at least once - even if you didn't provide any data - to set up automatically some default parameters values and be sure to avoid any PHP notices.

## Configuration
Go to extensions > plugins and find System - Socialmeta
### Basic
![screenshot of the basic options](https://dl.dropboxusercontent.com/u/11260729/socialmeta/socialmeta-plugin-basic-conf.jpg)
### Advanced
Don't be scared, there's nothing to do here except if you get some specific compatibility issues. In this case it allows to disable globally the creation of some specific meta. It may be the case for example if you have some kind of sharing button extension which already creates the fb:app_id meta.
![screenshot of the advanced options](https://dl.dropboxusercontent.com/u/11260729/socialmeta/socialmeta-plugin-advanced-conf.jpg)
## Usage
This is how it looks in the Joomla! article view.
![screenshot of the article view](https://dl.dropboxusercontent.com/u/11260729/socialmeta/socialmeta-article-form.jpg)
## Sites with multiple authors
If you wish each author to be linked with his publications on the facebook stream you can add his own Facebook profile URL and Twitter @username in the Contact component.
To perform this just create a contact for each user for which you would like to override the general settings.  
- Create a new contact  
- Give him a name and link it with a existing user (fig.1)  
- Go the social tab (fig.2)

![screenshot of the contact creation](https://dl.dropboxusercontent.com/u/11260729/socialmeta/socialmeta-contact-form-link.jpg)  

- Provide Facebook (fig.1) and Twitter (fig.2) credentials. Note Facebook must be an Url and Twitter a @username
- Save the new contact.

![screenshot of the contact creation social tab](https://dl.dropboxusercontent.com/u/11260729/socialmeta/socialmeta-contact-form-social.jpg)

> NOTE  
> You absolutely don't need to use the contact component. I just use its table to store the data. The contact doesn't need to be published. You can even disable the component if you wish ;)  
I made this choice to avoid having to create a user plugin which may conflict with other extensions which will also override the user management.  
It may change in the future but that's the most reliable solution I found up to now.

## Disclaimer
This plugin was created for a friend of mine runing a Joomla! website. It was supposed to serve a particular purpose, because IMHO there was a lack on that particular matter. As it could be useful for anyone using Joomla!, we now **try to improve** it and to make it really **generic**. So, be confident, send me suggestions, and we will build together **the** solution to fix that **ONE FOR ALL** ;)
## Limitation
Up to now Socialmeta is only compatible with Joomla articles (com_content) and FLEXIcontent items (com_flexicontent). It only implements 2 objects from the open graph protocol: article and video.
If you are looking for an open graph solution for implementing the product type to your ecommerce, you should have a further look to the [JED](http://extensions.joomla.org)
## Requirements
Joomla! 3+ (it should also be compatible with 2.5 soon)
## Useful ressources
**Official documents and recommendations**  
[The open graph protocol](http://ogp.me/)  
[Sharing Best Practices for Websites & Mobile Apps](https://developers.facebook.com/docs/sharing/best-practices)  
[The article object](https://developers.facebook.com/docs/reference/opengraph/object-type/article/)  
[Twitter cards official documentation](https://dev.twitter.com/cards/overview)  

**Testing tools**  
[Open Graph Object debugger](https://developers.facebook.com/tools/debug/og/object/)  
[Twitter Card Validator](https://cards-dev.twitter.com/validator)  

**General articles**  
[What You Need to Know About Open Graph Meta Tags for Total Facebook and Twitter Mastery](https://blog.kissmetrics.com/open-graph-meta-tags/)  
[How to implement opengraph for video](http://www.marketing-mojo.com/blog/how-to-implement-open-graph-tags-for-videos/)  
[Increase your Social Impact with OpenGraph – Related Articles](http://wersm.com/increase-your-social-impact-with-opengraph-related-articles/)  
[Some meta templates](https://moz.com/blog/meta-data-templates-123)  
[New Open Graph tags for media publishers](https://developers.facebook.com/blog/post/2013/06/19/platform-updates--new-open-graph-tags-for-media-publishers-and-more/)  
[7 Common Meta Tag Mistakes That Publishers Make](http://www.trueanthem.com/blog/7-common-meta-tag-mistakes-that-publishers-make/)  
[Social Metadata: More Important than You Think](http://www.trueanthem.com/blog/social-metadata-more-important-than-you-think/)  
[Using Author Tags with Facebook Story Previews](http://www.trueanthem.com/blog/using-author-tags-with-facebook-story-previews/)  
[Facebook is King, Other Networks Fight for Scraps](http://blog.naytev.com/facebook-is-king/)  


**Articles about video tags and strategy**  
[Video SEO - basics, essentials & best practises](https://www.speechpad.com/video-seo)  
[How Video Marketing Creates Immediate SEO Results](https://blog.shareaholic.com/video-marketing-seo-results/)  
[Setting Videos not Hosted on Brightcove to Play within Facebook](https://support.brightcove.com/en/video-cloud/docs/setting-videos-not-hosted-brightcove-play-within-facebook)  

**Less interesting but still some information to grab**  
[Social Meta Tags for Google, Twitter and Facebook](http://www.9lessons.info/2014/01/social-meta-tags-for-google-twitter-and.html)  
[Facebook Open Graph Meta Tags Tutorial](http://qnimate.com/open-graph-protocol-in-facebook/)  
[Social Media Tags: 11 Most Important Facebook Meta Tags](http://www.saleoid.com/blog/social-media-tags-11-most-important-facebook-meta-tags/)  
