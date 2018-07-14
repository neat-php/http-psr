Neat HTTP PSR components
========================
[![Stable Version](https://poser.pugx.org/neat/http-psr/version)](https://packagist.org/packages/neat/http-psr)
[![Build Status](https://travis-ci.org/neat-php/http-psr.svg?branch=master)](https://travis-ci.org/neat-php/http-psr)

Neat HTTP PSR components allow for interoperability using industry standard
PSR-7 interfaces.

Getting started
---------------
To install this package, simply issue [composer](https://getcomposer.org) on the
command line:
```
composer require neat/http-psr
```

Now you can create PSR-7 compliant messages using Neat HTTP components:
```php
<?php

$request = Neat\Http\Request::capture();
$psrRequest = new Neat\Http\Psr\Request($request);

// ...

$response = new Neat\Http\Response("Here's my response");
$psrResponse = new Neat\Http\Psr\Response($response);
```
