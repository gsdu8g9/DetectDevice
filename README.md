DetectDevice 
============
[![Build Status](https://travis-ci.org/Kocal/DetectDevice.png?branch=master)](https://travis-ci.org/Kocal/DetectDevice)

DetectDevice is a little (~60 lines), simply, and functional PHP class which detect what kind of device is used to navigate on your website, a pc, a mobile, a tablet or a bot.


How use?
--------
#### Firstly, include DetectDevice class and initialize it
```php
<?php
require "class.DetectDevice.php";
$device = new DetectDevice();
// ...
```

#### Secondly, use methods to find what kind of device is used
```php
<?php
// return a boolean (true or false)
echo $device->isComputer();
echo $device->isMobile();
echo $device->isTablet();
echo $device->isBot();

// You can use the "getDeviceType()" to return a string
echo $device->getDeviceType(); // may return "computer", "mobile, "tablet", or "bot"
// ...
```

#### Thirdly, you can switch user-agent
```php
<?php
// first method : in the constructor
$device = new DetectDevice($userAgent);

// second method : with a method
$device->setUserAgent($userAgent);
```

#### Fourthly, profit!
