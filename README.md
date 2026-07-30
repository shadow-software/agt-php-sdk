# AGT PHP SDK

PHP client for the [American Gun Trader](https://americanguntrader.com/) Dealer API.

Namespace: **`ShadowSoftware\Agt`** (generated from `openapi.json` by
[`shadow-software/sdk-release`](https://github.com/shadow-software/sdk-release)).
Do not edit `generated/` by hand.

## Install

```bash
composer require shadow-software/agt-php-sdk
```

Requires PHP 8.1+. On [Packagist](https://packagist.org/packages/shadow-software/agt-php-sdk).

## Usage

```php
use ShadowSoftware\Agt\Configuration;
use ShadowSoftware\Agt\Api\DealerListingApi;

$config = Configuration::getDefaultConfiguration()
    ->setHost('https://americanguntrader.com')
    ->setAccessToken($accessToken);

$api = new DealerListingApi(null, $config);
```

## License

MIT
