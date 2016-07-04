Client for api zagruzka.com
===========================
Client for api zagruzka.com

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