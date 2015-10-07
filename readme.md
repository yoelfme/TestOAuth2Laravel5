## OAuth2 Server

This is a mini application that implement the library [oauth2-server-laravel](https://github.com/lucadegasperi/oauth2-server-laravel) for create a server of OAuth2 with [Laravel](http://laravel.com/)


### Environment Setup

- Clone the repo.
  - By SSH, run the command `git clone git@github.com:yoelfme/TestOAuth2Laravel5.git`
  - By HTTPS, run the command `git clone https://github.com/yoelfme/TestOAuth2Laravel5.git`
- Install dependencies, via `composer udpate`, if you have erros run `composer install`
- Configure environment, in the file `.env`

```
DB_HOST=localhost
DB_DATABASE=oauth2_server1
DB_USERNAME=homestead
DB_PASSWORD=secret
```

- Run migrations, via `php artisan migrate`
- Run seeders, via `php artisan db:seed`
- Test the application via CURL o Postman, send the fields by method POST to URL `urlproject/oauth/access_token`.

```
grant_type: client_credentials
client_secret: secret
client_id: test
```

---

Create with :heart: by [yoelfme](https://github.com/yoelfme).