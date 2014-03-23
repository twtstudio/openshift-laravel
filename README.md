# Laravel quickstarts on Openshift

## Requirement(s)

- Openshift Composer Cartridge: https://github.com/twtstudio/openshift-composer

## Openshift origin quickstart

```
{"quickstart": {
  "id": "12",
  "name": "Laravel 4.1",
  "website": "http://www.laravel.com",
  "initial_git_url": "git://github.com/twtstudio/openshift-laravel.git",
  "cartridges": ["php-5", "composer"],
  "summary": "Laravel is a PHP web application framework with expressive, elegant syntax.",
  "tags": ["php", "framework", "mysql", "laravel", "composer"],
  "admin_tags": []
}}
```
## First commit

Once your laravel app was created, you need to rename `composer.json.example` to `composer.json` to make your app work.

```
$ git mv composer.json.example
$ git add composer.json
$ git commit -m 'enable composer'
$ git push -u origin master
```

## Markers

- markers for composer: https://github.com/twtstudio/openshift-composer#markers

## I'm unable too add the openshift composer cartridge

Please checkout branch `raw` to quickstart your laravel app without a composer cartridge.
