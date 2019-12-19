## .htaccess

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
