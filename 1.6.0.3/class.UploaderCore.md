Class UploaderCore
=====================





* Class name: UploaderCore
* Source: [classes/Uploader.php line 27](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.3/classes/Uploader.php#L27)


Contents
--------

### Constants

* [DEFAULT_MAX_SIZE](#constant-DEFAULT_MAX_SIZE)

### Properties

* [$_accept_types](#property-$_accept_types)
* [$_files](#property-$_files)
* [$_max_size](#property-$_max_size)
* [$_name](#property-$_name)
* [$_save_path](#property-$_save_path)

### Methods

* [__construct](#method-__construct)
* [_getFileSize](#method-_getFileSize)
* [_getServerVars](#method-_getServerVars)
* [_normalizeDirectory](#method-_normalizeDirectory)
* [getAcceptTypes](#method-getAcceptTypes)
* [getFilePath](#method-getFilePath)
* [getFiles](#method-getFiles)
* [getMaxSize](#method-getMaxSize)
* [getName](#method-getName)
* [getPostMaxSizeBytes](#method-getPostMaxSizeBytes)
* [getSavePath](#method-getSavePath)
* [getUniqueFileName](#method-getUniqueFileName)
* [process](#method-process)
* [setAcceptTypes](#method-setAcceptTypes)
* [setMaxSize](#method-setMaxSize)
* [setName](#method-setName)
* [setSavePath](#method-setSavePath)
* [upload](#method-upload)
* [validate](#method-validate)


Constants
----------


### <a name="constant-DEFAULT_MAX_SIZE"></a>DEFAULT_MAX_SIZE

```php
const DEFAULT_MAX_SIZE = 10485760
```





* Source: [classes/Uploader.php line 29](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.3/classes/Uploader.php#L29).


Properties
----------


### <a name="property-$_accept_types"></a>$_accept_types

```php
private mixed $_accept_types
```





* Visibility: **private**
* Source: [classes/Uploader.php line 31](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.3/classes/Uploader.php#L31).


### <a name="property-$_files"></a>$_files

```php
private mixed $_files
```





* Visibility: **private**
* Source: [classes/Uploader.php line 32](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.3/classes/Uploader.php#L32).


### <a name="property-$_max_size"></a>$_max_size

```php
private mixed $_max_size
```





* Visibility: **private**
* Source: [classes/Uploader.php line 33](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.3/classes/Uploader.php#L33).


### <a name="property-$_name"></a>$_name

```php
private mixed $_name
```





* Visibility: **private**
* Source: [classes/Uploader.php line 34](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.3/classes/Uploader.php#L34).


### <a name="property-$_save_path"></a>$_save_path

```php
private mixed $_save_path
```





* Visibility: **private**
* Source: [classes/Uploader.php line 35](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.3/classes/Uploader.php#L35).


Methods
-------


### <a name="method-__construct"></a>__construct

```php
mixed UploaderCore::__construct($name)
```





* Visibility: **public**
* Source: [classes/Uploader.php line 37](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.3/classes/Uploader.php#L37)


#### Arguments
* $name **mixed**



### <a name="method-_getFileSize"></a>_getFileSize

```php
mixed UploaderCore::_getFileSize($file_path, $clear_stat_cache)
```





* Visibility: **protected**
* Source: [classes/Uploader.php line 221](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.3/classes/Uploader.php#L221)


#### Arguments
* $file_path **mixed**
* $clear_stat_cache **mixed**



### <a name="method-_getServerVars"></a>_getServerVars

```php
mixed UploaderCore::_getServerVars($var)
```





* Visibility: **protected**
* Source: [classes/Uploader.php line 228](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.3/classes/Uploader.php#L228)


#### Arguments
* $var **mixed**



### <a name="method-_normalizeDirectory"></a>_normalizeDirectory

```php
mixed UploaderCore::_normalizeDirectory($directory)
```





* Visibility: **protected**
* Source: [classes/Uploader.php line 233](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.3/classes/Uploader.php#L233)


#### Arguments
* $directory **mixed**



### <a name="method-getAcceptTypes"></a>getAcceptTypes

```php
mixed UploaderCore::getAcceptTypes()
```





* Visibility: **public**
* Source: [classes/Uploader.php line 49](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.3/classes/Uploader.php#L49)




### <a name="method-getFilePath"></a>getFilePath

```php
mixed UploaderCore::getFilePath($file_name)
```





* Visibility: **public**
* Source: [classes/Uploader.php line 54](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.3/classes/Uploader.php#L54)


#### Arguments
* $file_name **mixed**



### <a name="method-getFiles"></a>getFiles

```php
mixed UploaderCore::getFiles()
```





* Visibility: **public**
* Source: [classes/Uploader.php line 62](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.3/classes/Uploader.php#L62)




### <a name="method-getMaxSize"></a>getMaxSize

```php
mixed UploaderCore::getMaxSize()
```





* Visibility: **public**
* Source: [classes/Uploader.php line 76](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.3/classes/Uploader.php#L76)




### <a name="method-getName"></a>getName

```php
mixed UploaderCore::getName()
```





* Visibility: **public**
* Source: [classes/Uploader.php line 90](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.3/classes/Uploader.php#L90)




### <a name="method-getPostMaxSizeBytes"></a>getPostMaxSizeBytes

```php
mixed UploaderCore::getPostMaxSizeBytes()
```





* Visibility: **public**
* Source: [classes/Uploader.php line 101](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.3/classes/Uploader.php#L101)




### <a name="method-getSavePath"></a>getSavePath

```php
mixed UploaderCore::getSavePath()
```





* Visibility: **public**
* Source: [classes/Uploader.php line 119](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.3/classes/Uploader.php#L119)




### <a name="method-getUniqueFileName"></a>getUniqueFileName

```php
mixed UploaderCore::getUniqueFileName($prefix)
```





* Visibility: **public**
* Source: [classes/Uploader.php line 127](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.3/classes/Uploader.php#L127)


#### Arguments
* $prefix **mixed**



### <a name="method-process"></a>process

```php
mixed UploaderCore::process()
```





* Visibility: **public**
* Source: [classes/Uploader.php line 132](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.3/classes/Uploader.php#L132)




### <a name="method-setAcceptTypes"></a>setAcceptTypes

```php
mixed UploaderCore::setAcceptTypes($value)
```





* Visibility: **public**
* Source: [classes/Uploader.php line 43](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.3/classes/Uploader.php#L43)


#### Arguments
* $value **mixed**



### <a name="method-setMaxSize"></a>setMaxSize

```php
mixed UploaderCore::setMaxSize($value)
```





* Visibility: **public**
* Source: [classes/Uploader.php line 70](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.3/classes/Uploader.php#L70)


#### Arguments
* $value **mixed**



### <a name="method-setName"></a>setName

```php
mixed UploaderCore::setName($value)
```





* Visibility: **public**
* Source: [classes/Uploader.php line 84](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.3/classes/Uploader.php#L84)


#### Arguments
* $value **mixed**



### <a name="method-setSavePath"></a>setSavePath

```php
mixed UploaderCore::setSavePath($value)
```





* Visibility: **public**
* Source: [classes/Uploader.php line 95](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.3/classes/Uploader.php#L95)


#### Arguments
* $value **mixed**



### <a name="method-upload"></a>upload

```php
mixed UploaderCore::upload($file, $dest)
```





* Visibility: **public**
* Source: [classes/Uploader.php line 161](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.3/classes/Uploader.php#L161)


#### Arguments
* $file **mixed**
* $dest **mixed**



### <a name="method-validate"></a>validate

```php
mixed UploaderCore::validate($file)
```





* Visibility: **protected**
* Source: [classes/Uploader.php line 193](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.3/classes/Uploader.php#L193)


#### Arguments
* $file **mixed**


