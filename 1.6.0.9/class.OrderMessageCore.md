Class OrderMessageCore
=====================





* Class name: OrderMessageCore
* Parent class: [ObjectModel](class.ObjectModelCore.md)
* Source: [classes/order/OrderMessage.php line 27](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.9/classes/order/OrderMessage.php#L27)


Contents
--------


### Properties

* [$date_add](#property-$date_add)
* [$definition](#property-$definition)
* [$message](#property-$message)
* [$name](#property-$name)
* [$webserviceParameters](#property-$webserviceParameters)

### Methods

* [getOrderMessages](#method-getOrderMessages)




Properties
----------


### <a name="property-$date_add"></a>$date_add

```php
public string $date_add
```





* Visibility: **public**
* Source: [classes/order/OrderMessage.php line 36](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.9/classes/order/OrderMessage.php#L36).


### <a name="property-$definition"></a>$definition

```php
public mixed $definition = array('table' => 'order_message', 'primary' => 'id_order_message', 'multilang' => true, 'fields' => array('date_add' => array('type' => self::TYPE_DATE, 'validate' => 'isDate'), 'name' => array('type' => self::TYPE_STRING, 'lang' => true, 'validate' => 'isGenericName', 'required' => true, 'size' => 128), 'message' => array('type' => self::TYPE_STRING, 'lang' => true, 'validate' => 'isMessage', 'required' => true, 'size' => 1200)))
```





* Visibility: **public**
* This property is **static**.
* Source: [classes/order/OrderMessage.php line 41](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.9/classes/order/OrderMessage.php#L41).


### <a name="property-$message"></a>$message

```php
public string $message
```





* Visibility: **public**
* Source: [classes/order/OrderMessage.php line 33](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.9/classes/order/OrderMessage.php#L33).


### <a name="property-$name"></a>$name

```php
public string $name
```





* Visibility: **public**
* Source: [classes/order/OrderMessage.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.9/classes/order/OrderMessage.php#L30).


### <a name="property-$webserviceParameters"></a>$webserviceParameters

```php
protected mixed $webserviceParameters = array('fields' => array('id' => array('sqlId' => 'id_discount_type', 'xlink_resource' => 'order_message_lang'), 'date_add' => array('sqlId' => 'date_add')))
```





* Visibility: **protected**
* Source: [classes/order/OrderMessage.php line 54](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.9/classes/order/OrderMessage.php#L54).


Methods
-------


### <a name="method-getOrderMessages"></a>getOrderMessages

```php
mixed OrderMessageCore::getOrderMessages($id_lang)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/order/OrderMessage.php line 61](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.9/classes/order/OrderMessage.php#L61)


#### Arguments
* $id_lang **mixed**

