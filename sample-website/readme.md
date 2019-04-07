This contain sample website which you can

Simple nginx host html


docker-compose need to add the following environment variable
```
     WORDPRESS_CONFIG_EXTRA: |
        define( 'WP_HOME', 'https://wordpress.sharechiwai.com/' );
        define( 'WP_SITEURL', 'https://wordpress.sharechiwai.com/' );
        $$_SERVER['HTTPS']       = 'on';
        $$_SERVER['SERVER_PORT'] = '443';
        define('FORCE_SSL_ADMIN', true);
        $$_SERVER['HTTP_HOST'] = $$_SERVER['HTTP_X_FORWARDED_HOST'];
```