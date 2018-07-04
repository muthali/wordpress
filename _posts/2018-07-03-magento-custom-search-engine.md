---
ID: 1813
post_title: >
  How to create a magento custom search
  engine
author: muthali ganesh
post_excerpt: ""
layout: post
permalink: >
  https://blog.expertrec.com/magento-custom-search-engine/
published: true
post_date: 2018-07-03 17:49:25
---
The default magento search engine is not that great. A custom search engine can help you surface the right products to your customers on your magento store. It also helps in reducing the time for product discovery.

In this article we will see how to create a magento custom search engine for a magento store (cosjj.com) using expertrec, google custom search and duckduckgo custom search.
<h3><strong>Option 1 - Using <a href="https://cse.expertrec.com?platform=cse" target="_blank" rel="noopener">expertrec</a> to build a magento custom search - Paid ( 9 USD per month+) No ads</strong></h3>
Here are steps-
<ol>
 	<li><strong>Go to  <a href="https://cse.expertrec.com?platform=cse" target="_blank" rel="noopener">https://cse.expertrec.com?platform=cse</a> </strong></li>
 	<li><strong>Sign in with your gmail id.</strong><img src="https://blog.expertrec.com/wp-content/uploads/2018/07/mixmax1-1.png" alt="magento custom search" width="566" height="222" class="wp-image-1815 aligncenter" /></li>
 	<li><strong>Enter the website url of your magento site</strong> <strong>and choose your nearest server location</strong>.<img src="https://blog.expertrec.com/wp-content/uploads/2018/07/mixmax2-1.png" alt="magento custom search" width="565" height="301" class="aligncenter wp-image-1816" /></li>
 	<li><strong>By now crawl should have started for your site</strong>. Get the code and add it to your magento site. Get your developer help if needed. <img src="https://blog.expertrec.com/wp-content/uploads/2018/07/magento-custom-search-code.png" alt="magento custom search " width="520" height="389" class="aligncenter wp-image-1823" /></li>
 	<li><strong>Replace your magento search box form with expertrec search boc</strong>-<span>The template for Magento search box can be found at app/design/frontend/base/default/template/catalogsearch/form.mini.phtml. We will customize this so it will call expertrec search results when a search query is entered. Replace the following code with the code you copied from <a href="https://cse.expertrec.com?platform=cse" target="_blank" rel="noopener">expertrec's control panel</a>. </span>
<ol>
 	<li>
<div class="line number1 index0 alt2"><code class="php plain">&lt;form id=</code><code class="php string">"search_mini_form"</code> <code class="php plain">action=</code><code class="php string">"&lt;?php echo $this-&gt;helper('catalogsearch')-&gt;getResultUrl() ?&gt;"</code> <code class="php plain">method=</code><code class="php string">"get"</code><code class="php plain">&gt;</code></div>
<div class="line number2 index1 alt1"><code class="php plain">&lt;div<span> </span></code><code class="php keyword">class</code><code class="php plain">=</code><code class="php string">"form-search"</code><code class="php plain">&gt;</code></div>
<div class="line number3 index2 alt2"><code class="php spaces">        </code><code class="php plain">&lt;label<span> </span></code><code class="php keyword">for</code><code class="php plain">=</code><code class="php string">"search"</code><code class="php plain">&gt;&lt;!--?php<span> </span></code><code class="php functions">echo</code> <code class="php variable">$this</code><code class="php plain">---&gt;__(</code><code class="php string">'Search:'</code><code class="php plain">) ?&gt;&lt;/label&gt;</code></div>
<div class="line number4 index3 alt1"><code class="php plain">&lt;input id=</code><code class="php string">"search"</code> <code class="php keyword">class</code><code class="php plain">=</code><code class="php string">"input-text"</code> <code class="php plain">name=</code><code class="php string">"&lt;?php echo $this-&gt;helper('catalogsearch')-&gt;getQueryParamName() ?&gt;"</code> <code class="php plain">type=</code><code class="php string">"text"</code> <code class="php plain">value=</code><code class="php string">"&lt;?php echo $this-&gt;helper('catalogsearch')-&gt;getEscapedQueryText() ?&gt;"</code><code class="php plain">&gt;</code></div>
<div class="line number5 index4 alt2"><code class="php spaces">        </code><code class="php plain">&lt;button<span> </span></code><code class="php keyword">class</code><code class="php plain">=</code><code class="php string">"button"</code> <code class="php plain">title=</code><code class="php string">"&lt;?php echo $this-&gt;__('Search') ?&gt;"</code><code class="php plain">&gt;&lt;span&gt;&lt;span&gt;&lt;!--?php<span> </span></code><code class="php functions">echo</code> <code class="php variable">$this</code><code class="php plain">---&gt;__(</code><code class="php string">'Search'</code><code class="php plain">) ?&gt;&lt;/span&gt;&lt;/span&gt;&lt;/button&gt;</code></div>
<div class="line number6 index5 alt1"></div>
<div class="line number7 index6 alt2"><code class="php spaces">        </code><code class="php plain">&lt;script type=</code><code class="php string">"text/javascript"</code><code class="php plain">&gt;&lt;/script&gt;&lt;/div&gt;</code></div>
<div class="line number8 index7 alt1"><code class="php plain">&lt;/form&gt;</code></div></li>
</ol>
</li>
 	<li><strong>That's it, you have added custom search to your magento site</strong>. You can monitor crawl status and edit look and feel of the search UI in your control panel.<img src="https://blog.expertrec.com/wp-content/uploads/2018/07/mixmax-dashboard.png" alt="￼magento custom search" width="594" height="241" class="aligncenter wp-image-1819" /></li>
</ol>
Here is a screenshot of the search autocomplete UI.<img src="https://blog.expertrec.com/wp-content/uploads/2018/07/avengers-1.png" alt="magento custom search" width="592" height="531" class="aligncenter wp-image-1818 size-full" />

And the search results page-<img src="https://blog.expertrec.com/wp-content/uploads/2018/07/avengers-listing.png" alt="magento custom search" width="601" height="423" class="aligncenter wp-image-1820" />

Create your own magento custom search engine at <a href="https://cse.expertrec.com?platform=cse" target="_blank" rel="noopener">https://cse.expertrec.com?platform=cse</a>