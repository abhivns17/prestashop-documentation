Class AdminRequestSqlControllerCore
=====================





* Class name: AdminRequestSqlControllerCore
* Parent class: [AdminController](class.AdminControllerCore.md)
* Source: [controllers/admin/AdminRequestSqlController.php line 27](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/controllers/admin/AdminRequestSqlController.php#L27)


Contents
--------


### Properties

* [$encoding_file](#property-$encoding_file)

### Methods

* [__construct](#method-__construct)
* [_childValidation](#method-_childValidation)
* [ajaxProcess](#method-ajaxProcess)
* [displayError](#method-displayError)
* [displayExportLink](#method-displayExportLink)
* [generateExport](#method-generateExport)
* [initContent](#method-initContent)
* [initPageHeaderToolbar](#method-initPageHeaderToolbar)
* [initProcess](#method-initProcess)
* [initToolbar](#method-initToolbar)
* [postProcess](#method-postProcess)
* [renderForm](#method-renderForm)
* [renderList](#method-renderList)
* [renderOptions](#method-renderOptions)
* [renderView](#method-renderView)




Properties
----------


### <a name="property-$encoding_file"></a>$encoding_file

```php
public array $encoding_file = array(array('value' => 1, 'name' => 'utf-8'), array('value' => 2, 'name' => 'iso-8859-1'))
```





* Visibility: **public**
* This property is **static**.
* Source: [controllers/admin/AdminRequestSqlController.php line 32](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/controllers/admin/AdminRequestSqlController.php#L32).


Methods
-------


### <a name="method-__construct"></a>__construct

```php
mixed AdminRequestSqlControllerCore::__construct()
```





* Visibility: **public**
* Source: [controllers/admin/AdminRequestSqlController.php line 37](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/controllers/admin/AdminRequestSqlController.php#L37)




### <a name="method-_childValidation"></a>_childValidation

```php
mixed AdminRequestSqlControllerCore::_childValidation()
```





* Visibility: **public**
* Source: [controllers/admin/AdminRequestSqlController.php line 233](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/controllers/admin/AdminRequestSqlController.php#L233)




### <a name="method-ajaxProcess"></a>ajaxProcess

```php
mixed AdminRequestSqlControllerCore::ajaxProcess()
```

method call when ajax request is made with the details row action



* Visibility: **public**
* Source: [controllers/admin/AdminRequestSqlController.php line 182](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/controllers/admin/AdminRequestSqlController.php#L182)




### <a name="method-displayError"></a>displayError

```php
mixed AdminRequestSqlControllerCore::displayError($e)
```

Display all errors



* Visibility: **public**
* Source: [controllers/admin/AdminRequestSqlController.php line 377](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/controllers/admin/AdminRequestSqlController.php#L377)


#### Arguments
* $e **mixed** - : array of errors



### <a name="method-displayExportLink"></a>displayExportLink

```php
mixed AdminRequestSqlControllerCore::displayExportLink($token, $id)
```

Display export action link



* Visibility: **public**
* Source: [controllers/admin/AdminRequestSqlController.php line 249](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/controllers/admin/AdminRequestSqlController.php#L249)


#### Arguments
* $token **mixed**
* $id **mixed**



### <a name="method-generateExport"></a>generateExport

```php
mixed AdminRequestSqlControllerCore::generateExport()
```

Genrating a export file



* Visibility: **public**
* Source: [controllers/admin/AdminRequestSqlController.php line 323](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/controllers/admin/AdminRequestSqlController.php#L323)




### <a name="method-initContent"></a>initContent

```php
mixed AdminRequestSqlControllerCore::initContent()
```





* Visibility: **public**
* Source: [controllers/admin/AdminRequestSqlController.php line 271](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/controllers/admin/AdminRequestSqlController.php#L271)




### <a name="method-initPageHeaderToolbar"></a>initPageHeaderToolbar

```php
mixed AdminRequestSqlControllerCore::initPageHeaderToolbar()
```





* Visibility: **public**
* Source: [controllers/admin/AdminRequestSqlController.php line 308](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/controllers/admin/AdminRequestSqlController.php#L308)




### <a name="method-initProcess"></a>initProcess

```php
mixed AdminRequestSqlControllerCore::initProcess()
```





* Visibility: **public**
* Source: [controllers/admin/AdminRequestSqlController.php line 261](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/controllers/admin/AdminRequestSqlController.php#L261)




### <a name="method-initToolbar"></a>initToolbar

```php
mixed AdminRequestSqlControllerCore::initToolbar()
```





* Visibility: **public**
* Source: [controllers/admin/AdminRequestSqlController.php line 92](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/controllers/admin/AdminRequestSqlController.php#L92)




### <a name="method-postProcess"></a>postProcess

```php
mixed AdminRequestSqlControllerCore::postProcess()
```





* Visibility: **public**
* Source: [controllers/admin/AdminRequestSqlController.php line 166](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/controllers/admin/AdminRequestSqlController.php#L166)




### <a name="method-renderForm"></a>renderForm

```php
mixed AdminRequestSqlControllerCore::renderForm()
```





* Visibility: **public**
* Source: [controllers/admin/AdminRequestSqlController.php line 130](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/controllers/admin/AdminRequestSqlController.php#L130)




### <a name="method-renderList"></a>renderList

```php
mixed AdminRequestSqlControllerCore::renderList()
```





* Visibility: **public**
* Source: [controllers/admin/AdminRequestSqlController.php line 106](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/controllers/admin/AdminRequestSqlController.php#L106)




### <a name="method-renderOptions"></a>renderOptions

```php
mixed AdminRequestSqlControllerCore::renderOptions()
```





* Visibility: **public**
* Source: [controllers/admin/AdminRequestSqlController.php line 81](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/controllers/admin/AdminRequestSqlController.php#L81)




### <a name="method-renderView"></a>renderView

```php
mixed AdminRequestSqlControllerCore::renderView()
```





* Visibility: **public**
* Source: [controllers/admin/AdminRequestSqlController.php line 203](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/controllers/admin/AdminRequestSqlController.php#L203)


