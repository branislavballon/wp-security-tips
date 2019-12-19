
## LINKS
- [Acunetix - Top tips to prevent a WordPress hack](https://www.acunetix.com/websitesecurity/preventing-wordpress-hack/)
- [WordPress Username Enumeration Techniques and How to Fix Them](https://medium.com/@ahmed_elhady/wordpress-username-enumeration-techniques-2ca0510df632)



## .htaccess Disable xmlrpc and readme

```
#Block WordPress xmlrpc.php requests
<Files xmlrpc.php>
    order deny,allow
    deny from all
</Files>


#block readme.htm
<files readme.html>
    order allow,deny
    deny from all
</files>
```

## Full Path Dusclosure rss-functions.php
https://www.owasp.org/index.php/Full_Path_Disclosure
https://www.acunetix.com/vulnerabilities/web/wordpress-full-path-disclosure/

php.ini:
```
display_errors = 'off'
```
apache2.conf:
```
php_flag  display_errors  off
```

## Disable File Editing
define('DISALLOW_FILE_EDIT', true);
