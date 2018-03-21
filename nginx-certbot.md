### This is a markdown file
## certbot + nginx
Autorenew of certificate with certbot does not work when nginx is running.

root crontab set to stop/renew/start once per day as follows:

```27 1 * * *   service nginx stop; /var/inpho/bin/certbot-auto renew; service nginx start```

Note -- renewal check doesn't require nginx to stop, but actually renewal may.  However, need to check out --webroot method for certbot-auto
