---
ID: 1938
post_title: >
  How to add a google like search engine
  to your magento store
author: muthali ganesh
post_excerpt: ""
layout: post
permalink: >
  https://blog.expertrec.com/how-to-add-a-google-like-search-engine-to-your-magento-store/
published: true
post_date: 2018-07-12 12:25:20
---
Want to deliver a google like search engine on your magento store? You can accomplish this with expertrec custom search engine for 9 USD per month depending upon the number of URLs in your website.

You can add features such as autocomplete, spell correct, image search, filtered search in a matter of few minutes.

How to do this?
<ol>
 	<li><strong>Go to <a href="https://cse.expertrec.com?platform=true" target="_blank" rel="noopener">https://cse.expertrec.com?platform=true</a></strong><img src="https://blog.expertrec.com/wp-content/uploads/2018/07/1-1.png" alt="" width="546" height="214" class="wp-image-1951 aligncenter" /></li>
 	<li><strong>Enter your website URL</strong>.<img src="https://blog.expertrec.com/wp-content/uploads/2018/07/2-1.png" alt="" width="537" height="285" class="wp-image-1952 aligncenter" /></li>
 	<li><strong>Wait for crawl to complete.</strong><img src="https://blog.expertrec.com/wp-content/uploads/2018/07/4-1.png" alt="" width="618" height="251" class="wp-image-1954 aligncenter" /></li>
 	<li><strong>Copy the code</strong>.<img src="https://blog.expertrec.com/wp-content/uploads/2018/07/3-1.png" alt="" width="589" height="440" class="wp-image-1953 aligncenter" /></li>
 	<li><strong>Replace your magento search box with expertrec' search box</strong>- <span>The template for Magento search box can be found at <strong><em>app/design/frontend/base/default/template/catalogsearch/form.mini.phtml</em></strong>. We will customize this so it will call expertrec search results when a search query is entered. Replace the following code with the code you copied from <a href="https://cse.expertrec.com/?platform=cse" target="_blank" rel="noopener">expertrec’s control panel</a>.  </span><span>Replace</span>
<pre class="lang:php decode:true">&lt;form id="search_mini_form" action="&lt;?php echo $this-&gt;helper('catalogsearch')-&gt;getResultUrl() ?&gt;" method="get"&gt;
&lt;div class="form-search"&gt;
        &lt;label for="search"&gt;&lt;!--?php echo $this---&gt;__('Search:') ?&gt;&lt;/label&gt;
&lt;input id="search" class="input-text" name="&lt;?php echo $this-&gt;helper('catalogsearch')-&gt;getQueryParamName() ?&gt;" type="text" value="&lt;?php echo $this-&gt;helper('catalogsearch')-&gt;getEscapedQueryText() ?&gt;"&gt;
        &lt;button class="button" title="&lt;?php echo $this-&gt;__('Search') ?&gt;"&gt;&lt;span&gt;&lt;span&gt;&lt;!--?php echo $this---&gt;__('Search') ?&gt;&lt;/span&gt;&lt;/span&gt;&lt;/button&gt;
 
        &lt;script type="text/javascript"&gt;&lt;/script&gt;&lt;/div&gt;
&lt;/form&gt;</pre>
with the code you copied from your expertrec control panel.</li>
 	<li>That's it , you have added a google like search engine to your magento store. Here are some screenshots-<img src="https://blog.expertrec.com/wp-content/uploads/2018/07/5-2.png" alt="" width="592" height="531" class="size-full wp-image-1957 aligncenter" /> <img src="https://blog.expertrec.com/wp-content/uploads/2018/07/6-1.png" alt="" width="646" height="454" class="wp-image-1958 aligncenter" /></li>
</ol>