---
layout: post
title:  "分享任意网页至微信"
date:   2013-12-14 19:50:52
tags: [JavaScript, 微信]
---

有时候我们想把网页分享给微信的朋友，如果网站（例如优酷等）的网页上有“分享到微信”的链接，那就很好办，但仍然有不少网站，特别是国外的网站并没有这样的链接，怎么办？可以用下面的简单方法。

分享任意网页至微信的二维码由<a href="http://jiathis.com" target="_blank">jiathis</a>生成，感谢。另外暂时不支持https的链接。

* 将以下内容复制到粘贴板。
{% highlight javascript %}
javascript:(function(){try{if (typeof jiathis_sendto == 'undefined'){var jiathis=document.createElement("script");jiathis.type='text/javascript';jiathis.src="http://v3.jiathis.com/code/jia.js";jiathis.charset='utf-8';jiathis.onload=function(){jiathis_sendto('weixin')};document.getElementsByTagName("body")[0].appendChild(jiathis);}else{jiathis_sendto('weixin')}}catch(e){alert(e);}})();
{% endhighlight %}

* 在浏览器的bookmark栏上右击。

![]({{site.baseurl}}/images/20131214/2.jpg)

* 选择Add Page。

![]({{site.baseurl}}/images/20131214/3.jpg)

* 弹出框中名字随意，URL框中将刚才粘贴板中的内容复制过来，保存即可。

![]({{site.baseurl}}/images/20131214/4.jpg)

* 在分享页面上点击该按钮。接下来你懂的。

![]({{site.baseurl}}/images/20131214/5.jpg)
