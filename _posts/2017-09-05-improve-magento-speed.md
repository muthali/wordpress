---
ID: 93
post_title: How to improve magento speed
author: muthali ganesh
post_excerpt: ""
layout: post
permalink: >
  https://blog.expertrec.com/improve-magento-speed/
published: true
post_date: 2017-09-05 17:54:21
---
To <strong>speed up magento</strong>, follow the below steps. Some of the below mentioned steps would require some technical expertise.
<ul>
 	<li><strong>As a first step, check your site speed stats using <a href="https://developers.google.com/speed/pagespeed/insights/" target="_blank" rel="noopener">Google page insights</a>/ <a href="https://tools.pingdom.com" target="_blank" rel="noopener">Pingdom tools</a>/ <a href="https://gtmetrix.com" target="_blank" rel="noopener">GT Metrix</a>:</strong> This will give some insights into what is making your site slow and will also help you in assessing whether you site speed has improved once you have made your optimizations.<img class="aligncenter wp-image-203" src="https://blog.expertrec.com/wp-content/uploads/2017/09/speed.jpg" alt="speed up magento" width="645" height="343" /></li>
 	<li><strong>Use a CDN: </strong>A CDN is a set of webservers at multiple locationsreduces the distance between your website visitors and your website server by storing a cached version of its content in various locations.<img class="aligncenter wp-image-96" src="https://blog.expertrec.com/wp-content/uploads/2017/09/speed-up-magento-CDN-300x162.png" alt="speed up magento" width="328" height="177" /><span style="color: #555555; font-size: 17px;">You could also integrate you magento store with amazon CDN (</span><a style="font-size: 17px;" href="http://aws.amazon.com/cloudfront/" target="_blank" rel="noopener">http://aws.amazon.com/cloudfront/</a><span style="color: #555555; font-size: 17px;">)<img class="aligncenter wp-image-204" src="https://blog.expertrec.com/wp-content/uploads/2017/09/amazon-cloudfront-settings-1_0.png" alt="speed up magento" width="639" height="196" /></span></li>
 	<li><strong>Server and Hosting: </strong>The right type of hosting is determined by your site traffic, number of products, attributes, peak traffic and whether you need a staging/ testing site. This data can be used to find calculate your CPU and RAM requirements. To calculate your requirements, this article might be helpful <a style="font-size: 17px;" href="https://magento.stackexchange.com/questions/43907/how-to-determine-hosting-requirements" target="_blank" rel="noopener">How to determine magento hosting requirements</a>. In case if your site traffic is low (around 100000) and  around 10k-50k products- CPU- 4 cores RAM- 2GB/4GB. For high traffic (around 1 million)- CPU- 8 cores, RAM-16GB</li>
</ul>
<ul>
 	<li><strong>Enable Gzip Compression: </strong>Gzip is the most used and effective compression technique. It reduces response times significantly. <a style="font-size: 17px;" href="https://magento.stackexchange.com/questions/82424/how-to-enable-gzip-compression" target="_blank" rel="noopener">How to enable magento gzip compression</a> <img class="aligncenter wp-image-205 size-full" src="https://blog.expertrec.com/wp-content/uploads/2017/09/gzip.png" alt="speed up magento" width="436" height="213" /></li>
</ul>
<ul>
 	<li><strong>Minify HTML, CSS and Javascript</strong>:
<ul>
 	<li>Minify HTML-to generate an optimized version of your HTML code.( <a href="http://minifycode.com/javascript-minifier/" target="_blank" rel="noopener">http://minifycode.com/javascript-minifier/</a>)</li>
 	<li>Minify CSS,: (<a href="http://minifycode.com/css-minifier/" target="_blank" rel="noopener">http://minifycode.com/css-minifier/</a>)</li>
 	<li>Minify JavaScript- (<a href="http://minifycode.com/html-minifier/" target="_blank" rel="noopener">http://minifycode.com/html-minifier/</a>)</li>
</ul>
</li>
 	<li><strong>Enable Flat Catalog: </strong>Categories and Products<strong> </strong>Attributes are stored in <em>separate</em> database tables . Enabling flat catalog in magento will put them in one table hence making it quicker for magento to retrieve for a search query.<img class="aligncenter wp-image-102" src="https://blog.expertrec.com/wp-content/uploads/2017/08/enable-flat-catalog-1024x412.png" alt="speed up magento" width="690" height="278" /><span style="color: #555555; font-size: 17px;">Go to </span><em style="color: #555555; font-size: 17px;">Magento Admin Panel&gt;&gt;System &gt;&gt; Configuration &gt;&gt; Catalog &gt;&gt;Frontend &gt;&gt; Use Flat Catalog Category &gt;&gt;Use Flat Catalog Product&gt;&gt;Select "Yes"&gt;&gt; Reindex.</em></li>
</ul>
<ul>
 	<li><strong>Install Varnish and Nginx Caching: </strong>Varnish cache- <em style="color: #555555; font-size: 17px;">Varnish Cache</em><span style="color: #555555; font-size: 17px;"> is a web application accelerator.It typically speeds up delivery and reduces page loading speed for websites with heavy static and dynamic content. </span>Nginx is a web-server that boosts performance results, and is much more stable when handling lots of requests, which results in high CPU usage.<img class="alignnone size-full wp-image-218" src="https://blog.expertrec.com/wp-content/uploads/2017/09/varnish-cache.png" alt="speed up magento" width="835" height="695" /></li>
</ul>
<ul>
 	<li><strong>Improve Magento Caching: </strong>Go to magento admin panel-&gt;System-&gt;Cache Management-&gt; Enable Cache<img class="aligncenter wp-image-206 size-full" src="https://blog.expertrec.com/wp-content/uploads/2017/09/cache.png" alt="speed up magento" width="577" height="346" /></li>
 	<li><strong>Merge Javacript and CSS files: </strong>Merging JS and CSS files helps reduce the number of HTTP requests raised each time the user visits the website. <a style="font-size: 17px;" href="https://blog.expertrec.com/merge-javascript-files-magento/" target="_blank" rel="noopener">https://blog.expertrec.com/merge-javascript-files-magento/</a></li>
</ul>
<ul>
 	<li><strong>Optimize images: </strong>You could use image compression tools such as <a href="https://tinypng.com/" target="_blank" rel="noopener">https://tinypng.com/</a> or  <a href="http://optimizilla.com/" target="_blank" rel="noopener">http://optimizilla.com/</a> which allows bulk upload and download of images</li>
 	<li><strong>Delete/Disable unused extensions: </strong> Go to magento admin panel-&gt; System-&gt; magento connect and uninstall unused extensions.<img class="aligncenter wp-image-207" src="https://blog.expertrec.com/wp-content/uploads/2017/09/magento-search-not-returning-results.png" alt="speed up magento" width="558" height="509" /></li>
</ul>
<ul>
 	<li><strong>Disable Magento logging: </strong>Go to <em>System -&gt; Configuration -&gt; Advanced -&gt; Developer -&gt; Log Settings-&gt; Set Enabled to "No"</em></li>
 	<li><strong>Make Javascript files Asynchronous:</strong> If you are adding any external javascripts to your magento site, make sure they are in asynchronous mode. To make JS asynchronus, this is the format <strong>&lt;script async src="yourjs.js"&gt;&lt;/script&gt;<em><img class="aligncenter wp-image-209" src="https://blog.expertrec.com/wp-content/uploads/2017/09/Disbale-logging.png" alt="speed up magento" width="689" height="379" /></em></strong></li>
 	<li><strong>Use magento speed optimization extensions</strong> - You could try a few extensions on <a href="https://www.magentocommerce.com/magento-connect/utilities/optimization.html" target="_blank" rel="noopener">magento connect </a>.<img class="wp-image-216 aligncenter" src="https://blog.expertrec.com/wp-content/uploads/2017/09/speed-extensions.jpg" alt="speed up magento" width="609" height="375" /></li>
</ul>
speed up magento

<strong>Summary: (How to speed up magento)</strong>
<ol>
 	<li><em>Check current site loading speed.</em></li>
 	<li><em>Use CDN</em></li>
 	<li><em>Choose good server and hosting.</em></li>
 	<li><em>Enable Gzip compression</em></li>
 	<li><em>Minify HTML,Javascript and CSS</em></li>
 	<li><em>Enable Flat catalog.</em></li>
 	<li><em>Install Varnish and Nginx cache.</em></li>
 	<li><em>Enable Magento caching.</em></li>
 	<li><em>Merge JS and CSS files</em></li>
 	<li><em>Optimize images.</em></li>
 	<li><em>Disbale unused extensions.</em></li>
 	<li><em>Disbale magento logging.</em></li>
 	<li><em>Make Javascript files Asynchronous</em></li>
 	<li><em>Use magento speed optimization extensions</em></li>
</ol>
Do let us know your thought/ comments in the comments section. Visit <a href="http://expertrec.com">expertrec.com</a> to know more about how you can boost your magento site search.
<p style="text-align: center;">[inbound_button font_size="20" color="#c8232b" text_color="#ffffff" icon="" url="https://magento.expertrec.com/signup" width="" target="_blank"]Install expertrec search extension[/inbound_button]</p>
&nbsp;