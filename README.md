# Phan stubs for WordPress

[![CircleCI branch](https://img.shields.io/circleci/project/github/skaut/phan-wordpress-stubs/master.svg)](https://circleci.com/gh/skaut/workflows/phan-wordpress-stubs/tree/master)

This repo contains stubs for WordPress functions and classes to be used with [phan](https://github.com/phan/phan), the PHP static analyzer. This allows for better type-checking of a codebase as the stubs all have type information.

## Installation

```sh
$ composer require --dev skaut/phan-wordpress-stubs
```

Add to your '.phan/config.php':

```php
return [
	'directory_list' => [
		'vendor/skaut/phan-wordpress-stubs/stubs'
	],
	'exclude_analysis_directory_list' => [
		'vendor/skaut/phan-wordpress-stubs/stubs'
	]
];
```

## Completeness

The stubs are not complete. If you spot any missing functions or classes, please [open an issue](https://github.com/skaut/phan-wordpress-stubs/issues/new).
