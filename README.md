# Laravel quickstarts on Openshift

## Create app using this repo

### Use rhc

`rhc create-app xxxxxx php-5.3 -n yyyy --from-code git://github.com/twtstudio/openshift-laravel.git`

### Openshift origin quickstart

```
{"quickstart": {
  "id": "12",
  "name": "Laravel 4.1",
  "website": "http://www.laravel.com",
  "initial_git_url": "git://github.com/twtstudio/openshift-laravel.git",
  "cartridges": ["php-5"],
  "summary": "Laravel is a PHP web application framework with expressive, elegant syntax.",
  "tags": ["php", "framework", "mysql"],
  "admin_tags": []
}}
```

## Deploy first time

Comment L7 like `exit 0;` in `.openshift/action_hooks/build` to install dependencies for laravel.
