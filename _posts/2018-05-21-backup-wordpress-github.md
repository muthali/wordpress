---
ID: 1665
post_title: >
  How to Backup your wordpress to github
  for free using github sync plugin
author: muthali ganesh
post_excerpt: ""
layout: post
permalink: >
  https://blog.expertrec.com/backup-wordpress-github/
published: true
post_date: 2018-05-21 13:00:28
---
In this article, we will see how to backup your wordpress site to github for free using the wordpress github sync plugin.

You can easily take backups of your wordpress site to github. In case if you lose some of your wordpress content, you can easily get back your lost content using github wordpress backup.

Steps-
<ol>
 	<li>Go to https://github.com/ and create a Github account if you don't have one.<img src="https://blog.expertrec.com/wp-content/uploads/2018/05/1-7.jpg" alt="wordpress github" width="1045" height="646" class="alignnone wp-image-1666 size-full" /></li>
 	<li>Sign in to your github account.<img src="https://blog.expertrec.com/wp-content/uploads/2018/05/2-7.jpg" alt="wordpress github" width="677" height="512" class="aligncenter wp-image-1667 size-full" /></li>
 	<li>Go to the + button icon on the top right and click on "new repository"<img src="https://blog.expertrec.com/wp-content/uploads/2018/05/3-7.jpg" alt="wordpress github" width="1043" height="356" class="alignnone wp-image-1668 size-full" /></li>
 	<li>Create a new respository-&gt; name it as "wordpress" (or anything you want). Make sure initialize this repository with a README is enabled. Click on create repository.<img src="https://blog.expertrec.com/wp-content/uploads/2018/05/4-6.jpg" alt="wordpress github" width="775" height="596" class="alignnone wp-image-1669 size-full" /></li>
 	<li>Now go to your wordpress control panel and go to Plugins-&gt; Add New. Search for "github sync". Install and activate "wordpress github sync".<img src="https://blog.expertrec.com/wp-content/uploads/2018/05/5-5.jpg" alt="wordpress github" width="1195" height="554" class="alignnone wp-image-1670 size-full" /></li>
 	<li>Go to settings-&gt; and click Github sync. Here enter the following details-
<ol>
 	<li>https://api.github.com</li>
 	<li>Repository <strong>your github username/repository name</strong> (For example- muthali/wordpress)<strong> </strong><img src="https://blog.expertrec.com/wp-content/uploads/2018/05/7-5.jpg" alt="wordpress github" width="732" height="331" class="aligncenter wp-image-1672" /></li>
</ol>
</li>
 	<li>Create a personal oauth token- Click on the personal oauth token link given in the dashboard. Give token description as "wordpress sync"  and<strong> scope as "public repo" </strong>and click generate token .<strong><img src="https://blog.expertrec.com/wp-content/uploads/2018/05/8-6.jpg" alt="wordpress github" width="1013" height="628" class="alignnone wp-image-1673 size-full" /><img src="https://blog.expertrec.com/wp-content/uploads/2018/05/9.jpg" alt="wordpress github" width="1048" height="381" class="alignnone wp-image-1675 size-full" /></strong></li>
 	<li><strong>Export to github</strong>- Now this will create a token for you. Copy paste this in your wordpress control panel and click on export to github. Now if you go to github profile-&gt; repositories-&gt; wordpress, you will find your wordpress site backup.<img src="https://blog.expertrec.com/wp-content/uploads/2018/05/11-4.jpg" alt="wordpress github" width="1013" height="419" class="alignnone wp-image-1679 size-full" /></li>
 	<li><strong>Go to wordpress folder</strong>-&gt;<img src="https://blog.expertrec.com/wp-content/uploads/2018/05/12-3.jpg" alt="wordpress github" width="1008" height="556" class="aligncenter wp-image-1680 size-full" /> <img src="https://blog.expertrec.com/wp-content/uploads/2018/05/13-4.jpg" alt="wordpress github" width="1001" height="571" class="aligncenter wp-image-1681 size-full" /></li>
 	<li>Here you can see that all your posts have been backed up.</li>
 	<li>How to restore- Go to settings-&gt; github sync-&gt; Import from Github<img src="https://blog.expertrec.com/wp-content/uploads/2018/05/14.jpg" alt="wordpress github" width="855" height="364" class="aligncenter wp-image-1682 size-full" /></li>
</ol>