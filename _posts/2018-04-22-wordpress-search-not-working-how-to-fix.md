---
ID: 1206
post_title: 'WordPress search not working- How to fix'
author: muthali ganesh
post_excerpt: ""
layout: post
permalink: >
  https://blog.expertrec.com/wordpress-search-not-working-how-to-fix/
published: true
post_date: 2018-04-22 13:38:16
---
Let's face it- the default wordpress search is not great. If your wordpress search is not working it could manifest in one of the following ways-
<ol>
 	<li>wordpress search box is not displaying on your site.</li>
 	<li>wordpress search box is not returning results.</li>
 	<li>wordpress search results page is not loading after user entered search query.</li>
 	<li>wordpress search is not returning certain posts in search results.</li>
</ol>
In this article we will discuss on how to fix this issue without writing any code.

Here are steps to fix your wordpress search not working issue-
<ol>
 	<li><strong>Disable your existing wordpress search</strong>-
<ol>
 	<li>you can disable your search using the plugin - <a href="https://wordpress.org/plugins/disable-search/">Disable search</a>.</li>
 	<li>To do this manually, go to your functions.php file and add the following piece of code.<strong><img src="https://blog.expertrec.com/wp-content/uploads/2018/04/functions.php_.png" alt="wordpress search not working" width="995" height="485" class="aligncenter wp-image-1207 size-full" /></strong>
<pre>function wpb_filter_query( $query, $error = true ) {

if ( is_search() ) {

$query-&gt;is_search = false;

$query-&gt;query_vars[s] = false;

$query-&gt;query[s] = false;

if ( $error == true )

$query-&gt;is_404 = true;

}

}

add_action( 'parse_query', 'wpb_filter_query' );

add_filter( 'get_search_form', create_function( '$a', "return null;" ) );

function remove_search_widget() {

unregister_widget('WP_Widget_Search');

&amp;nbsp;

add_action( 'widgets_init', 'remove_search_widget' );
</pre>
<div class="line number1 index0 alt2">This will disable the search form from your site.</div></li>
</ol>
</li>
 	<li>Create a <strong>custom search engine</strong>-
<ul>
 	<li>Go to <a href="https://cse.expertrec.com?platform=cse">https://cse.expertrec.com?platform=cse</a>.</li>
 	<li>Enter your website url.<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/enter-url.png" alt="wordpress search not working" width="1235" height="533" class="aligncenter wp-image-1208 size-full" /></li>
 	<li>Enter sitemap Url (this will help restrict site urls within the posts that you want google to index)<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/sitemap.png" alt="wordpress search not working" width="1095" height="663" class="aligncenter wp-image-1209 size-full" /></li>
 	<li>wait for crawl to complete.</li>
 	<li>Get your custom search demo URL</li>
</ul>
</li>
 	<li>Install the plugin "<a href="https://wordpress.org/plugins/insert-headers-and-footers/" target="_blank" rel="noopener">insert headers and footers</a>".</li>
 	<li>Go to your expertrec dashboard and get the code for your custom search engine.<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/code.png" alt="wordpress search not working" width="1115" height="543" class="aligncenter wp-image-1211 size-full" /></li>
 	<li>Use the Insert headers plugin to add this code to the head section of your site.<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/headers-and-footers-2.png" alt="wordpress search not working" width="725" height="453" class="aligncenter wp-image-1212 size-full" /></li>
 	<li><strong>Adding this code</strong> will add a new search bar to your wordpress site. You will have complete control over your search function of your site. You can choose to show certain urls or not in search results using the plugin. You can use the default crawler to crawl and extract content that you want to show in search. You can also edit the look and feel of the search form and search results pages easily with the dashboard.<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/dashboard.png" alt="wordpress search not working" width="1088" height="400" class="aligncenter wp-image-1213 size-full" /></li>
 	<li>Your brand new wordpress search is up and running! Here are snapshots of the search form and the search results pages.</li>
 	<li><img src="https://blog.expertrec.com/wp-content/uploads/2018/04/search-ui.png" alt="wordpress search not working" width="992" height="640" class="aligncenter wp-image-1218 size-full" /><img src="https://blog.expertrec.com/wp-content/uploads/2018/04/search-demo.png" alt="wordpress search not working" width="1334" height="641" class="aligncenter wp-image-1217 size-full" /></li>
</ol>