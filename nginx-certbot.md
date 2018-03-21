## This is a markdown file
Autorenew of certificate with certbot does not work when nginx is running.

root crontab set to stop/renew/start once per day as follows:

```27 1 * * *   service nginx stop; /var/inpho/bin/certbot-auto renew; service nginx start```
