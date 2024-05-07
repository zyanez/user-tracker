# user-tracker 🕵️‍♀️

Laravel package for retrieving user browser, operating system, and device type.

## Features 🛠️

- Easily obtain the user's operating system, browser, preferred language, and device type 🖥️.
- User-agent parsers for quickly understanding user information such as the above, preferred language, browser, etc. 🕵️‍♂️

## Quickstart 🚀

To install user-tracker and use it, follow these steps:

1. In your Laravel project, run the command `composer require zyanez/user-tracker`.
2. Add the following line at the top of the PHP file where you intend to utilize this code:
  ```php
  use Zyanez\UserTracker\UserTracker;
  ```
4. Use the commands below in documentation!

## Documentation

### Initialization
To start gathering information about the user's environment using the UserTracker class, you must first create an instance of it:
```php
$userTracker = new UserTracker();
```

### Get user's browser
This method identifies the user's web browser by examining the User-Agent header sent by the browser:
```php
$browser = $userTracker->getUserBrowser();
```

### Get user's OS
Similarly, this method identifies the user's operating system by analyzing the User-Agent header:
```php
$os = $userTracker->getUserOS();
```

### Get user's device type
This method determines the type of device the user is using, whether it's a desktop, mobile, or tablet:
```php
$deviceType = $userTracker->getUserDevice();
```
### Get user's prefered language
Lastly, this method retrieves the user's preferred language based on the Accept-Language header sent by their browser:
```php
$language = $userTracker->getUserLanguage();
```

## License 📝

This project is licensed under the [MIT](https://github.com/zyanez/user-tracker?tab=MIT-1-ov-file#) License.

## Contribution 🤝

If you find a bug or have any feature suggestions to enhance the project, feel free to contribute!
