Password Generator Bundle
=========================


[![Build Status](https://travis-ci.org/hackzilla/password-generator-bundle.png?branch=master)](https://travis-ci.org/hackzilla/password-generator-bundle)
[![SensioLabsInsight](https://insight.sensiolabs.com/projects/022d0d22-f291-4923-8c03-14e665d94b9c/mini.png)](https://insight.sensiolabs.com/projects/022d0d22-f291-4923-8c03-14e665d94b9c)

Requirements
------------

PHP 5.3.2


Installation
------------

Add HackzillaPasswordGeneratorBundle in your composer.json:

```yaml
{
    "require": {
        "hackzilla/password-generator-bundle": "~1.0"
    }
}
```

Install Composer

```
curl -sS https://getcomposer.org/installer | php
mv composer.phar /usr/local/bin/composer
```

Now tell composer to download the library by running the command:

``` bash
$ composer update hackzilla/password-generator
```

Composer will install the bundle into your project's `vendor/hackzilla` directory.

### Step 2: Enable the bundle

Enable the bundle in the kernel:

``` php
<?php
// app/AppKernel.php

public function registerBundles()
{
    $bundles = array(
        // ...
        new Hackzilla\Bundle\PasswordGeneratorBundle\HackzillaPasswordGeneratorBundle(),
    );
}
```

### Step 3: Enable Translations

// app/config/config.yml
```yaml
framework:
    #esi:             ~
    translator:      { fallback: "en" }
```


Example Implementation
----------------------

See [Password generator app](https://github.com/hackzilla/password-generator-app)


Pull Requests
-------------

I'm open to pull requests for additional languages, features and/or improvements.
