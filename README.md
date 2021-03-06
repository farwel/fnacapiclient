# Fnac Marketplace API PHP Client
> A comprehensive PHP library to connect your shop to Fnac.com Marketplace

If you are managing a shop on Fnac.com Marketplace, you would probably want to automate some repetitive tasks upon offers or orders.
Fnac.com offers a REST API to take control over your account and this library can help you quickly develop your custom client to connect and use all the features of your Fnac Marketplace seller account.

## Installing / Getting started

Make sure your PHP version is at least 5.3.2, and that you have php5-xsl mod installed.
You will also need to have composer installed on your host.

Simply clone the project into a private directory:  
/!\ Important /!\ if you use symfony 2.8 please use the version tagged v2.0

```shell
git clone https://github.com/FnacMarketplace/fnacapiclient.git
```

And launch the installation

```shell
composer install
```

or with

```shell
php composer.phar install
```

Or download and extract the archive in that directory (https://marketplace.ws.fd-recette.net/docs/api/2.6/download/fnacapiclient.tgz)

## Configuration

Edit the config.yml file, and fill it in with your seller account test or production ids given by Fnac teams.

```shell
vi config/config.yml
```

You should be provided with 3 ids: partner_id, shop_id and key. As it is an .yml file, be careful on the indentation.
Here is an example:
```yaml
fnac_api_client:
  partner_id: 509490E8-7341-AE98-F708-11768C65539B
  shop_id: 0EA474BC-BE18-5F77-D7F0-E509DE2AABC6
  key: 0D00AF6D-D33F-B5F1-3A5F-BF153C8DAE08
  host: https://marketplace.ws.fd-recette.net/api.php
```

You are now ready to go.

## Features

The Fnac Marketplace PHP Client offers methods to call the available services such as:
* Create and update offers on your products
* Retrieve and update your orders status
* Exchange communications with customers about the offers or the orders
* Manage claims on orders and eventually refund them
* Retrieve the best prices among the competition

This client is shipped with a graphical user interface. Once your ids properly added in the config.yml file, you can open it in your browser at http://yourhost.com/your_project/index.php

## Documentation

The documentation of our API and a complete how-to-use guide is available on Fnac Marketplace API test sandbox here: https://marketplace.ws.fd-recette.net/docs/api/2.6/index.html
You will need to get your access by demanding it from the Fnac Marketplace commercial support. 

## Contributing

This library is already used as is by many Fnac Marketplace vendors, but it can now be improved by anyone.
If you'd like to contribute, please fork the repository and use a feature
branch. Any helping suggestions and pull requests are warmly welcome.

## Licensing

The code in this project is licensed under MIT license.
