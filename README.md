# Deploy app



## Setup
Clone app
```bash
git clone https://github.com/TheYkk/laravel-weather
```
Create https://openweathermap.org/api token

Create google auth id for suppor to login with google.
Details: https://developers.google.com/identity/protocols/oauth2

Configure .env
```bash
APP_NAME=
APP_ENV=
APP_DEBUG=
APP_URL=
DB_CONNECTION=
DB_HOST=
DB_PORT=
DB_DATABASE=
DB_USERNAME=
DB_PASSWORD=
MAIL_MAILER=
MAIL_HOST=
MAIL_PORT=
MAIL_USERNAME=
MAIL_PASSWORD=
MAIL_ENCRYPTION=
MAIL_FROM_ADDRESS=

GOOGLE_CLIENT_ID=
GOOGLE_CLIENT_SECRET=
GOOGLE_REDIRECT=
WEATHER_API=
```


Composer install
```bash
composer install
```

Npm packages install
```bash
yarn install
#npm install 
```

Create css and js 
```bash
yarn prod
```

Generate key
```
php aritsan key:generate
```

Link Storage
```
php artisan storage:link
```

Run migrations
```
php artisan migrate:fresh --seed
```


## Setup cron
```bash
sudo crontab -e
```

Go the end of the file and include this line:
```bash
* * * * * php /path-to-your-project/artisan schedule:run >> /dev/null 2>&1
```
