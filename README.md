Client for api zagruzka.com
===========================
Client for api zagruzka.com

[![Latest Stable Version](https://poser.pugx.org/sevenfloor/yii2-zagruzka/version)](https://packagist.org/packages/sevenfloor/yii2-zagruzka)
[![Total Downloads](https://poser.pugx.org/sevenfloor/yii2-zagruzka/downloads)](https://packagist.org/packages/sevenfloor/yii2-zagruzka)
[![Latest Unstable Version](https://poser.pugx.org/sevenfloor/yii2-zagruzka/v/unstable)](//packagist.org/packages/sevenfloor/yii2-zagruzka)
[![License](https://poser.pugx.org/sevenfloor/yii2-zagruzka/license)](https://packagist.org/packages/sevenfloor/yii2-zagruzka)
[![composer.lock available](https://poser.pugx.org/sevenfloor/yii2-zagruzka/composerlock)](https://packagist.org/packages/sevenfloor/yii2-zagruzka)


Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist sevenfloor/yii2-zagruzka "*"
```

or add

```
"sevenfloor/yii2-zagruzka": "*"
```

to the require section of your `composer.json` file.


Usage
-----

Add this to your main configuration's components array:

```php
'clientZagruzka' => [
            'class' => \sevenfloor\zagruzka\ClientZagruzka::className() ,
            'url' => 'zagruzka.url',
            'login' => 'your_login',
            'pass' => 'your_password',
            'urlCallback' => 'partner.url'
        ],
```
Typical component usage
-----------------------
```php
Yii::$app->clientZagruzka->pay(phone, sum);
Yii::$app->clientZagruzka->balance();
```
