# AliExpress PHP SDK

PHP SDK for integrating with AliExpress APIs

## Installation

```bash
composer require theprosolutionx/aliexpress-php-sdk
```

## Usage

```php
require_once __DIR__.'/vendor/autoload.php';

use AliExpress\IopClient;
use AliExpress\IopRequest;

$client = new IopClient('YOUR_APP_KEY', 'YOUR_APP_SECRET');
$request = new IopRequest('/api_endpoint', 'POST');
$request->addApiParam('param1', 'value1');

$response = $client->execute($request);
print_r($response);
```

## Configuration

Set your API credentials in environment variables:
```bash
export ALIEXPRESS_APP_KEY='your_app_key'
export ALIEXPRESS_APP_SECRET='your_app_secret'
```

## Examples

See the `demo/` directory for complete usage examples:
- Simple API call demo
- File upload demo
- Internal API demo

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request

## License

MIT
