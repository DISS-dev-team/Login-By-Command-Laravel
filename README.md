# Login-By-Command-Laravel

```php
$response = [];

$request = new Request();

$request->offsetSet('key','value');

$user = User::where('email', 'email')->first();

Auth::login($user);

$request->setUserResolver(function () use ($user) {
    return $user;
});
```
