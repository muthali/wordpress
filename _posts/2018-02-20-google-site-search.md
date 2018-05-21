---
ID: 947
post_title: Google site search
author: melchi
post_excerpt: ""
layout: post
permalink: >
  https://blog.expertrec.com/google-site-search/
published: true
post_date: 2018-02-20 15:00:57
---
Google Site Search Engine - How does it work? You login into google site search console, enter your URL and bam! you have ready site search engine code to add to your website in minutes. How Google does this?

Google is a web search engine.  Google Site Search is a product where one can use Google Web Search for powering the site search.

<img src="https://blog.expertrec.com/wp-content/uploads/2018/02/google-site-search.png" alt="google site search" width="560" height="315" class="size-full wp-image-991 aligncenter" />

&nbsp;

&nbsp;

In this article we will cover-
<ol>
 	<li><strong><em>How Google Web Search works</em></strong></li>
 	<li><strong><em>What components of Google Web Search are re-used for Site Search</em></strong>.  We will try and cover how this is implemented behind the scene.</li>
</ol>
<p style="text-align: center;">[inbound_button font_size="20" color="<span>#51b049</span>" text_color="#ffffff" icon="" url="https://cse.expertrec.com?platform=cse" width="" target="_blank"]Add search to my website[/inbound_button]</p>


[caption id="attachment_949" align="aligncenter" width="962"]<img src="https://blog.expertrec.com/wp-content/uploads/2018/02/how_google_works.jpg" alt="google site search" width="962" height="1220" class="wp-image-949 size-full" /> google site search[/caption]

<span>Source: </span><strong>Tham Yuen-C</strong><span> &amp; </span><strong>Quek Hong Shin</strong>

There are roughly 3 major components makes the google site search suite-

<strong>Google site search Crawler</strong> -

<strong>What is a crawler?-</strong> A crawler is a software program that visits websites and reads its pages and creates entries for a search engine index. These are also called as bots or spiders. The web crawler starts with a initial list of URLs crawl

<strong>Crawler main characteristics-</strong>

Google's crawler is a highly resilient one and it has a great balance between latency and throughput.

<strong>Latency</strong> - the amount of time it takes for a newly discovered page to be made available in the results page.  <strong>Throughput-</strong> the number of pages that gets re-crawled and updated in the search results.

If we crawl one page at a time and update the index, it will be having a much lower Latency, but the Throughput will suffer greatly.  Google will not be able to crawl the entire web, one page at a time.  If we update the index every 1million pages, it might be too late for a news page to be made available in the results.  Google has a very elaborate setup to handle this (probably another article down the line).  Another important aspect one has to consider when building a crawler is not to overload the webserver in which the pages are hosted.  This is called politeness.  If the server is loaded, the bots give it enough breathing time between requests so that regular users are not affected by the crawl.  When we built our crawler(Expertrec Bot), we have given it a great amount of consideration.

<strong>Indexer</strong> - The crawler might have fetched a variety of documents.  Html, PDF, Word file, etc.  They all needs to be indexed so that they can come in the search results.  Most of the books have an index at the end.

[caption id="" align="aligncenter" width="500"]<img src="https://www.pdfindexgenerator.com/wp-content/uploads/2016/10/index_sample.jpg" width="500" height="364" alt="google site search" /> Search Index Site Search[/caption]

Having this index helps us quickly find a word in the book.  e.g. in the above Index, the word <strong>ABC</strong> has occurred on pages <strong>164</strong> and <strong>321</strong>.  Creating this data of Word=&gt;Location is the job of an Indexer.  To facilitate various search operations, the Index has to be built accordingly.  Google's indexer not only have to be CPU efficient, but the generated index size also has to be quite small.  If you created a bloated index, you wont be able to hold the index for billions of documents.  Our indexer was built to handle only 10s of millions of documents (not Billions) as Google.  Yes, We know we might have to re-write it sooner :)
<ol>
 	<li>Search operation - Once the Index is built, a query (search term) can be made to retrieve the search results.  Search results for a multi-word query like "Site Search Replacement" happens by looking up "Site", "Search" and "Replacement" in the index.  The list of documents with each of the words will be retrieved from the index.  e.g. if "Site" is present in documents [1,2,3,4,5,6], "Search" is present in documents [2,4,6,8] and "Replacement" is present in documents [3,6,9,12].  The <strong>intersection</strong> of the above 3 <strong>sets</strong> gives the list of documents with all the 3 words.  i.e. Document [6] has all of "Site", "Search" and "Replacement" words in it.  Hence is the most relevant result from the Information retreival point of view (IR score).  There are various other relevance scoring mechanism that are together considered when the results are created.  Google claims to be using more than 200 such signals, including but not limited to "page rank", "domain authority", "recency", "TF/IDF", prominence of the words in the document etc.</li>
</ol>
In Google Site Search, in addition to retrieving the search results, (the set intersection operation) we talked about in the above paragraph, there is a list which has the documents that are present only in your website.  i.e. if your site is wikipedia.org and documents [1,..100] are present in wikipedia.org, then before returning the search results, Google does a set intersection with this set as well, so that only documents in 1-100 alone are returned (there by only wikipedia.org results come in the results).  By leveraging their existing crawler, indexer and search server, Google just made a minimum change to support Google Site Search and have there by powered many many site searches.

Google Site Search is getting discontinued unfortunately.  Shameless plug : We (Expertrec) are offering a drop in replacement for Google Site Search at 9$ per 1000 documents.   We will be happy to on board you there.