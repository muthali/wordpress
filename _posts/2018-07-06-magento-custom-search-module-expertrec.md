---
ID: 1902
post_title: 'Magento custom search module &#8211; expertrec'
author: muthali ganesh
post_excerpt: ""
layout: post
permalink: >
  https://blog.expertrec.com/magento-custom-search-module-expertrec/
published: true
post_date: 2018-07-06 12:50:11
---
<a href="https://cse.expertrec.com?platform=cse">Expertrec's magento custom search module</a> adds search autocomplete, spell correct features to your magento store. Here are some screen shots of the search features built using expertrec magento custom search module. Price begins at 9 USD per month (paid annually).

<strong>Autocomplete</strong>- Search autocomplete or typeahead to make sure your customers find the right products within the shortest time<img src="https://blog.expertrec.com/wp-content/uploads/2018/07/magento-custom-search-module.jpg" alt="magento custom search module" width="501" height="496" class="aligncenter wp-image-1904 size-full" />

<strong>Spell correct- </strong>Spell correct features for your magento store so that you don't lose sales on your magento site . Here you can see that the magento custom search module corrects spelling errors to show the right. Search for "alddin" shows the right Aladdin products to the user.<img src="https://blog.expertrec.com/wp-content/uploads/2018/07/spell-correct.jpg" alt="magento custom search module" width="505" height="462" class="aligncenter wp-image-1905 size-full" />

<strong>Search results page-  </strong>Deliver a google like search results page experience on your magento store.<strong><img src="https://blog.expertrec.com/wp-content/uploads/2018/07/search-results-page.jpg" alt="magento custom search module" width="599" height="452" class="aligncenter wp-image-1906" /></strong>

Steps to create a custom search engine using expertrec magento custom search module.
<ol>
 	<li>Go to <a href="https://cse.expertrec.com" target="_blank" rel="noopener">https://cse.expertrec.com</a><img src="https://blog.expertrec.com/wp-content/uploads/2018/07/cse.png" alt="magento custom search module" width="768" height="301" class="aligncenter wp-image-1907 size-full" /></li>
 	<li>Enter your website URL.<img src="https://blog.expertrec.com/wp-content/uploads/2018/07/url.png" alt="magento custom search module" width="768" height="408" class="alignnone wp-image-1908 size-full" /></li>
 	<li>Copy the code from your expertrec control panel. <img src="https://blog.expertrec.com/wp-content/uploads/2018/07/code.png" alt="magento custom search module" width="729" height="545" class="alignnone wp-image-1909 size-full" /></li>
 	<li>Wait for crawl to complete<img src="https://blog.expertrec.com/wp-content/uploads/2018/07/crawl.png" alt="magento custom search module" width="630" height="256" class="aligncenter wp-image-1910" /></li>
 	<li>Replace your magento search box with expertrec's search box- For this step you might need the help of your deveoper. <span><span><span><span><span><span><span><span>The template for Magento search box can be found at <em>app/design/frontend/base/default/template/catalogsearch/form.mini.phtml</em>. We will change this so it will call expertrec's custom  search code. Change this from:</span></span></span></span></span></span></span></span>
<pre class="lang:php decode:true ">&lt;form id="search_mini_form" action="" method="get"&gt;
 &lt;div class="form-search"&gt;
 &lt;label for="search"&gt; __('Search:') ?&gt; &lt;/label&gt;
 &lt;input id="search" class="input-text" name="" type="text" value=""&gt;
 &lt;button class="button" title=""&gt; 
&lt;span&gt; 
&lt;span&gt; __('Search') ?&gt; &lt;/span&gt;
 &lt;/span&gt;
 &lt;/button&gt; 
&lt;script type="text/javascript"&gt;
&lt;/script&gt;
&lt;/div&gt;
&lt;/form&gt;</pre>
to the code you copied from your expertrec control panel.</li>
 	<li>That's it, you have added expertrec's custom search module to your magento store.<img src="https://blog.expertrec.com/wp-content/uploads/2018/07/search-demo.gif" alt="magento custom search module" width="600" height="289" class="alignnone size-full wp-image-1911" /></li>
</ol>
&nbsp;