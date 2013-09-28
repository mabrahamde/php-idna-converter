# php-idna-converter

**mabrahamde/php-idna-converter** is a fork of [phlyLabs' pure PHP IDNA Converter](http://phlymail.com/en/downloads/idna-convert.html). It converts  internationalized domain names between UTF-8 and ASCII (punycode) notation.

Unlike the original **mabrahamde/php-idna-converter** is available on [packagist.org](packagist.org).

[Visit author's website](mabraham.de)

## Installation


### Via composer

Add the package to your `composer.json` file:


    {
      "require": {
        "mabrahamde/php-idna-converter": "dev-master",
      },
    }

Run `composer.phar update`.

## Usage

This library is used exactly as the original. The original documentation is available at `src/ReadMe.txt` and `src/example.php`.

The following example describes basic usage.

	<?php

	require_once('vendor/autoload.php');

	$idn = new idna_convert(array('idn_version' => 2008));

	echo $idn->encode('lübeck.de'); // prints 'xn--lbeck-kva.de'

	echo $idn->decode('xn--lbeck-kva.de') // prints 'lübeck.de'

	?>
	
## Contact

Do you have any questions or suggestions? Feel free to contact me at `dev ( at ) mabraham.de`.

[Visit author's website](mabraham.de)