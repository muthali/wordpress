---
ID: 1104
post_title: Expertrec custom search API
author: muthali ganesh
post_excerpt: ""
layout: post
permalink: >
  https://blog.expertrec.com/expertrec-custom-search-api/
published: true
post_date: 2018-04-07 04:24:45
---
<strong>Expertrec's custom search API-</strong>

This article explains how you can use expertrec's custom search api to get search results programatically.

Go to <a href="https://cse.expertrec.com?platform=cse" target="_blank" rel="noopener">https://cse.expertrec.com?platform=cse </a> and enter your website and sitemap URLs to get your crawl done. Go and click on your demo link.
<p style="text-align: center;">[inbound_button font_size="20" color="#c8232b" text_color="#ffffff" icon="" url="https://cse.expertrec.com/?platform=cse" width="" target="_blank"]Get your expertrec site search API[/inbound_button]</p>

<ol>
 	<li>In your demo link open developer tools (control+shift+I) on your chrome browser.</li>
 	<li>Go to network tab.</li>
 	<li>Go to XHR section.</li>
 	<li>Search for expertrec.</li>
 	<li>Click on searchv7...</li>
</ol>
<img src="https://blog.expertrec.com/wp-content/uploads/2018/03/expertrec-api.png" alt="google site search api" width="1346" height="773" class="wp-image-1059 size-full aligncenter" />

The API will be of this format-
<pre>https://searchv7.expertrec.com/v6/search/{org_id}/?q={keyword}&amp;page={pagination}&amp;size={number_of_search_results}</pre>
<pre>https://searchv7.expertrec.com/v6/search/79b96660-27e0-11e8-a8e3-12b6486824f4/?q=a&amp;page=0&amp;size=16</pre>
Expertrec site search API parameters-
<ol>
 	<li>org_id- Your unique ID that identifies your website/ websites.</li>
 	<li>q- Keyword.</li>
 	<li>page- pagination</li>
 	<li>size- number of search results to be displayed.</li>
</ol>
The results will be in JSON format and will be similar to this screen shot-

<img src="https://blog.expertrec.com/wp-content/uploads/2018/03/expertrec-api-results.png" alt="" width="1440" height="900" class="size-full wp-image-1061 aligncenter" />
<p style="text-align: center;">[inbound_button font_size="20" color="#c8232b" text_color="#ffffff" icon="" url="https://cse.expertrec.com/?platform=cse" width="" target="_blank"]Get your site search API[/inbound_button]</p>