---
ID: 962
post_title: 'Indexing &#8220;behind login&#8221;/ Authenticated pages using expertrec custom search'
author: muthali ganesh
post_excerpt: ""
layout: post
permalink: >
  https://blog.expertrec.com/crawling-behind-login-authenticated-pages/
published: true
post_date: 2018-02-22 10:55:28
---
Sometimes you might want to add a search box to your authenticated pages ( pages that need a login for access). So while using a search engine crawler to index these pages, you have to give certain details so that it can go beyond the login pages. Doing this is very easy with expertrec site search engine.

Lets take an example. We want to index the following pages and the related URLs, <a href="https://www.thornburg.com/registration/logon.aspx" target="_blank" rel="noopener">https://www.thornburg.com/registration/logon.aspx</a><img src="https://blog.expertrec.com/wp-content/uploads/2018/02/thornburg1.png" alt="crawling behind login pages" width="1366" height="662" class="alignnone size-full wp-image-963" />
<ul>
 	<li>Go to <strong><a href="https://cse.expertrec.com">https://cse.expertrec.com</a></strong></li>
 	<li>Go to <strong>Crawl settings</strong></li>
 	<li>Go to <strong>Login Auth</strong></li>
</ul>
<a href="crawling behind login pages"><img src="https://blog.expertrec.com/wp-content/uploads/2018/02/thornburg1-1.png" alt="" width="1366" height="662" class="alignnone size-full wp-image-967" /></a>

Here<strong> login URL</strong> is the page URL. In this case it is <a href="https://www.thornburg.com/registration/logon.aspx">https://www.thornburg.com/registration/logon.aspx</a>

<strong>Login formid</strong>- To find the login form ID, open developer tools in your chrome browser (control+shift+i) and select the form element in the developer mode. In this case it is <strong>p_login<img src="https://blog.expertrec.com/wp-content/uploads/2018/02/p_login.jpg" alt="crawling behind login pages" width="825" height="552" class="alignnone size-full wp-image-968" /></strong>

<strong>Enter the id/name for username box- </strong>Select the id/name of the input box. Here it is <strong>p_txtUsername</strong><a href="crawling behind login pages"><img src="https://blog.expertrec.com/wp-content/uploads/2018/02/p_txtusername.jpg" alt="" width="820" height="541" class="alignnone size-full wp-image-969" /></a>

<strong>Enter the id/name for password box- </strong>In the inspect element mode, click on the password box for the password box id<img src="https://blog.expertrec.com/wp-content/uploads/2018/02/p_txtpassword.jpg" alt="crawling behind login pages" width="833" height="549" class="alignnone size-full wp-image-970" />

Enter a username and password for the crawler and press update.

Now go to the home page and press recrawl. Thats it. Now you can go to your demo page and check if your search results include the behind login pages or not.<img src="https://blog.expertrec.com/wp-content/uploads/2018/02/search.jpg" alt="crawling behind login pages" width="1342" height="662" class="alignnone size-full wp-image-971" />

&nbsp;