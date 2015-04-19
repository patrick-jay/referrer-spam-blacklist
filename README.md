Reusable list of referrer spammers

TODO: introduction to explain why and promote Piwik

## Usage

The list is stored in this repository in `spammers.txt`. This text file contains one host per line.

You can [download this file manually](https://github.com/piwik/referrer-spam-blacklist/blob/master/spammers.txt), download the [whole folder as zip](https://github.com/piwik/referrer-spam-blacklist/archive/master.zip) or clone the repository using git:

```
git clone https://github.com/piwik/referrer-spam-blacklist.git
```

If you are using PHP, you can also install the list through Composer:

```
composer require piwik/referrer-spam-blacklist
```

Parsing the file should be pretty easy using your favorite language. Beware that the file can contain empty lines.

Here is an example using PHP:

```php
$list = file('spammers.txt', FILE_IGNORE_NEW_LINES | FILE_SKIP_EMPTY_LINES);
```

## Contributing

Contributing a new host to the list can be done by either opening a new issue or a pull request. Please check if somebody already reported the host before opening a new one.

If you open a pull request, remember to keep one host per line without any extra character (e.g. no comma). The list should be kept ordered alphabetically. You should use [Linux line endings](http://en.wikipedia.org/wiki/Newline).

## Disclaimer

This list of Referrer spammers is contributed by the community and is provided as is, without any guarantee. Using this list is under your own responsibility and risk.

## License

Public Domain (no copyright).
