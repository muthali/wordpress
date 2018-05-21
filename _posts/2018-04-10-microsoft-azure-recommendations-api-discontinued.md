---
ID: 1134
post_title: 'Microsoft azure recommendation API discontinued- What next?'
author: muthali ganesh
post_excerpt: ""
layout: post
permalink: >
  https://blog.expertrec.com/microsoft-azure-recommendations-api-discontinued/
published: true
post_date: 2018-04-10 14:55:43
---
Microsoft Azure recommendations API (microsoft azure congnitive services) has been shut down as of Feb 15th 2018. If you have been using this service, you might be looking to replace your recommendation engine. Expertrec recommendation engine is a good alternative to microsoft azure recommendations.This article gives a brief on how to move to expertrec's recommendation engine.

<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/Recommendation-API.png" alt="Azure recommendation API" width="736" height="324" class="aligncenter wp-image-1135 size-full" />

<strong>About Expertrec-</strong>

Expertrec is a SAAS solution,similar to the microsoft cognitive services recommendations. Expertrec provides recommendations through a real time API. These recommendations can be consumed over desktop, mobile, call centres or in kiosks in your physical stores.

<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/recommendation-engine.png" alt="Azure recommendation API" width="768" height="512" class="aligncenter wp-image-1136 size-full" />

<strong>How does Expertrec recommendation engine work?</strong>

Expertrec recommendation engine works by learning from user behavior across your website, mobile and other channels.

You have to add expertrec's Javascript to your website. This Javascript learns from website user's behavior and creates user profiles and product profiles that are merged to generate recommendations.

On a high level two types of recommendations are generated-
<ol>
 	<li>Product to product/ Item to item recommendations (P2P)- This could be recommendations such as customers who viewed this item also viewed, similar products etc.</li>
 	<li>User to product recommendations (U2P)- Recommended for you, recently viewed etc.</li>
</ol>
These recommendations evolve in real time for every individual customer browsing on your website applications.

<strong>High level architecture-</strong>

<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/recommend2.jpeg" alt="Azure recommendation API" width="707" height="400" class="aligncenter wp-image-1137 size-full" />

&nbsp;

<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/User-behavior-on-website-mobileweb.png" alt="Azure recommendation API" width="1024" height="768" class="aligncenter wp-image-1138 size-full" />

&nbsp;
<ol>
 	<li>Create an account at <a href="https://cse.expertrec.com" target="_blank" rel="noopener">https://cse.expertrec.com</a></li>
 	<li>Add Javascript code to your website. (<a href="https://docs.google.com/spreadsheets/d/1rXd3v6tQlj-7SgIrNuBI4oUePHmmPUkIQrE6zdggFIc/edit#gid=0">click here</a> to get javascript code for your website)</li>
 	<li>Upload your inventory in CSV / JSON format (If you have a feed link (google product feed), you can enter that link as well.</li>
 	<li>Map your fields.</li>
 	<li>Choose recommendations to be generated. ( VAV, similar products etc)</li>
 	<li>Visit recommendations API page at ( <a href="http://expertrec.com/api/#api-reqRecData" target="_blank" rel="noopener">http://expertrec.com/api/#api-reqRecData</a> )<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/get-recommendations.png" alt="Azure recommendation API" width="993" height="663" class="aligncenter wp-image-1139 size-full" /><img src="https://blog.expertrec.com/wp-content/uploads/2018/04/rec-example.png" alt="Azure recommendation API" width="988" height="570" class="aligncenter wp-image-1140 size-full" /></li>
 	<li>Integrate to your website or apps.</li>
 	<li>You could also choose for expertrec to build your UI. The Javascript code added will generate the recommendation widget on your website and mobile web.</li>
</ol>