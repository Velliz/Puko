# Puko - V0.93 Beta [![Build Status](https://travis-ci.org/Velliz/puko.svg?branch=master)](https://travis-ci.org/Velliz/puko) [![Total Downloads](https://poser.pugx.org/velliz/puko/downloads)](https://packagist.org/packages/velliz/puko) [![Latest Stable Version](https://poser.pugx.org/velliz/puko/v/stable)](https://packagist.org/packages/velliz/puko) [![Coverage Status](https://coveralls.io/repos/github/Velliz/puko/badge.svg?branch=master)](https://coveralls.io/github/Velliz/puko?branch=master)

Puko is the Micro MVC PHP Framework for faster PHP application Development.

*Puko Require* **PHP 5.3** *or greater*

Download via composer:
```
composer create-project velliz/puko --prefer-dist --stability="dev" --no-install
```
Or checkout the lastest [zipped](https://github.com/Velliz/puko/releases) package.

## Main Features

**URL Routing**

Basic URL routing follows these rules:
```PHP
localhost/[controller]/
localhost/[controller]/[function]/
localhost/[controller]/[function]/[var1]/[var2]/[var3]/
localhost/[controller]/[ID]/[function]/[var1]/[var2]/[var3]/
```
**Data Access**

Database Access can configure via **Config/db.php** and you can use static **Data.php** class to perform CRUD operations like:
```PHP
Data::To("table name")->Save($arraydata);
Data::To("table name")->Update($arraywhere, $arraydata);
Data::To("table name")->Delete($arraydata);
Data::From("your query here")->FetchAll();
```
**Template Engine**

Puko use **.html** file for view. So if you want to do styling or scripting:
```
<!--@css{bootstrap.min,datatable}-->
<!--@js{jquery.min,datatable.min}-->
```
And the **.html** file has always have their partners. **.css** and **.js** located in Assets

For data Boilerplates, you can print data returned by Controller class like this:
```
{!value}
{!loop} {!value} {/loop}
{!!condition} {/condition}
```

And many more you can find in the [Documentation](https://github.com/Velliz/puko/wiki/Welcome-to-Puko-Docs)

## About

Crafted with <3 from **Bandung**, Indonesia.

If you find bugs error or you want contribute to this project. 

just send me email to : diditvelliz@gmail.com 

Thanks :)

Copyright **2016 - Didit Velliz**
