Codeigniter-Smarty
=======================

Codeigniter + Smarty integration<br/>
<br/>

<h2>Versions:</h2>
Codeigniter 2.1.4<br/>
Smarty 3.1.16<br/>

<h2>Pre-configured:</h2>
- Smarty templating engine
- Demonstration templates to give an idea how it works
- Default DB driver MySQLi
- global_xss_filtering = TRUE
- Moved CodeIgniter outside the webroot
- Using a .htaccess to remove index.php from the URL

<h2>Installation and configuration</h2>
- Place all the files in the site's directory.<br/>
- Make sure you upload the files one folder above the <em>public_html</em> (or <em>www</em>, depending on your server)<br/>
- Change the config files to suit your needs<br/>

<h3>Encryption key</h3>
Make sure you change the encryption key inside <em>application/config/config.php</em><br/>
Look for: <em>$config['encryption_key'] = 'ENTERYOUROWNKEYHERE';<em><br/>
And replace <em>ENTERYOUROWNKEYHERE</em> with a unique key.<br/>

<h2>CodeIgniter inside the webroot (public_html/www)</h2>
If you do not like CodeIgniter being outside the webroot it can be changed quite easily.
All you have to do is:
- move the files inside the public_html to the folder above them (where the application and system folders are)
- open index.php
- change the system path to: $system_path = 'system';
- change the application folder to: $application_folder = 'application';
- delete the (now empty) public_html folder
- upload the files to your your server and enjoy!

<h2>Changelog</h2>
11-03-2014
- updated smarty to 3.1.16
- refactored custom smarty code
- updated the readme (from now on I will ignore this change because it will happen every time...)
<strong>Note:</strong> In this release the cache directory will change. So make sure to delete your old one, it's not needed anymore.


23-07-2013
- changed template extension to ".tpl"
- modified the demonstration templates to a structure users will probably use more often
- updated codeigniter to 2.1.4
- changed DBDriver to MySQLi
- updated the readme


14-02-2013
- initial commit

