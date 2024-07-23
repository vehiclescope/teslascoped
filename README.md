# Teslascoped
An open-source Tesla vehicle polling infrastructure and platform, intended for running on your own devices.

Teslascoped provides a lightweight backend and web-based client for monitoring and recording your vehicle's activity, including
driving and charging sessions, software updates, battery health, and more.

Easily import and export data interchangeably between the [Teslascope](https://teslascope.com/) live service for backup purposes.

### Core Features
- Driving and Charging Sessions with detailed breakdowns.
- Lifetime Statistics
- Software Updates History, with optional data from the global fleet.
- Locations
- Effortlessly import and export data to and from live Teslascope service.

### Setup
Teslascoped is powered by [Laravel](https://laravel.com), which requires [PHP8.1+](https://php.net), [Composer](https://getcomposer.org/) and [NPM](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm).

Within the repository directory, copy the file .env.example to .env, and then modify any options as necessary.
By default, Teslascoped utilizes SQLite for a database. However, you can adjust this to use a different connection if desired.

To install run the following:
```bash
composer install
npm run build
php artisan migrate
php artisan octane:install
```

To run the service:
```bash
php artisan optimize
php artisan octane:start
```
(This is subject to change before our first release.) 

### Considerations
To help alleviate initial development fatigue, not all features available on the live service will be implemented. Contributions
via Pull Requests are always appreciated, and will be considered.
