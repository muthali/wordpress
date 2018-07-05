---
ID: 1837
post_title: >
  How to add Google custom search to
  magento
author: muthali ganesh
post_excerpt: ""
layout: post
permalink: >
  https://blog.expertrec.com/how-to-add-google-custom-search-to-magento/
published: true
post_date: 2018-07-05 10:30:46
---
The default magento search is not upto your expectations? You are not alone. Fortunately, You can use Google custom search for free to add a good search functionality to your magento store.

The only issue is that Google custom search has ads . If you are looking for an ad free magento search experience, you could opt for <a href="https://cse.expertrec.com?platform=cse">expertrec custom search engine</a> (plans begin at 9 USD per month).

Here are steps to create a magento google custom search engine -
<ol>
 	<li style="list-style-type: none;">
<ol>
 	<li><strong>Go to <a href="https://cse.google.com/cse/create/new" target="_blank" rel="noopener">https://cse.google.com/cse/create/new</a></strong><img src="https://blog.expertrec.com/wp-content/uploads/2018/07/gcse1.png" alt="magento google custom search" width="627" height="293" class="aligncenter wp-image-1838" /></li>
 	<li><strong>Enter your magento website URL and click on create- </strong><img src="https://blog.expertrec.com/wp-content/uploads/2018/07/gcse2.png" alt="magento google custom search" width="635" height="523" class="aligncenter wp-image-1839" /></li>
 	<li><strong>Click on "get code"</strong> .<img src="https://blog.expertrec.com/wp-content/uploads/2018/07/gcse3.png" alt="magento google custom search" width="662" height="380" class="aligncenter wp-image-1840" /></li>
 	<li><strong>Copy the code-</strong><img src="https://blog.expertrec.com/wp-content/uploads/2018/07/gcse4.png" alt="magento google custom search" width="568" height="428" class="aligncenter wp-image-1841 size-full" /></li>
 	<li><strong>Replace the magento search box code with Google custom search box code. </strong> For this step you might need the help of your deveoper. <span><span><span><span><span><span>The template for Magento search box can be found at <em>app/design/frontend/base/default/template/catalogsearch/form.mini.phtml</em>. We will change this so it will call the google search code. Change this from:</span></span></span></span></span></span>

[php]&lt;/pre&gt;
&lt;div class=&quot;line number1 index0 alt2&quot;&gt;&lt;code class=&quot;php plain&quot;&gt;&lt;form id=&lt;/code&gt;&lt;code class=&quot;php string&quot;&gt;&quot;search_mini_form&quot;&lt;/code&gt; &lt;code class=&quot;php plain&quot;&gt;action=&lt;/code&gt;&lt;code class=&quot;php string&quot;&gt;&quot;&lt;?php echo $this-&gt;helper('catalogsearch')-&gt;getResultUrl() ?&gt;&quot;&lt;/code&gt; &lt;code class=&quot;php plain&quot;&gt;method=&lt;/code&gt;&lt;code class=&quot;php string&quot;&gt;&quot;get&quot;&lt;/code&gt;&lt;code class=&quot;php plain&quot;&gt;&gt;&lt;/code&gt;&lt;/div&gt;
&lt;div class=&quot;line number2 index1 alt1&quot;&gt;&lt;code class=&quot;php plain&quot;&gt;&lt;div&lt;span&gt; &lt;/span&gt;&lt;/code&gt;&lt;code class=&quot;php keyword&quot;&gt;class&lt;/code&gt;&lt;code class=&quot;php plain&quot;&gt;=&lt;/code&gt;&lt;code class=&quot;php string&quot;&gt;&quot;form-search&quot;&lt;/code&gt;&lt;code class=&quot;php plain&quot;&gt;&gt;&lt;/code&gt;&lt;/div&gt;
&lt;div class=&quot;line number3 index2 alt2&quot;&gt;&lt;code class=&quot;php spaces&quot;&gt;        &lt;/code&gt;&lt;code class=&quot;php plain&quot;&gt;&lt;label&lt;span&gt; &lt;/span&gt;&lt;/code&gt;&lt;code class=&quot;php keyword&quot;&gt;for&lt;/code&gt;&lt;code class=&quot;php plain&quot;&gt;=&lt;/code&gt;&lt;code class=&quot;php string&quot;&gt;&quot;search&quot;&lt;/code&gt;&lt;code class=&quot;php plain&quot;&gt;&gt;&lt;!--?php&lt;span&gt; &lt;/span&gt;&lt;/code&gt;&lt;code class=&quot;php functions&quot;&gt;echo&lt;/code&gt; &lt;code class=&quot;php variable&quot;&gt;$this&lt;/code&gt;&lt;code class=&quot;php plain&quot;&gt;---&gt;__(&lt;/code&gt;&lt;code class=&quot;php string&quot;&gt;'Search:'&lt;/code&gt;&lt;code class=&quot;php plain&quot;&gt;) ?&gt;&lt;/label&gt;&lt;/code&gt;&lt;/div&gt;
&lt;div class=&quot;line number4 index3 alt1&quot;&gt;&lt;code class=&quot;php plain&quot;&gt;&lt;input id=&lt;/code&gt;&lt;code class=&quot;php string&quot;&gt;&quot;search&quot;&lt;/code&gt; &lt;code class=&quot;php keyword&quot;&gt;class&lt;/code&gt;&lt;code class=&quot;php plain&quot;&gt;=&lt;/code&gt;&lt;code class=&quot;php string&quot;&gt;&quot;input-text&quot;&lt;/code&gt; &lt;code class=&quot;php plain&quot;&gt;name=&lt;/code&gt;&lt;code class=&quot;php string&quot;&gt;&quot;&lt;?php echo $this-&gt;helper('catalogsearch')-&gt;getQueryParamName() ?&gt;&quot;&lt;/code&gt; &lt;code class=&quot;php plain&quot;&gt;type=&lt;/code&gt;&lt;code class=&quot;php string&quot;&gt;&quot;text&quot;&lt;/code&gt; &lt;code class=&quot;php plain&quot;&gt;value=&lt;/code&gt;&lt;code class=&quot;php string&quot;&gt;&quot;&lt;?php echo $this-&gt;helper('catalogsearch')-&gt;getEscapedQueryText() ?&gt;&quot;&lt;/code&gt;&lt;code class=&quot;php plain&quot;&gt;&gt;&lt;/code&gt;&lt;/div&gt;
&lt;div class=&quot;line number5 index4 alt2&quot;&gt;&lt;code class=&quot;php spaces&quot;&gt;        &lt;/code&gt;&lt;code class=&quot;php plain&quot;&gt;&lt;button&lt;span&gt; &lt;/span&gt;&lt;/code&gt;&lt;code class=&quot;php keyword&quot;&gt;class&lt;/code&gt;&lt;code class=&quot;php plain&quot;&gt;=&lt;/code&gt;&lt;code class=&quot;php string&quot;&gt;&quot;button&quot;&lt;/code&gt; &lt;code class=&quot;php plain&quot;&gt;title=&lt;/code&gt;&lt;code class=&quot;php string&quot;&gt;&quot;&lt;?php echo $this-&gt;__('Search') ?&gt;&quot;&lt;/code&gt;&lt;code class=&quot;php plain&quot;&gt;&gt;&lt;span&gt;&lt;span&gt;&lt;!--?php&lt;span&gt; &lt;/span&gt;&lt;/code&gt;&lt;code class=&quot;php functions&quot;&gt;echo&lt;/code&gt; &lt;code class=&quot;php variable&quot;&gt;$this&lt;/code&gt;&lt;code class=&quot;php plain&quot;&gt;---&gt;__(&lt;/code&gt;&lt;code class=&quot;php string&quot;&gt;'Search'&lt;/code&gt;&lt;code class=&quot;php plain&quot;&gt;) ?&gt;&lt;/span&gt;&lt;/span&gt;&lt;/button&gt;&lt;/code&gt;&lt;/div&gt;
&lt;div class=&quot;line number6 index5 alt1&quot;&gt;&lt;/div&gt;
&lt;div class=&quot;line number7 index6 alt2&quot;&gt;&lt;code class=&quot;php spaces&quot;&gt;        &lt;/code&gt;&lt;code class=&quot;php plain&quot;&gt;&lt;script type=&lt;/code&gt;&lt;code class=&quot;php string&quot;&gt;&quot;text/javascript&quot;&lt;/code&gt;&lt;code class=&quot;php plain&quot;&gt;&gt;&lt;/script&gt;&lt;/div&gt;&lt;/code&gt;&lt;/div&gt;
&lt;div class=&quot;line number8 index7 alt1&quot;&gt;&lt;code class=&quot;php plain&quot;&gt;&lt;/form&gt;&lt;/code&gt;&lt;/div&gt;
&lt;pre&gt;[/php]

<span><span><span><span>
to the code that you copied from Google custom search control panel</span></span></span></span></li>
 	<li><strong>That's it!</strong> you have added google custom search to your magento store. Here are some screenshots of the search user interface which you can further change from your control panel. Here is a <a href="https://cse.google.com/cse/create/getcode?cx=012278024424817052234%3Aocuhgvaknyy" target="_blank" rel="noopener">demo link</a> built on the data of cosjj ( a magento store).<img src="https://blog.expertrec.com/wp-content/uploads/2018/07/gcse5.png" alt="magento google custom search" width="935" height="522" class="alignnone wp-image-1842 size-full" /></li>
</ol>
</li>
</ol>
&nbsp;

&nbsp;