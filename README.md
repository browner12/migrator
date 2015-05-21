# migrator

[![Latest Version](https://img.shields.io/github/release/browner12/migrator.svg?style=flat-square)](https://github.com/browner12/migrator/releases)
[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](LICENSE.md)
[![Build Status](https://img.shields.io/travis/browner12/migrator/master.svg?style=flat-square)](https://travis-ci.org/browner12/migrator)
[![Total Downloads](https://img.shields.io/packagist/dt/browner12/migrator.svg?style=flat-square)](https://packagist.org/packages/browner12/migrator)

This is a migrator package for PHP. It deviates from the traditional migration pattern by simply having a single file represent a table in the database. This package then analyzes the existing database schema, and the desired schema, and translates any differences into a set of executable queries.

## Who Should Use This Package

Use this package if you want each migrator file to represent a table in the database.

## Who Should Not Use This Package

Do not use this package if you like the traditional migration pattern of running `up` and `down` commands, and each file containing a specific set of directions to change your tables.

## Caution

Handling table and column renaming was the biggest hurdle when designing this package. Pay extra attention to how to handle renames, in order to prevent the loss of data.

## PSRs

This package follows PSR-1 and PSR-4. All contributions should follow these as well.

## Influence

This package was influenced by the Laravel migrator.

## Install

Via Composer

``` bash
$ composer require browner12/migrator
```

## Documentation

Please see the `docs` folder for full documentation.

## Testing

``` bash
$ phpunit
```

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

## Credits

- [Andrew Brown](https://github.com/browner12)

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
