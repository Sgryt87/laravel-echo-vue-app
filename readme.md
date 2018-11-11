```bash
cd laravel-echo-vue-app
cp .env.example .env
composer update
npm install
php artisan key:generate

#.env 
DB_CONNECTION=mysql
DB_DATABASE=laravel_echo
DB_USERNAME=root
DB_PASSWORD=root
#go https://pusher.com and create a free app, then 
PUSHER_APP_ID=your_pusher_app_id
PUSHER_APP_KEY=your_pusher_app_key
PUSHER_APP_SECRET=your_pusher_app_secret
PUSHER_APP_CLUSTER=your_pusher_cluster
BROADCAST_DRIVER=pusher

php artisan migrate

php artisan tinker:
    factory(App\User::class, 15)->create() 
    factory(App\Message::class, 150)->create()



npm run watch
```


