---
layout: post
title:  "Game Story Design"
date:   2016-04-06
excerpt: "First composition idea of the story."
project: true
tag:
- Game Story
- Theme
- Justice
comments: true
---

![j](https://user-images.githubusercontent.com/39361933/59728268-54ea1780-9274-11e9-9fe9-259e7ecfc4aa.jpg)

<center><b>정의</b>란 무엇인가?</center>
     
 고등학생 때 이 책을 읽게 되고 난 후, 계속해서 공리주의, 자유주의 간의 균형에 대해 생각하게 되었고 이를 사람들에게 알려 사람들은 어떤 가치를 중요하게 여기는지, 그리고 그 가치를 중요하게 여기는 것이 옳은 것인지 사람들 스스로가 생각해 볼 수 있는 게임을 만들어 보고 싶었습니다.
 
<iframe src="https://ko.wikipedia.org/wiki/%EC%A0%95%EC%9D%98%EB%9E%80_%EB%AC%B4%EC%97%87%EC%9D%B8%EA%B0%80" frameborder="0" scrolling="0"></iframe>    
      
## Installation
* Fork the [Moon repo](https://github.com/TaylanTatli/Moon/fork)
* Edit `_config.yml` file.
* Remove sample posts from `_posts` folder and add yours.
* Edit `index.md` file in `about` folder.
* Change repo name to `YourUserName.github.io`    
     
That's all.

## Preview

{% capture images %}
	https://cloud.githubusercontent.com/assets/754514/14509716/61ac6c8e-01d6-11e6-879f-8308883de790.png
	https://cloud.githubusercontent.com/assets/754514/14509717/61ad05ae-01d6-11e6-85ae-5a817dd8763b.png
	https://cloud.githubusercontent.com/assets/754514/14509714/61a89708-01d6-11e6-8fcd-74b002a060df.png
{% endcapture %}
{% include gallery images=images caption="Screenshots of Moon Theme" cols=3 %}

---

{% capture images %}
	https://cloud.githubusercontent.com/assets/754514/14509718/61b09a20-01d6-11e6-8da1-4202ae4d83cd.png
	https://cloud.githubusercontent.com/assets/754514/14509715/61aa9d00-01d6-11e6-81a6-c6837edf2e84.png
{% endcapture %}
{% include gallery images=images caption="Moon Theme on Small Screen Size" cols=2 %}      
      
See a [live version of Moon](http://taylantatli.github.io/Moon) hosted on GitHub.      

## Site Setup
A quick checklist of the files you’ll want to edit to get up and running.    

### Site Wide Configuration
`_config.yml` is your friend. Open it up and personalize it. Most variables are self explanatory but here's an explanation of each if needed:

#### title

The title of your site... shocker!

Example `title: My Awesome Site`

#### bio

The description to show on your homepage.

#### description

The description to use for meta tags and navigation menu.

#### url

Used to generate absolute urls in `sitemap.xml`, `feed.xml`, and for generating canonical URLs in `<head>`. When developing locally either comment this out or use something like `http://localhost:4000` so all assets load properly. *Don't include a trailing `/`*.

Examples:

{% highlight yaml %}
url: http://taylantatli.me/Moon
url: http://localhost:4000
url: //cooldude.github.io
url:
{% endhighlight %}

#### reading_time

Set true to show reading time for posts. And set `words_per_minute`, default is 200.

#### logo
Your site's logo. It will show on homepage and navigation menu. Also used for twitter meta tags.

#### background
Image for background. If you don't set it, color will be used as a background.

#### Google Analytics and Webmaster Tools

Google Analytics UA and Webmaster Tool verification tags can be entered in `_config.yml`. For more information on obtaining these meta tags check [Google Webmaster Tools](http://support.google.com/webmasters/bin/answer.py?hl=en&answer=35179) and [Bing Webmaster Tools](https://ssl.bing.com/webmaster/configure/verify/ownership) support.

#### MathJax
It's enabled. But if you don't want to use it. Set it false in  `_config.yml`.

#### Disqus Comments
Set your disqus shortname in `_config.yml` to use comments.

---

### Navigation Links

To set what links appear in the top navigation edit `_data/navigation.yml`. Use the following format to set the URL and title for as many links as you'd like. *External links will open in a new window.*

{% highlight yaml %}
- title: Home
  url: /

- title: Blog
  url: /blog/

- title: Projects
  url: /projects/

- title: About
  url: /about/

- title: Moon
  url: http://taylantatli.me/Moon
{% endhighlight %}

---

## Layouts and Content

Moon Theme use [Jekyll Compress](https://github.com/penibelst/jekyll-compress-html) to compress html output. But it can cause errors if you use "linenos" (line numbers). I suggest don't use line numbers for codes, because it won't look good with this theme, also i didn't give a proper style for them. If you insist to use line numbers, just remove `layout: compress` string from layouts. It will disable compressing.

### Feature Image

You can set feature image per post. Just add `feature: some link` to your post's front matter.

```
feature: /assets/img/some-image.png
or
feaure: http://example.com/some-image.png
```    
 This also will be used for twitter card:

![Moon Twitter Card](https://cloud.githubusercontent.com/assets/754514/14509719/61c5751c-01d6-11e6-8c29-ce8ccad149bf.png)

### Comments
To show disqus comments for your post add `comments: true` to your post's front matter.

---

## Questions?

Found a bug or aren't quite sure how something works? By all means [file a GitHub Issue](https://github.com/TaylanTatli/Moon/issues/new). And if you make something cool with this theme feel free to let me know.

---

## License

This theme is free and open source software, distributed under the MIT License. So feel free to use this Jekyll theme on your site without linking back to me or including a disclaimer.