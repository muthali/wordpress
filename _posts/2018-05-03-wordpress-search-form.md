---
ID: 1295
post_title: How to add a wordpress search form
author: muthali ganesh
post_excerpt: ""
layout: post
permalink: >
  https://blog.expertrec.com/wordpress-search-form/
published: true
post_date: 2018-05-03 15:25:01
---
In this article, we will see how you can create a custom wordpress search form using two different methods- by adding code, and not adding code.

<strong>Method 1- Wordpress search form by adding some code.</strong>

All wordpress sites come with a default search form. Given that you are here, you want to edit the look and feel of your search form- The placeholder, the submit button, size of the search box etc.

You can add a search form by including<em><strong> </strong></em><span><em><strong>&lt;?php get_search_form(); ?&gt;</strong></em> in your wordpress template. </span>

For creating a custom search form, create a new php file called searchform.php and save it to your themes folder. You can add the following form code to this file.
<pre>&lt;form role="search" method="get" class="searchform group" action="&lt;?php echo home_url( '/' ); ?&gt;"&gt; &lt;label&gt; &lt;span class="offscreen"&gt;&lt;?php echo _x( 'Search for:', 'label' ) ?&gt;&lt;/span&gt; &lt;input type="search" class="search-field" placeholder="&lt;?php echo esc_attr_x( 'Search', 'placeholder' ) ?&gt;" value="&lt;?php echo get_search_query() ?&gt;" name="s" title="&lt;?php echo esc_attr_x( 'Search for:', 'label' ) ?&gt;" /&gt; &lt;/label&gt; &lt;input type="image" alt="Submit search query" src="&lt;?php echo get_template_directory_uri(); ?&gt;/images/search-icon.png"&gt; &lt;/form&gt;
</pre>
<strong>Method 2- Wordpress search from by creating a custom search engine ( no coding method)</strong>

This method involves creating a custom search engine using expertrec.

-&gt;Go to <a href="https://cse.expertrec.com?platform=cse">https://cse.expertrec.com?platform=cse</a>

-&gt;Enter your website URL.

-&gt;Wait for crawl to complete.

-&gt;Get code.

-&gt;Install the plugin - <a href="https://wordpress.org/plugins/insert-headers-and-footers/" target="_blank" rel="noopener">Insert Headers and footers.</a>

-&gt;Add this code to your website using the insert headers and footers

<img src="https://blog.expertrec.com/wp-content/uploads/2018/05/code.png" alt="wordpress search form" width="785" height="663" class="aligncenter wp-image-1296 size-full" />

This code will display the search form and the search results pages.<img src="https://blog.expertrec.com/wp-content/uploads/2018/05/search-from.png" alt="wordpress search form" width="867" height="505" class="aligncenter wp-image-1297 size-full" />

You can edit the look and feel of the search from by going to <em>Look and feel-&gt;Input box/ search results .</em>

<img src="https://blog.expertrec.com/wp-content/uploads/2018/05/look-and-feel.png" alt="wordpress search form" width="1277" height="775" class="aligncenter wp-image-1298 size-full" />