---
layout: post
title:  "用Jekyll构建blog"
date:   2013-12-15 14:50:52
---

分享任意网页至微信的二维码由<a href="http://jiathis.com" target="_blank">jiathis</a>生成，感谢。另外暂时不支持https的链接。

* 将以下内容复制到粘贴板。
{% highlight javascript %}
javascript:(function(){try{if (typeof jiathis_sendto == 'undefined'){var jiathis=document.createElement("script");jiathis.type='text/javascript';jiathis.src="http://v3.jiathis.com/code/jia.js";jiathis.charset='utf-8';jiathis.onload=function(){jiathis_sendto('weixin')};document.getElementsByTagName("body")[0].appendChild(jiathis);}else{jiathis_sendto('weixin')}}catch(e){alert(e);}})();
{% endhighlight %}

* 在浏览器的bookmark栏上右击。

![]({{site.url}}/assets/images/20131214/2.jpg)

* 选择Add Page。

![]({{site.url}}/assets/images/20131214/3.jpg)

* 弹出框中名字随意，URL框中将刚才粘贴板中的内容复制过来，保存即可。

![]({{site.url}}/assets/images/20131214/4.jpg)

* 在分享页面上点击该按钮。接下来你懂的。

![]({{site.url}}/assets/images/20131214/5.jpg)
