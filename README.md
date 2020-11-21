# Next version

WIP

# twitchls

Watch Twitch streams via HLS. Works on Safari 6+ (5+ for iOS), Chrome for Android 30+ and Edge on Windows 10. If the used browser does not support HLS it loads the stream via an experimental HTML5 Twitch.tv feature (tested on latest Chrome and Firefox). If this feature is disabled, Flash is used. Built using [Laravel 8](https://laravel.com/), [Alpine.js](https://github.com/alpinejs/alpine) and [TailwindCSS](https://tailwindcss.com/).

This application is running on [twitchls.com](https://twitchls.com).

## Development

```shell
composer install
npm install

# Frontend development
npm run dev

# For production
npm run build

# Tests
vendor/bin/phpunit
```

In order to Login via Twitch and load the followed streams you need to [register your application on the Twitch.tv website](http://www.twitch.tv/settings/connections). After you've registered, fill the `TWITCH_CLIENT_ID`, `TWITCH_CLIENT_SECRET` and `TWITCH_REDIRECT_URL` with the appropriate values in the `.env` file.

## License

Twitchls is licensed under the [MIT license](http://opensource.org/licenses/MIT).
