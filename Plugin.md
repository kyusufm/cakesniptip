I got 403 error after installing filemanager for tiny mce.

changes your .htaccess from

`<Files ~ "^.*">
  Deny from all
</Files>

<Files ~ "^index\.php|css|js|.*\.png|.*\.jpg|.*\.gif|.*\.woff2|.*\.eot|.*\.svg|.*\.ttf|.*\.woff">
  Allow from all
</Files>

into

<Files ~ "^.*">
  Deny from all
</Files>

<Files ~ "^index\.php|css|js|php|.*\.png|.*\.jpg|.*\.gif|.*\.woff2|.*\.eot|.*\.svg|.*\.ttf|.*\.woff">
  Allow from all
</Files>`
