---
ID: 1236
post_title: WordPress login not working! How to fix?
author: muthali ganesh
post_excerpt: ""
layout: post
permalink: >
  https://blog.expertrec.com/wordpress-login-not-working/
published: true
post_date: 2018-04-27 13:45:52
---
If your wordpress login is not working, it could be due to this one of the following reasons.
<ol>
 	<li>Password reset is not working</li>
 	<li>Issues due to cookies.</li>
 	<li>An empty page appears or it throws a PHP error message.</li>
 	<li>You are getting a 404 not found error.</li>
 	<li>Wordpress URL redirects or page refreshes.</li>
</ol>
<strong>Wordpress login not working due to - Password reset is not working :</strong>
You can try to fix this issue by clicking on the "lost your password" link. You will be taken to a page <img src="https://blog.expertrec.com/wp-content/uploads/2018/04/rest-password.jpg" alt="wordpress login not working" width="601" height="514" class="aligncenter wp-image-1237 size-full" />

Sometimes you might not get the password reset email. Now you have to edit your password manually.

<strong>Reset password by editing your database -</strong>

Before attempting this step- backup your wordpress website.
<ul>
 	<li>Login into your cpanel.</li>
 	<li>Go to database section.</li>
 	<li>Click on Phpmyadmin. <img src="https://blog.expertrec.com/wp-content/uploads/2018/04/1-2.png" alt="wordpress login not working" width="1366" height="662" class="aligncenter wp-image-1245 size-full" /></li>
 	<li>Click on databases.<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/2-2.png" alt="wordpress login not working" width="1366" height="662" class="aligncenter wp-image-1246 size-full" /></li>
 	<li>Click on wordpress database.<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/3.png" alt="wordpress login not working" width="1366" height="662" class="aligncenter wp-image-1247 size-full" /></li>
 	<li>Click on wp_users<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/4-1.png" alt="wordpress login not working" width="1366" height="662" class="aligncenter wp-image-1248 size-full" /></li>
 	<li>Click on edit<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/5-1.png" alt="wordpress login not working" width="1366" height="662" class="aligncenter wp-image-1249 size-full" /></li>
 	<li>Enter your new password in "user_pass" box, select md5 from function drop down list and click go.<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/6-1.png" alt="wordpress login not working" width="1366" height="662" class="aligncenter wp-image-1250 size-full" /></li>
</ul>
<strong>Reset your password using functions.php file</strong>

You will need ftp access to access this functions.php file.

Here are the steps-
<ul>
 	<li>login to your ftp account<span><img src="https://blog.expertrec.com/wp-content/uploads/2018/04/Login-to-your-FTP-account-1024x814.jpg" alt="wordpress login not working" width="1024" height="703" class="aligncenter wp-image-1238 size-full" /></span></li>
 	<li>Go to themes folder "<span>xx/wp-content/themes/[your theme name]" <img src="https://blog.expertrec.com/wp-content/uploads/2018/04/Go-to-theme-1024x812.jpg" alt="wordpress login not working" width="1024" height="677" class="aligncenter wp-image-1239 size-full" /></span></li>
 	<li>Download functions.php<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/Download-the-functions-1024x812.jpg" alt="" width="1024" height="706" class="alignnone size-full wp-image-1240" /></li>
 	<li>Delete the old password and enter your new password<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/Delete-the-pre-entered-1024x668.jpg" alt="wordpress login not working" width="1024" height="668" class="aligncenter wp-image-1241 size-full" /></li>
 	<li><span>Upload this functions.php file to your FTP.<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/Upload-the-edited-functions-1024x812.jpg" alt="wordpress login not working" width="1024" height="705" class="aligncenter wp-image-1242 size-full" /></span></li>
</ul>
<strong>Wordpress login not working due to cookies issues</strong>

Wordpress needs cookies to be enabled to work properly. Check if you browser cookies are enabled or not in your browser. If they are not enabled, then enable it. Press control+shift+delete to go to cookie settings in chrome browser and enable. After doing this, you can try to login to your wordpress account.<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/cookies.jpg" alt="wordpress login not working" width="750" height="606" class="aligncenter wp-image-1251 size-full" />

&nbsp;

<strong>Wordpress login not working when you are shown a blank page or a php error message is shown- </strong>

<strong>Disable plugins using FTP</strong>- Since you dont have access to your admin panel, you will have to use FTP access to your site plugins and disable them. You can use filezilla FTP client to access your wordpress files.

Rename the plugins folder so that wordpress can no longer load the plugins. <img src="https://blog.expertrec.com/wp-content/uploads/2018/04/filezilla_2017-04-30_10-10-57.png" alt="wordpress login not working" width="1366" height="570" class="aligncenter wp-image-1253 size-full" />

<strong>Remove your theme using FTP</strong>

Access your wordpress files using Filezilla or any other FTP client.

Filezilla will show site files and folders. locate the folder that has your wordpress files. Usually this is "public_html"<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/public_html.png" alt="wordpress login not working" width="1355" height="576" class="aligncenter wp-image-1254 size-full" />

Search for "wp_content"<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/wp_content.png" alt="wordpress login not working" width="1366" height="571" class="aligncenter wp-image-1255 size-full" />

Open the themes folder<strong><img src="https://blog.expertrec.com/wp-content/uploads/2018/04/themes-folder.png" alt="wordpress login not working" width="1366" height="620" class="aligncenter wp-image-1256 size-full" /></strong>

Search for the themes folder and rename it . This will disable the theme<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/rename-theme.png" alt="wordpress login not working" width="1366" height="619" class="aligncenter wp-image-1257 size-full" />

Now try login in to your admin panel . If you are able to login it means your current theme is the reason you are not able to login.

<strong>Wordpress login not working due to 404 not found error or url redirects or page refreshes- </strong>

Disable .htcaccess files using ftp client-

Open the public_html folder <img src="https://blog.expertrec.com/wp-content/uploads/2018/04/public_html.png" alt="wordpress login not working" width="1355" height="576" class="aligncenter wp-image-1254 size-full" />

Search for <strong>.htcaccess</strong> file and rename it<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/htcaccess.png" alt="wordpress login not working" width="1364" height="569" class="alignnone wp-image-1258 size-full" />

Now try the login  again.

<strong>Change your site URL-</strong>

Access your site site using ftp. find the file containing your wordpress files (public_html)<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/public_html.png" alt="wordpress login not working" width="1355" height="576" class="aligncenter wp-image-1254 size-full" />

Find <span>wp_config.php file. Right click and click on view/edit the file and open with any text editor of your choice.<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/wp_content-1.png" alt="wordpress login not working" width="1366" height="571" class="aligncenter wp-image-1259 size-full" /> </span>

Click on view/edit<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/view_edit.png" alt="wordpress login not working" width="1366" height="570" class="aligncenter wp-image-1260 size-full" />

<span>Add these two lines of code.</span>

<code>define('WP_HOME','<a class="vglnk" href="http://example.com/" rel="nofollow"><span>https</span><span>://</span></a>yourwebsiteurl.com');</code>

<code>define('WP_SITEURL','<a class="vglnk" href="http://example.com/" rel="nofollow"><span>https</span><span>://</span></a>yourwebsiteurl.com');</code>

After saving the file wait for upload to complete.<img src="https://blog.expertrec.com/wp-content/uploads/2018/04/upload.png" alt="wordpress login not working" width="1366" height="568" class="aligncenter wp-image-1261 size-full" />

Now try login in after going to your new site URL.