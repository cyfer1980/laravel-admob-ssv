# Laravel Google AdMob Server-side Verification
The library help you to verify Admob callback in server.

## Install
```
composer require cyfer1980/laravel-admob-ssv
```


## How to use

```php
use Casperlaitw\LaravelAdmobSsv\AdMob;
use Illuminate\Http\Request;

public function callback(Request $request) {
    $adMob = new AdMob($request);
    if ($adMob->validate()) {
        // success
    } else {
        // failed
    }
}
```
