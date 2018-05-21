---
ID: 1051
post_title: Google site search API simplified
author: muthali ganesh
post_excerpt: ""
layout: post
permalink: >
  https://blog.expertrec.com/google-site-search-api/
published: true
post_date: 2018-03-22 15:19:52
---
Google site search API (now custom search API since Google site search is shutting down) lets you develop applications to get and show results from Google custom/ site search programatically. Google site search In this article we will discuss on the components of the google site search api and where to find them.
<p style="text-align: center;">[inbound_button font_size="20" color="#c8232b" text_color="#ffffff" icon="" url="https://cse.expertrec.com/?platform=cse" width="" target="_blank"]Get your site search API[/inbound_button]</p>
The usual API call is
<pre>https://www.googleapis.com/customsearch/v1?parameters</pre>
Here parameters could be -
<ol>
 	<li><strong>q</strong>- query string</li>
 	<li><strong>cx</strong>- Custom search engine ID.</li>
 	<li><strong>fileType</strong>- bmp, gif, jpg, png, pdf etc</li>
 	<li><strong>num</strong>-number of search results to display</li>
 	<li><strong>searchType- </strong>search type.</li>
 	<li><strong>sort</strong>-Sort by functionality to use.</li>
</ol>
For a list of all query parameters, go to this <a href="https://developers.google.com/apis-explorer/?hl=en_US#p/customsearch/v1/search.cse.list" target="_blank" rel="noopener">link</a>.

<img src="https://blog.expertrec.com/wp-content/uploads/2018/03/parameters.png" alt="google site search API" width="712" height="601" class="aligncenter wp-image-1054 size-full" />

A sample api call would be like this-
<pre>https://www.googleapis.com/customsearch/v1?key={YOUR_API_KEY}&amp;cx={CUSTOM_SEARCH_ENGINE_ID}&amp;q={KEYWORD}</pre>
<pre>https://www.googleapis.com/customsearch/v1?key=<span>AIzaSyCVAXiUzRYsML1Pv</span>cx=<span>012278024424817052234:cimrvj4h4uk</span><span>&amp;q=jeff</span></pre>
Response of this API will be in JSON format for you to consume to build your search application.

<img src="https://blog.expertrec.com/wp-content/uploads/2018/03/sitesearchapiresults.png" alt="google site search api" width="938" height="730" class="aligncenter wp-image-1062 size-full" />

<strong>Getting your API Key</strong>
<ol>
 	<li>Go to <a href="https://developers.google.com/custom-search/json-api/v1/overview">https://developers.google.com/custom-search/json-api/v1/overview</a></li>
 	<li>Click on get key.<img src="https://blog.expertrec.com/wp-content/uploads/2018/03/Google-site-search-api-get-key.png" alt="google site search api" width="856" height="294" class="alignnone wp-image-1075 size-full" /></li>
 	<li>Click create new project.<img src="https://blog.expertrec.com/wp-content/uploads/2018/03/custom-search-api.png" alt="google site search api" width="845" height="506" class="alignnone wp-image-1077 size-full" /></li>
 	<li>This will generate your new API key.<img src="https://blog.expertrec.com/wp-content/uploads/2018/03/api-key.png" alt="google site search api" width="667" height="392" class="alignnone wp-image-1079 size-full" /></li>
 	<li>You can restrict the usage of this API key in your google api console <a href="https://console.developers.google.com/apis">https://console.developers.google.com/apis</a></li>
</ol>
<img src="https://blog.expertrec.com/wp-content/uploads/2018/03/google-api-console.png" alt="google site search api" width="781" height="769" class="alignnone wp-image-1080 size-full" />

<strong>Getting your CX / Search engine ID:</strong>

Go to your custom search / site search control panel-&gt; edit search engine-&gt;Basics-&gt;Details-&gt;Search engine ID.

This is your search engine ID.

<img src="https://blog.expertrec.com/wp-content/uploads/2018/03/search-engine-ID.png" alt="google site search api" width="854" height="491" class="aligncenter wp-image-1057 size-full" />

If you are finding issues with the Google site search API, you could try out expertrec's site search API, which is easier to implement.

<strong>Expertrec's Google site search replacement API-</strong>

Go to <a href="https://cse.expertrec.com?platform=cse" target="_blank" rel="noopener">https://cse.expertrec.com?platform=cse </a> and enter your website and sitemap URLs to get your crawl done. Go and click on your demo link.
<p style="text-align: center;">[inbound_button font_size="20" color="#c8232b" text_color="#ffffff" icon="" url="https://cse.expertrec.com/?platform=cse" width="" target="_blank"]Get your expertrec site search API[/inbound_button]</p>

<ol>
 	<li>In your demo link open developer tools (control+shift+I) on your chrome browser.</li>
 	<li>Go to network tab.</li>
 	<li>Go to XHR section.</li>
 	<li>Search for expertrec.</li>
 	<li>Click on searchv7...</li>
</ol>
<img src="https://blog.expertrec.com/wp-content/uploads/2018/03/expertrec-api.png" alt="google site search api" width="1346" height="773" class="aligncenter wp-image-1059 size-full" />

The API will be of this format-
<pre>https://searchv7.expertrec.com/v6/search/{org_id}/?q={keyword}&amp;page={pagination}&amp;size={number_of_search_results}</pre>
<pre>https://searchv7.expertrec.com/v6/search/79b96660-27e0-11e8-a8e3-12b6486824f4/?q=a&amp;page=0&amp;size=16</pre>
&nbsp;

Expertrec site search API parameters-
<ol>
 	<li>org_id- Your unique ID that identifies your website/ websites.</li>
 	<li>q- Keyword.</li>
 	<li>page- pagination</li>
 	<li>size- number of search results to be displayed.</li>
</ol>
The results will be in JSON format and will be similar to this screen shot-

<img src="https://blog.expertrec.com/wp-content/uploads/2018/03/expertrec-api-results.png" alt="" width="1440" height="900" class="size-full wp-image-1061 aligncenter" />

&nbsp;
<p style="text-align: center;">[inbound_button font_size="20" color="#c8232b" text_color="#ffffff" icon="" url="https://cse.expertrec.com/?platform=cse" width="" target="_blank"]Get your site search API[/inbound_button]</p>