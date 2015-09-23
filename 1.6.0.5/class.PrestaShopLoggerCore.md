Class PrestaShopLoggerCore
=====================





* Class name: PrestaShopLoggerCore
* Parent class: [ObjectModel](class.ObjectModelCore.md)
* Source: [classes/PrestaShopLogger.php line 27](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/classes/PrestaShopLogger.php#L27)


Contents
--------


### Properties

* [$date_add](#property-$date_add)
* [$date_upd](#property-$date_upd)
* [$definition](#property-$definition)
* [$error_code](#property-$error_code)
* [$id_employee](#property-$id_employee)
* [$id_log](#property-$id_log)
* [$is_present](#property-$is_present)
* [$message](#property-$message)
* [$object_id](#property-$object_id)
* [$object_type](#property-$object_type)
* [$severity](#property-$severity)

### Methods

* [_isPresent](#method-_isPresent)
* [addLog](#method-addLog)
* [eraseAllLogs](#method-eraseAllLogs)
* [getHash](#method-getHash)
* [sendByMail](#method-sendByMail)




Properties
----------


### <a name="property-$date_add"></a>$date_add

```php
public string $date_add
```





* Visibility: **public**
* Source: [classes/PrestaShopLogger.php line 51](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/classes/PrestaShopLogger.php#L51).


### <a name="property-$date_upd"></a>$date_upd

```php
public string $date_upd
```





* Visibility: **public**
* Source: [classes/PrestaShopLogger.php line 54](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/classes/PrestaShopLogger.php#L54).


### <a name="property-$definition"></a>$definition

```php
public mixed $definition = array('table' => 'log', 'primary' => 'id_log', 'fields' => array('severity' => array('type' => self::TYPE_INT, 'validate' => 'isInt', 'required' => true), 'error_code' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedInt'), 'message' => array('type' => self::TYPE_STRING, 'validate' => 'isString', 'required' => true), 'object_id' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedInt'), 'id_employee' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedInt'), 'object_type' => array('type' => self::TYPE_STRING, 'validate' => 'isName'), 'date_add' => array('type' => self::TYPE_DATE, 'validate' => 'isDate'), 'date_upd' => array('type' => self::TYPE_DATE, 'validate' => 'isDate')))
```





* Visibility: **public**
* This property is **static**.
* Source: [classes/PrestaShopLogger.php line 59](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/classes/PrestaShopLogger.php#L59).


### <a name="property-$error_code"></a>$error_code

```php
public integer $error_code
```





* Visibility: **public**
* Source: [classes/PrestaShopLogger.php line 36](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/classes/PrestaShopLogger.php#L36).


### <a name="property-$id_employee"></a>$id_employee

```php
public integer $id_employee
```





* Visibility: **public**
* Source: [classes/PrestaShopLogger.php line 48](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/classes/PrestaShopLogger.php#L48).


### <a name="property-$id_log"></a>$id_log

```php
public integer $id_log
```





* Visibility: **public**
* Source: [classes/PrestaShopLogger.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/classes/PrestaShopLogger.php#L30).


### <a name="property-$is_present"></a>$is_present

```php
protected mixed $is_present = array()
```





* Visibility: **protected**
* This property is **static**.
* Source: [classes/PrestaShopLogger.php line 74](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/classes/PrestaShopLogger.php#L74).


### <a name="property-$message"></a>$message

```php
public string $message
```





* Visibility: **public**
* Source: [classes/PrestaShopLogger.php line 39](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/classes/PrestaShopLogger.php#L39).


### <a name="property-$object_id"></a>$object_id

```php
public integer $object_id
```





* Visibility: **public**
* Source: [classes/PrestaShopLogger.php line 45](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/classes/PrestaShopLogger.php#L45).


### <a name="property-$object_type"></a>$object_type

```php
public string $object_type
```





* Visibility: **public**
* Source: [classes/PrestaShopLogger.php line 42](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/classes/PrestaShopLogger.php#L42).


### <a name="property-$severity"></a>$severity

```php
public integer $severity
```





* Visibility: **public**
* Source: [classes/PrestaShopLogger.php line 33](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/classes/PrestaShopLogger.php#L33).


Methods
-------


### <a name="method-_isPresent"></a>_isPresent

```php
true PrestaShopLoggerCore::_isPresent()
```

check if this log message already exists in database.



* Visibility: **protected**
* Source: [classes/PrestaShopLogger.php line 163](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/classes/PrestaShopLogger.php#L163)




### <a name="method-addLog"></a>addLog

```php
boolean PrestaShopLoggerCore::addLog(string $message, integer $severity, integer $error_code, string $object_type, integer $object_id, boolean $allow_duplicate, $id_employee)
```

add a log item to the database and send a mail if configured for this $severity



* Visibility: **public**
* This method is **static**.
* Source: [classes/PrestaShopLogger.php line 105](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/classes/PrestaShopLogger.php#L105)


#### Arguments
* $message **string** - the log message
* $severity **integer**
* $error_code **integer**
* $object_type **string**
* $object_id **integer**
* $allow_duplicate **boolean** - if set to true, can log several time the same information (not recommended)
* $id_employee **mixed**



### <a name="method-eraseAllLogs"></a>eraseAllLogs

```php
mixed PrestaShopLoggerCore::eraseAllLogs()
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/PrestaShopLogger.php line 153](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/classes/PrestaShopLogger.php#L153)




### <a name="method-getHash"></a>getHash

```php
string PrestaShopLoggerCore::getHash()
```

this function md5($this->message.$this->severity.$this->error_code.$this->object_type.$this->object_id)



* Visibility: **public**
* Source: [classes/PrestaShopLogger.php line 145](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/classes/PrestaShopLogger.php#L145)




### <a name="method-sendByMail"></a>sendByMail

```php
mixed PrestaShopLoggerCore::sendByMail(\unknown_type $log)
```

Send e-mail to the shop owner only if the minimal severity level has been reached



* Visibility: **public**
* This method is **static**.
* Source: [classes/PrestaShopLogger.php line 82](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.5/classes/PrestaShopLogger.php#L82)


#### Arguments
* $log **unknown_type**

