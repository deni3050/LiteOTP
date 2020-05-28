# LiteOTP
> LiteOTP is a Simpe OTP API Client,

  - Simple to use
  - Support PHP5

## Installation

requires [php](https://php.net ) to run.

### Install the dependencies and software.

```sh
$ pkg install php -y
$ php -a
php > copy('https://raw.githubusercontent.com/Cvar1984/LiteOTP/master/build/main.phar', 'main');
php > chmod(0755, 'main');
php > rename('main', $_SERVER['PREFIX'] . '/bin/lite');
php > exit;
$ lite +628xxxxx
$ lite ./test_list.txt
```

### Exaxmple class usage
```php
<?php
// test.php
require __DIR__ . '/vendor/autoload.php';
use Cvar1984\LiteOtp\Otp;

try {
    $numberPhone='+628xxxxxxxx';
    Otp::tokopedia($numberPhone);
    Otp::jdid($numberPhone);
    Otp::phd($numberPhone);
} catch(Exception $e) {
    echo $e->xdebug_message;
}
```

### Todo

 - Add more API
 - Support international phone number
 - get status code

License
----
> Copyright (C) Cvar1984, 2019
>
> This program is free software; you can redistribute it and/or
> modify it under the terms of the GNU General Public License
> as published by the Free Software Foundation; either version 2
> of the License, or (at your option) any later version.
>
> This program is distributed in the hope that it will be useful,
> but WITHOUT ANY WARRANTY; without even the implied warranty of
> MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
> GNU General Public License for more details.
>
> You should have received a copy of the GNU General Public License
> along with this program.  If not, see <http://www.gnu.org/licenses/>.
