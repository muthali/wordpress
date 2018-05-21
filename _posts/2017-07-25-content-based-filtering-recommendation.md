---
ID: 51
post_title: CONTENT BASED FILTERING RECOMMENDATION
author: muthali ganesh
post_excerpt: ""
layout: post
permalink: >
  https://blog.expertrec.com/content-based-filtering-recommendation/
published: true
post_date: 2017-07-25 14:37:37
---
What is a content based filtering recommendation engine?

A recommendation engine picks up the best items out of a large number of items to display to a user. Content based recommender picks up these items based on the content/ characteristics of these items. It doesnt take into consideration users' preferences/ ratings. You might have seen on many e-commerce sites recommendation such as similar products which are based on some similarity algorithm.

<img class="alignnone size-full wp-image-183" src="https://blog.expertrec.com/wp-content/uploads/2017/07/content-based-filtering-1.jpg" alt="content based filtering recommendation" width="1289" height="307" />

Why do businesses implement recommendation engines?
<ol>
 	<li>To cut the time for product discovery.</li>
 	<li>To boost sales by upselling, cross selling and bundling.</li>
</ol>
Content based recommenders, recommend items that are similar to the current item. <span style="color: #3c4858; font-size: 16px;">They focus on properties of items. </span><span style="color: #3c4858; font-size: 16px;">Similarity is determined by finding out how similar their properties are.</span>

There first step is to have a item profile for all the items/ products in your inventory. <span style="color: #3c4858; font-size: 16px;">For example - for an iphone, profile can be price, display size, RAM, storage capacity etc.</span>

Item profiles can be easy to get in a few cases like mobile phones, in some other cases like images or articles, it is difficult to get.

Here are commonly used content based filtering methods-
<ol>
 	<li>1.TF/IDF</li>
 	<li>Neural Networks</li>
 	<li>Clustering algorithms.</li>
 	<li>Jaccard similarity</li>
 	<li>Cosine similarity</li>
</ol>
The TF IDF method-
<ol>
 	<li>Remove stop words- Example – and, the , of , but …</li>
 	<li>Calculate TF.IDF score (term frequency multiplied by inverse document frequency) which gives the importance of a word.</li>
</ol>
Term frequency- <span style="color: #3c4858; font-size: 16px;"> Measures how frequently a term occurs in a document.</span>
<ul>
 	<li>TF(t) = (Number of times term t appears in a document) / (Total number of terms in the document)</li>
 	<li>IDF(t) = log_e(Total number of documents / Number of documents with term t in it)</li>
</ul>
Example-

Lets assume that there are two documents and they contain the following words.

<style type="text/css"><!--td {border: 1px solid #ccc;}br {mso-data-placement:same-cell;}--></style>
<table dir="ltr" border="1" cellspacing="0" cellpadding="0"><colgroup> <col width="100" /> <col width="100" /> <col width="100" /></colgroup>
<tbody>
<tr>
<td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Document 1&quot;}"><strong>Document 1</strong></td>
<td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Word&quot;}"><strong>Word</strong></td>
<td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;count&quot;}"><strong>count</strong></td>
</tr>
<tr>
<td></td>
<td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;the&quot;}">the</td>
<td data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:2}">2</td>
</tr>
<tr>
<td></td>
<td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;apple&quot;}">apple</td>
<td data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1}">1</td>
</tr>
<tr>
<td></td>
<td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;tree&quot;}">tree</td>
<td data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:3}">3</td>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Document 2&quot;}"><strong>Document 2</strong></td>
<td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Word&quot;}"><strong>Word</strong></td>
<td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;count&quot;}"><strong>count</strong></td>
</tr>
<tr>
<td></td>
<td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;the&quot;}">the</td>
<td data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1}">1</td>
</tr>
<tr>
<td></td>
<td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;orange&quot;}">orange</td>
<td data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:2}">2</td>
</tr>
<tr>
<td></td>
<td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;tree&quot;}">tree</td>
<td data-sheets-value="{&quot;1&quot;:3,&quot;3&quot;:1}">1</td>
</tr>
</tbody>
</table>
Calculating Term frequency and inverse document frequency in d1 and d2

TF (“tree”, d1)= 3/6=0.5  TF (“tree”, d2)= 1/4=0.25

IDF(“tree”,D)=log(2/2)=0

<strong>TFT IDF(“tree”, d1)=0  TFT IDF(“tree”, d2)=0</strong>

TF (“apple”, d1)= 1/6=0.2   TF (“apple”, d2)=0/4=0

IDF(“apple”,D)=log(2/1)=0.3

<strong>TFT IDF(“apple”, d1)=0.2*0.3=.06            TFT IDF(“apple”, d2)=0*0.3=0</strong>

As you can see, the TF IDF scores are used in most of the text based recommender systems.

After calculating, TF IDF, to find out which items are close to each other , we can use multiple similarity algorithms such as cosine similarity, jaccard index etc.
<p style="text-align: center;">[inbound_button font_size="20" color="#c8232b" text_color="#ffffff" icon="" url="https://magento.expertrec.com/signup" width="" target="_blank"]Sign-Up[/inbound_button]</p>