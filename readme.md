# datahoarder.space

This is the repository for the datahoarder.space knowledge base for the data hoarder community.

## Our infrastructure

We use Jigsaw, a Laravel-based static site framework that uses markdown as well as blade templating to make it easy to make changes and improve our site. We also use Tailwind CSS as well as Fontawesome icons throughout our site.

## Contributing

To contribute, first fork the site. Make some changes and then submit a pull request. Pull requests are checked once every week. If you want to host while you make your changes please ensure you run the following commands (after installing npm and composer):

```
composer install
npm install
cp config.sample.php config.php
npm run watch
```

| Command  | What and why |
| ------------- | ------------- |
| composer install  | Uses the composer.json configuration file to install all required composer-based packages to dev and run the site locally.  |
| npm install  | Uses the package-lock.json configuration file to install all required node-based (could use yarn to also do this) packages to compile the site with Laravel Mix and node-sass  |
| npm run watch | Compiles sass/js assets, compiles static site then serves static site on port 3000 |


