# AGT PHP SDK

PHP client for the [American Gun Trader](https://americanguntrader.com/) Dealer API.

Namespace: **`ShadowSoftware\Agt`** (generated from `openapi.json` by
[`shadow-software/sdk-release`](https://github.com/shadow-software/sdk-release)).
Do not edit `generated/` by hand.

## Install

```bash
composer require shadow-software/agt-php-sdk
```

Requires PHP 8.1+.

Until Packagist lists the package, add a VCS repository:

```json
{
  "repositories": [
    { "type": "vcs", "url": "https://github.com/shadow-software/agt-php-sdk" }
  ],
  "require": {
    "shadow-software/agt-php-sdk": "^0.2"
  }
}
```

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
