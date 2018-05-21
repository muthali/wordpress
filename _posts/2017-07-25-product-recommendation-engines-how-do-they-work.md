---
ID: 48
post_title: 'PRODUCT RECOMMENDATION ENGINES- HOW DO THEY WORK?'
author: muthali ganesh
post_excerpt: ""
layout: post
permalink: >
  https://blog.expertrec.com/product-recommendation-engines-how-do-they-work/
published: true
post_date: 2017-07-25 14:34:32
---
<img class="alignnone size-full wp-image-450" src="https://expertreco.files.wordpress.com/2017/05/product-recommendation-engine.jpg?w=700" sizes="(max-width: 700px) 100vw, 700px" srcset="https://expertreco.files.wordpress.com/2017/05/product-recommendation-engine.jpg?w=700 700w, https://expertreco.files.wordpress.com/2017/05/product-recommendation-engine.jpg?w=150 150w, https://expertreco.files.wordpress.com/2017/05/product-recommendation-engine.jpg?w=300 300w, https://expertreco.files.wordpress.com/2017/05/product-recommendation-engine.jpg?w=768 768w, https://expertreco.files.wordpress.com/2017/05/product-recommendation-engine.jpg?w=1024 1024w, https://expertreco.files.wordpress.com/2017/05/product-recommendation-engine.jpg 1171w" alt="product recommendation engine" data-attachment-id="450" data-permalink="https://blog.expertrec.com/2017/05/19/product-recommendation-engine-getting-started/product-recommendation-engine/" data-orig-file="https://expertreco.files.wordpress.com/2017/05/product-recommendation-engine.jpg?w=700" data-orig-size="1171,317" data-comments-opened="1" data-image-meta="{&quot;aperture&quot;:&quot;0&quot;,&quot;credit&quot;:&quot;muthali&quot;,&quot;camera&quot;:&quot;&quot;,&quot;caption&quot;:&quot;&quot;,&quot;created_timestamp&quot;:&quot;1495233018&quot;,&quot;copyright&quot;:&quot;&quot;,&quot;focal_length&quot;:&quot;0&quot;,&quot;iso&quot;:&quot;0&quot;,&quot;shutter_speed&quot;:&quot;0&quot;,&quot;title&quot;:&quot;&quot;,&quot;orientation&quot;:&quot;0&quot;}" data-image-title="Product recommendation engine" data-image-description="" data-medium-file="https://expertreco.files.wordpress.com/2017/05/product-recommendation-engine.jpg?w=700?w=300" data-large-file="https://expertreco.files.wordpress.com/2017/05/product-recommendation-engine.jpg?w=700?w=700" />

A recommendation engine involves connecting users to products/ items.

Lets take an example. Let’s assume we have ratings for products . In an e-commerces store these might be implicit signals such as view, add to cart, buy , remove from cart, time spent on a product and much more.

For simplicity we will take ratings on a scale of (1-5). C1,C2.. are customers and P1, P2 .. are products. C1 has rated P1 4, C2 has rated P2 5 etc . The recommendation engine’s goal is to predict what would customer 3’s rating would be for P2 using the given ratings(or any other blank cell in the matrix).
<table dir="ltr" border="1" cellspacing="0" cellpadding="0"><colgroup> <col width="100" /> <col width="100" /> <col width="100" /> <col width="100" /> <col width="100" /></colgroup>
<tbody>
<tr>
<td></td>
<td>P1</td>
<td>P2</td>
<td>P3</td>
<td>P4</td>
</tr>
<tr>
<td>C1</td>
<td>4</td>
<td></td>
<td>1</td>
<td>5</td>
</tr>
<tr>
<td>C2</td>
<td></td>
<td>5</td>
<td></td>
<td>3</td>
</tr>
<tr>
<td>C3</td>
<td>3</td>
<td>?</td>
<td></td>
<td></td>
</tr>
<tr>
<td>C4</td>
<td></td>
<td>2</td>
<td></td>
<td>3</td>
</tr>
</tbody>
</table>
<ul>
 	<li style="list-style-type: none;">
<ul style="text-align: left;">Recommendations are classified according to how these blanks in this matrix are filled.</ul>
</li>
</ul>
<ul>
 	<li>Content based- using properties of items.</li>
 	<li>Collaborative filtering (CF)- using similarity of items and/or similarity of users. The items recommended to the user.
<ul>
 	<li>Neighborhood based approach</li>
 	<li>Model based approach.</li>
 	<li>Hybrid models.</li>
</ul>
</li>
 	<li>Hybrid – CF + content based approach.</li>
</ul>
Hope this gives a simple introduction into what recommender systems are all about, I will discuss in detail more of these methods in my future posts.
<p style="text-align: center;">[inbound_button font_size="20" color="#c8232b" text_color="#ffffff" icon="" url="https://magento.expertrec.com/signup" width="" target="_blank"]Sign-Up[/inbound_button]</p>
&nbsp;

<a href="https://www.expertrec.com/product-recommendation-engine/">Read more..</a>