Class DbMySQLiCore
=====================





* Class name: DbMySQLiCore
* Parent class: [Db](class.DbCore.md)
* Source: [classes/db/DbMySQLi.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.1/classes/db/DbMySQLi.php#L30)


Contents
--------



### Methods

* [Affected_Rows](#method-Affected_Rows)
* [Insert_ID](#method-Insert_ID)
* [_escape](#method-_escape)
* [_numRows](#method-_numRows)
* [_query](#method-_query)
* [checkCreatePrivilege](#method-checkCreatePrivilege)
* [connect](#method-connect)
* [createDatabase](#method-createDatabase)
* [disconnect](#method-disconnect)
* [getBestEngine](#method-getBestEngine)
* [getMsgError](#method-getMsgError)
* [getNumberError](#method-getNumberError)
* [getVersion](#method-getVersion)
* [hasTableWithSamePrefix](#method-hasTableWithSamePrefix)
* [nextRow](#method-nextRow)
* [set_db](#method-set_db)
* [tryToConnect](#method-tryToConnect)
* [tryUTF8](#method-tryUTF8)






Methods
-------


### <a name="method-Affected_Rows"></a>Affected_Rows

```php
mixed DbMySQLiCore::Affected_Rows()
```





* Visibility: **public**
* Source: [classes/db/DbMySQLi.php line 116](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.1/classes/db/DbMySQLi.php#L116)




### <a name="method-Insert_ID"></a>Insert_ID

```php
mixed DbMySQLiCore::Insert_ID()
```





* Visibility: **public**
* Source: [classes/db/DbMySQLi.php line 108](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.1/classes/db/DbMySQLi.php#L108)




### <a name="method-_escape"></a>_escape

```php
mixed DbMySQLiCore::_escape($str)
```





* Visibility: **public**
* Source: [classes/db/DbMySQLi.php line 148](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.1/classes/db/DbMySQLi.php#L148)


#### Arguments
* $str **mixed**



### <a name="method-_numRows"></a>_numRows

```php
mixed DbMySQLiCore::_numRows($result)
```





* Visibility: **protected**
* Source: [classes/db/DbMySQLi.php line 100](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.1/classes/db/DbMySQLi.php#L100)


#### Arguments
* $result **mixed**



### <a name="method-_query"></a>_query

```php
mixed DbMySQLiCore::_query($sql)
```





* Visibility: **protected**
* Source: [classes/db/DbMySQLi.php line 82](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.1/classes/db/DbMySQLi.php#L82)


#### Arguments
* $sql **mixed**



### <a name="method-checkCreatePrivilege"></a>checkCreatePrivilege

```php
mixed DbMySQLiCore::checkCreatePrivilege($server, $user, $pwd, $db, $prefix, $engine)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/db/DbMySQLi.php line 220](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.1/classes/db/DbMySQLi.php#L220)


#### Arguments
* $server **mixed**
* $user **mixed**
* $pwd **mixed**
* $db **mixed**
* $prefix **mixed**
* $engine **mixed**



### <a name="method-connect"></a>connect

```php
mixed DbMySQLiCore::connect()
```





* Visibility: **public**
* Source: [classes/db/DbMySQLi.php line 35](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.1/classes/db/DbMySQLi.php#L35)




### <a name="method-createDatabase"></a>createDatabase

```php
mixed DbMySQLiCore::createDatabase($host, $user, $password, $dbname, $dropit)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/db/DbMySQLi.php line 56](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.1/classes/db/DbMySQLi.php#L56)


#### Arguments
* $host **mixed**
* $user **mixed**
* $password **mixed**
* $dbname **mixed**
* $dropit **mixed**



### <a name="method-disconnect"></a>disconnect

```php
mixed DbMySQLiCore::disconnect()
```





* Visibility: **public**
* Source: [classes/db/DbMySQLi.php line 74](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.1/classes/db/DbMySQLi.php#L74)




### <a name="method-getBestEngine"></a>getBestEngine

```php
mixed DbMySQLiCore::getBestEngine()
```





* Visibility: **public**
* Source: [classes/db/DbMySQLi.php line 195](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.1/classes/db/DbMySQLi.php#L195)




### <a name="method-getMsgError"></a>getMsgError

```php
mixed DbMySQLiCore::getMsgError($query)
```





* Visibility: **public**
* Source: [classes/db/DbMySQLi.php line 124](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.1/classes/db/DbMySQLi.php#L124)


#### Arguments
* $query **mixed**



### <a name="method-getNumberError"></a>getNumberError

```php
mixed DbMySQLiCore::getNumberError()
```





* Visibility: **public**
* Source: [classes/db/DbMySQLi.php line 132](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.1/classes/db/DbMySQLi.php#L132)




### <a name="method-getVersion"></a>getVersion

```php
mixed DbMySQLiCore::getVersion()
```





* Visibility: **public**
* Source: [classes/db/DbMySQLi.php line 140](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.1/classes/db/DbMySQLi.php#L140)




### <a name="method-hasTableWithSamePrefix"></a>hasTableWithSamePrefix

```php
mixed DbMySQLiCore::hasTableWithSamePrefix($server, $user, $pwd, $db, $prefix)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/db/DbMySQLi.php line 164](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.1/classes/db/DbMySQLi.php#L164)


#### Arguments
* $server **mixed**
* $user **mixed**
* $pwd **mixed**
* $db **mixed**
* $prefix **mixed**



### <a name="method-nextRow"></a>nextRow

```php
mixed DbMySQLiCore::nextRow($result)
```





* Visibility: **public**
* Source: [classes/db/DbMySQLi.php line 90](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.1/classes/db/DbMySQLi.php#L90)


#### Arguments
* $result **mixed**



### <a name="method-set_db"></a>set_db

```php
mixed DbMySQLiCore::set_db($db_name)
```





* Visibility: **public**
* Source: [classes/db/DbMySQLi.php line 156](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.1/classes/db/DbMySQLi.php#L156)


#### Arguments
* $db_name **mixed**



### <a name="method-tryToConnect"></a>tryToConnect

```php
mixed DbMySQLiCore::tryToConnect($server, $user, $pwd, $db, $newDbLink, $engine, $timeout)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/db/DbMySQLi.php line 178](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.1/classes/db/DbMySQLi.php#L178)


#### Arguments
* $server **mixed**
* $user **mixed**
* $pwd **mixed**
* $db **mixed**
* $newDbLink **mixed**
* $engine **mixed**
* $timeout **mixed**



### <a name="method-tryUTF8"></a>tryUTF8

```php
mixed DbMySQLiCore::tryUTF8($server, $user, $pwd)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/db/DbMySQLi.php line 242](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.1/classes/db/DbMySQLi.php#L242)


#### Arguments
* $server **mixed**
* $user **mixed**
* $pwd **mixed**

