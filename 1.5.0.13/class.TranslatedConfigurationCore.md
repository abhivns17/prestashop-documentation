Class TranslatedConfigurationCore
=====================





* Class name: TranslatedConfigurationCore
* Parent class: [Configuration](class.ConfigurationCore.md)
* Source: [classes/TranslatedConfiguration.php line 28](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/TranslatedConfiguration.php#L28)


Contents
--------


### Properties

* [$definition](#property-$definition)
* [$webserviceParameters](#property-$webserviceParameters)
* [$_CONF](#property-$_CONF)
* [$date_add](#property-$date_add)
* [$date_upd](#property-$date_upd)
* [$id](#property-$id)
* [$id_shop](#property-$id_shop)
* [$id_shop_group](#property-$id_shop_group)
* [$name](#property-$name)
* [$types](#property-$types)
* [$value](#property-$value)
* [$def](#property-$def)
* [$fieldsRequired](#property-$fieldsRequired)
* [$fieldsRequiredDatabase](#property-$fieldsRequiredDatabase)
* [$fieldsRequiredLang](#property-$fieldsRequiredLang)
* [$fieldsSize](#property-$fieldsSize)
* [$fieldsSizeLang](#property-$fieldsSizeLang)
* [$fieldsValidate](#property-$fieldsValidate)
* [$fieldsValidateLang](#property-$fieldsValidateLang)
* [$get_shop_from_context](#property-$get_shop_from_context)
* [$id_lang](#property-$id_lang)
* [$id_shop_list](#property-$id_shop_list)
* [$identifier](#property-$identifier)
* [$image_dir](#property-$image_dir)
* [$image_format](#property-$image_format)
* [$table](#property-$table)
* [$tables](#property-$tables)
* [$update_fields](#property-$update_fields)

### Methods

* [__construct](#method-__construct)
* [add](#method-add)
* [addFieldsRequiredDatabase](#method-addFieldsRequiredDatabase)
* [associateTo](#method-associateTo)
* [clearCache](#method-clearCache)
* [delete](#method-delete)
* [deleteByName](#method-deleteByName)
* [deleteFromContext](#method-deleteFromContext)
* [deleteImage](#method-deleteImage)
* [deleteSelection](#method-deleteSelection)
* [displayFieldName](#method-displayFieldName)
* [duplicateShops](#method-duplicateShops)
* [existsInDatabase](#method-existsInDatabase)
* [formatFields](#method-formatFields)
* [formatValue](#method-formatValue)
* [get](#method-get)
* [getAssociatedShops](#method-getAssociatedShops)
* [getDefinition](#method-getDefinition)
* [getFieldByLang](#method-getFieldByLang)
* [getFields](#method-getFields)
* [getFieldsLang](#method-getFieldsLang)
* [getFieldsRequiredDatabase](#method-getFieldsRequiredDatabase)
* [getFieldsShop](#method-getFieldsShop)
* [getGlobalValue](#method-getGlobalValue)
* [getIdByName](#method-getIdByName)
* [getInt](#method-getInt)
* [getMultiple](#method-getMultiple)
* [getTranslationsFields](#method-getTranslationsFields)
* [getValidationRules](#method-getValidationRules)
* [getWebserviceObjectList](#method-getWebserviceObjectList)
* [getWebserviceParameters](#method-getWebserviceParameters)
* [hasContext](#method-hasContext)
* [hasKey](#method-hasKey)
* [hasMultishopEntries](#method-hasMultishopEntries)
* [hydrate](#method-hydrate)
* [hydrateCollection](#method-hydrateCollection)
* [isAssociatedToShop](#method-isAssociatedToShop)
* [isCurrentlyUsed](#method-isCurrentlyUsed)
* [isLangKey](#method-isLangKey)
* [isLangMultishop](#method-isLangMultishop)
* [isMultishop](#method-isMultishop)
* [isOverridenByCurrentContext](#method-isOverridenByCurrentContext)
* [loadConfiguration](#method-loadConfiguration)
* [makeTranslationFields](#method-makeTranslationFields)
* [save](#method-save)
* [set](#method-set)
* [setDefinitionRetrocompatibility](#method-setDefinitionRetrocompatibility)
* [setFieldsToUpdate](#method-setFieldsToUpdate)
* [sqlRestriction](#method-sqlRestriction)
* [toggleStatus](#method-toggleStatus)
* [update](#method-update)
* [updateGlobalValue](#method-updateGlobalValue)
* [updateMultishopTable](#method-updateMultishopTable)
* [updateValue](#method-updateValue)
* [validateControler](#method-validateControler)
* [validateController](#method-validateController)
* [validateField](#method-validateField)
* [validateFields](#method-validateFields)
* [validateFieldsLang](#method-validateFieldsLang)




Properties
----------


### <a name="property-$definition"></a>$definition

```php
public mixed $definition = array('table' => 'configuration', 'primary' => 'id_configuration', 'multilang' => true, 'fields' => array('name' => array('type' => self::TYPE_STRING, 'validate' => 'isConfigName', 'required' => true, 'size' => 32), 'id_shop_group' => array('type' => self::TYPE_NOTHING, 'validate' => 'isUnsignedId'), 'id_shop' => array('type' => self::TYPE_NOTHING, 'validate' => 'isUnsignedId'), 'value' => array('type' => self::TYPE_STRING, 'lang' => true), 'date_add' => array('type' => self::TYPE_DATE, 'validate' => 'isDate'), 'date_upd' => array('type' => self::TYPE_DATE, 'validate' => 'isDate')))
```





* Visibility: **public**
* This property is **static**.
* Source: [classes/TranslatedConfiguration.php line 40](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/TranslatedConfiguration.php#L40).


### <a name="property-$webserviceParameters"></a>$webserviceParameters

```php
protected mixed $webserviceParameters = array('objectNodeName' => 'translated_configuration', 'objectsNodeName' => 'translated_configurations', 'fields' => array('value' => array(), 'date_add' => array(), 'date_upd' => array()))
```





* Visibility: **protected**
* Source: [classes/TranslatedConfiguration.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/TranslatedConfiguration.php#L30).


### <a name="property-$_CONF"></a>$_CONF

```php
protected array $_CONF
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ConfigurationCore](class.ConfigurationCore.md).
* Source: [classes/Configuration.php line 65](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/Configuration.php#L65).


### <a name="property-$date_add"></a>$date_add

```php
public string $date_add
```





* Visibility: **public**
* This property is defined by [ConfigurationCore](class.ConfigurationCore.md).
* Source: [classes/Configuration.php line 42](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/Configuration.php#L42).


### <a name="property-$date_upd"></a>$date_upd

```php
public string $date_upd
```





* Visibility: **public**
* This property is defined by [ConfigurationCore](class.ConfigurationCore.md).
* Source: [classes/Configuration.php line 45](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/Configuration.php#L45).


### <a name="property-$id"></a>$id

```php
public mixed $id
```





* Visibility: **public**
* This property is defined by [ConfigurationCore](class.ConfigurationCore.md).
* Source: [classes/Configuration.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/Configuration.php#L30).


### <a name="property-$id_shop"></a>$id_shop

```php
public mixed $id_shop
```





* Visibility: **public**
* This property is defined by [ConfigurationCore](class.ConfigurationCore.md).
* Source: [classes/Configuration.php line 36](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/Configuration.php#L36).


### <a name="property-$id_shop_group"></a>$id_shop_group

```php
public mixed $id_shop_group
```





* Visibility: **public**
* This property is defined by [ConfigurationCore](class.ConfigurationCore.md).
* Source: [classes/Configuration.php line 35](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/Configuration.php#L35).


### <a name="property-$name"></a>$name

```php
public string $name
```





* Visibility: **public**
* This property is defined by [ConfigurationCore](class.ConfigurationCore.md).
* Source: [classes/Configuration.php line 33](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/Configuration.php#L33).


### <a name="property-$types"></a>$types

```php
protected array $types = array()
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ConfigurationCore](class.ConfigurationCore.md).
* Source: [classes/Configuration.php line 68](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/Configuration.php#L68).


### <a name="property-$value"></a>$value

```php
public string $value
```





* Visibility: **public**
* This property is defined by [ConfigurationCore](class.ConfigurationCore.md).
* Source: [classes/Configuration.php line 39](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/Configuration.php#L39).


### <a name="property-$def"></a>$def

```php
protected array $def
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 131](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L131).


### <a name="property-$fieldsRequired"></a>$fieldsRequired

```php
protected mixed $fieldsRequired = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 81](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L81).


### <a name="property-$fieldsRequiredDatabase"></a>$fieldsRequiredDatabase

```php
protected mixed $fieldsRequiredDatabase = null
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 66](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L66).


### <a name="property-$fieldsRequiredLang"></a>$fieldsRequiredLang

```php
protected mixed $fieldsRequiredLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 96](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L96).


### <a name="property-$fieldsSize"></a>$fieldsSize

```php
protected mixed $fieldsSize = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 86](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L86).


### <a name="property-$fieldsSizeLang"></a>$fieldsSizeLang

```php
protected mixed $fieldsSizeLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 101](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L101).


### <a name="property-$fieldsValidate"></a>$fieldsValidate

```php
protected mixed $fieldsValidate = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 91](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L91).


### <a name="property-$fieldsValidateLang"></a>$fieldsValidateLang

```php
protected mixed $fieldsValidateLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 106](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L106).


### <a name="property-$get_shop_from_context"></a>$get_shop_from_context

```php
protected mixed $get_shop_from_context = true
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 64](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L64).


### <a name="property-$id_lang"></a>$id_lang

```php
protected integer $id_lang = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 58](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L58).


### <a name="property-$id_shop_list"></a>$id_shop_list

```php
public mixed $id_shop_list = null
```





* Visibility: **public**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 62](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L62).


### <a name="property-$identifier"></a>$identifier

```php
protected mixed $identifier
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 76](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L76).


### <a name="property-$image_dir"></a>$image_dir

```php
protected string $image_dir = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 117](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L117).


### <a name="property-$image_format"></a>$image_format

```php
protected string $image_format = 'jpg'
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 120](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L120).


### <a name="property-$table"></a>$table

```php
protected mixed $table
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 71](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L71).


### <a name="property-$tables"></a>$tables

```php
protected mixed $tables = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 111](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L111).


### <a name="property-$update_fields"></a>$update_fields

```php
protected array $update_fields = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 136](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L136).


Methods
-------


### <a name="method-__construct"></a>__construct

```php
mixed TranslatedConfigurationCore::__construct($id, $id_lang)
```





* Visibility: **public**
* Source: [classes/TranslatedConfiguration.php line 54](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/TranslatedConfiguration.php#L54)


#### Arguments
* $id **mixed**
* $id_lang **mixed**



### <a name="method-add"></a>add

```php
mixed TranslatedConfigurationCore::add($autodate, $nullValues)
```





* Visibility: **public**
* Source: [classes/TranslatedConfiguration.php line 73](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/TranslatedConfiguration.php#L73)


#### Arguments
* $autodate **mixed**
* $nullValues **mixed**



### <a name="method-addFieldsRequiredDatabase"></a>addFieldsRequiredDatabase

```php
mixed ObjectModelCore::addFieldsRequiredDatabase($fields)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1040](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L1040)


#### Arguments
* $fields **mixed**



### <a name="method-associateTo"></a>associateTo

```php
boolean ObjectModelCore::associateTo(integer|array $id_shops)
```

This function associate an item to its context



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1087](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L1087)


#### Arguments
* $id_shops **integer|array**



### <a name="method-clearCache"></a>clearCache

```php
mixed ObjectModelCore::clearCache($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1054](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L1054)


#### Arguments
* $all **mixed**



### <a name="method-delete"></a>delete

```php
boolean ObjectModelCore::delete()
```

Delete current object from database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 623](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L623)




### <a name="method-deleteByName"></a>deleteByName

```php
boolean ConfigurationCore::deleteByName(string $key)
```

Delete a configuration key in database (with or without language management)



* Visibility: **public**
* This method is **static**.
* This method is defined by [ConfigurationCore](class.ConfigurationCore.md).
* Source: [classes/Configuration.php line 377](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/Configuration.php#L377)


#### Arguments
* $key **string** - Key to delete



### <a name="method-deleteFromContext"></a>deleteFromContext

```php
mixed ConfigurationCore::deleteFromContext(string $key)
```

Delete configuration key from current context.



* Visibility: **public**
* This method is **static**.
* This method is defined by [ConfigurationCore](class.ConfigurationCore.md).
* Source: [classes/Configuration.php line 401](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/Configuration.php#L401)


#### Arguments
* $key **string**



### <a name="method-deleteImage"></a>deleteImage

```php
boolean ObjectModelCore::deleteImage()
```

Delete images associated with the object



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1214](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L1214)




### <a name="method-deleteSelection"></a>deleteSelection

```php
boolean ObjectModelCore::deleteSelection(array $selection)
```

Delete several objects from database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 669](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L669)


#### Arguments
* $selection **array**



### <a name="method-displayFieldName"></a>displayFieldName

```php
mixed ObjectModelCore::displayFieldName($field, $class, $htmlentities, \Context $context)
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 869](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L869)


#### Arguments
* $field **mixed**
* $class **mixed**
* $htmlentities **mixed**
* $context **[Context](class.ContextCore.md)**



### <a name="method-duplicateShops"></a>duplicateShops

```php
mixed ObjectModelCore::duplicateShops($id)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1131](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L1131)


#### Arguments
* $id **mixed**



### <a name="method-existsInDatabase"></a>existsInDatabase

```php
boolean ObjectModelCore::existsInDatabase(integer $id_entity, string $table)
```

Specify if an ObjectModel is already in database



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1248](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L1248)


#### Arguments
* $id_entity **integer**
* $table **string**



### <a name="method-formatFields"></a>formatFields

```php
array ObjectModelCore::formatFields(integer $type, integer $id_lang)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 327](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L327)


#### Arguments
* $type **integer** - FORMAT_COMMON or FORMAT_LANG or FORMAT_SHOP
* $id_lang **integer** - If this parameter is given, only take lang fields



### <a name="method-formatValue"></a>formatValue

```php
mixed ObjectModelCore::formatValue(mixed $value, integer $type, $with_quotes)
```

Format a data



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 373](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L373)


#### Arguments
* $value **mixed**
* $type **integer**
* $with_quotes **mixed**



### <a name="method-get"></a>get

```php
string ConfigurationCore::get(string $key, integer $id_lang, $id_shop_group, $id_shop)
```

Get a single configuration value (in one language only)



* Visibility: **public**
* This method is **static**.
* This method is defined by [ConfigurationCore](class.ConfigurationCore.md).
* Source: [classes/Configuration.php line 147](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/Configuration.php#L147)


#### Arguments
* $key **string** - Key wanted
* $id_lang **integer** - Language ID
* $id_shop_group **mixed**
* $id_shop **mixed**



### <a name="method-getAssociatedShops"></a>getAssociatedShops

```php
array ObjectModelCore::getAssociatedShops()
```

Get the list of associated id_shop



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1116](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L1116)




### <a name="method-getDefinition"></a>getDefinition

```php
array ObjectModelCore::getDefinition(string $class, string $field)
```

Get object definition



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1351](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L1351)


#### Arguments
* $class **string** - Name of object
* $field **string** - Name of field if we want the definition of one field only



### <a name="method-getFieldByLang"></a>getFieldByLang

```php
mixed ObjectModelCore::getFieldByLang($field_name, null $id_lang)
```

Return the field value for the specified language if the field is multilang, else the field value.



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1428](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L1428)


#### Arguments
* $field_name **mixed**
* $id_lang **null**



### <a name="method-getFields"></a>getFields

```php
array ObjectModelCore::getFields()
```

Prepare fields for ObjectModel class (add, update)
All fields are verified (pSQL, intval.

..)

* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 255](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L255)




### <a name="method-getFieldsLang"></a>getFieldsLang

```php
array ConfigurationCore::getFieldsLang()
```





* Visibility: **public**
* This method is defined by [ConfigurationCore](class.ConfigurationCore.md).
* Source: [classes/Configuration.php line 80](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/Configuration.php#L80)




### <a name="method-getFieldsRequiredDatabase"></a>getFieldsRequiredDatabase

```php
mixed ObjectModelCore::getFieldsRequiredDatabase($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1032](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L1032)


#### Arguments
* $all **mixed**



### <a name="method-getFieldsShop"></a>getFieldsShop

```php
array ObjectModelCore::getFieldsShop()
```

Prepare fields for multishop
Fields are not validated here, we considere they are already validated in getFields() method, this
not the best solution but this is the only one possible for retro compatibility.



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 278](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L278)




### <a name="method-getGlobalValue"></a>getGlobalValue

```php
mixed ConfigurationCore::getGlobalValue($key, $id_lang)
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ConfigurationCore](class.ConfigurationCore.md).
* Source: [classes/Configuration.php line 171](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/Configuration.php#L171)


#### Arguments
* $key **mixed**
* $id_lang **mixed**



### <a name="method-getIdByName"></a>getIdByName

```php
mixed ConfigurationCore::getIdByName(string $key, integer $id_shop_group, integer $id_shop)
```

Return ID a configuration key



* Visibility: **public**
* This method is **static**.
* This method is defined by [ConfigurationCore](class.ConfigurationCore.md).
* Source: [classes/Configuration.php line 94](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/Configuration.php#L94)


#### Arguments
* $key **string**
* $id_shop_group **integer**
* $id_shop **integer**



### <a name="method-getInt"></a>getInt

```php
array ConfigurationCore::getInt(string $key, integer $id_shop_group, integer $id_shop)
```

Get a single configuration value (in multiple languages)



* Visibility: **public**
* This method is **static**.
* This method is defined by [ConfigurationCore](class.ConfigurationCore.md).
* Source: [classes/Configuration.php line 184](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/Configuration.php#L184)


#### Arguments
* $key **string** - Key wanted
* $id_shop_group **integer**
* $id_shop **integer**



### <a name="method-getMultiple"></a>getMultiple

```php
array ConfigurationCore::getMultiple(array $keys, integer $id_lang, $id_shop_group, $id_shop)
```

Get several configuration values (in one language only)



* Visibility: **public**
* This method is **static**.
* This method is defined by [ConfigurationCore](class.ConfigurationCore.md).
* Source: [classes/Configuration.php line 200](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/Configuration.php#L200)


#### Arguments
* $keys **array** - Keys wanted
* $id_lang **integer** - Language ID
* $id_shop_group **mixed**
* $id_shop **mixed**



### <a name="method-getTranslationsFields"></a>getTranslationsFields

```php
mixed ObjectModelCore::getTranslationsFields($fields_array)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 701](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L701)


#### Arguments
* $fields_array **mixed**



### <a name="method-getValidationRules"></a>getValidationRules

```php
array ObjectModelCore::getValidationRules(string $class)
```

Returns object validation rules (fields validity)



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 144](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L144)


#### Arguments
* $class **string** - Child class name for static use (optional)



### <a name="method-getWebserviceObjectList"></a>getWebserviceObjectList

```php
mixed TranslatedConfigurationCore::getWebserviceObjectList($sql_join, $sql_filter, $sql_sort, $sql_limit)
```





* Visibility: **public**
* Source: [classes/TranslatedConfiguration.php line 101](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/TranslatedConfiguration.php#L101)


#### Arguments
* $sql_join **mixed**
* $sql_filter **mixed**
* $sql_sort **mixed**
* $sql_limit **mixed**



### <a name="method-getWebserviceParameters"></a>getWebserviceParameters

```php
mixed ObjectModelCore::getWebserviceParameters($ws_params_attribute_name)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 931](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L931)


#### Arguments
* $ws_params_attribute_name **mixed**



### <a name="method-hasContext"></a>hasContext

```php
mixed ConfigurationCore::hasContext(string $key, integer $id_lang, integer $context)
```

Check if configuration var is defined in given context



* Visibility: **public**
* This method is **static**.
* This method is defined by [ConfigurationCore](class.ConfigurationCore.md).
* Source: [classes/Configuration.php line 436](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/Configuration.php#L436)


#### Arguments
* $key **string**
* $id_lang **integer**
* $context **integer**



### <a name="method-hasKey"></a>hasKey

```php
boolean ConfigurationCore::hasKey(string $key, integer $id_lang, integer $id_shop_group, integer $id_shop)
```

Check if key exists in configuration



* Visibility: **public**
* This method is **static**.
* This method is defined by [ConfigurationCore](class.ConfigurationCore.md).
* Source: [classes/Configuration.php line 226](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/Configuration.php#L226)


#### Arguments
* $key **string**
* $id_lang **integer**
* $id_shop_group **integer**
* $id_shop **integer**



### <a name="method-hasMultishopEntries"></a>hasMultishopEntries

```php
boolean ObjectModelCore::hasMultishopEntries()
```

Check if there is entries in associated shop table for current entity



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1156](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L1156)




### <a name="method-hydrate"></a>hydrate

```php
mixed ObjectModelCore::hydrate(array $data, integer $id_lang)
```

Fill an object with given data. Data must be an array with this syntax: array(objProperty => value, objProperty2 => value, etc.)



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1283](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L1283)


#### Arguments
* $data **array**
* $id_lang **integer**



### <a name="method-hydrateCollection"></a>hydrateCollection

```php
array ObjectModelCore::hydrateCollection(string $class, array $datas, integer $id_lang)
```

Fill (hydrate) a list of objects in order to get a collection of these objects



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1302](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L1302)


#### Arguments
* $class **string** - Class of objects to hydrate
* $datas **array** - List of data (multi-dimensional array)
* $id_lang **integer**



### <a name="method-isAssociatedToShop"></a>isAssociatedToShop

```php
boolean ObjectModelCore::isAssociatedToShop(integer $id_shop)
```

Check if current object is associated to a shop



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1069](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L1069)


#### Arguments
* $id_shop **integer**



### <a name="method-isCurrentlyUsed"></a>isCurrentlyUsed

```php
boolean ObjectModelCore::isCurrentlyUsed(string $table, boolean $has_active_column)
```

This method is allow to know if a entity is currently used



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1266](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L1266)


#### Arguments
* $table **string** - name of table linked to entity
* $has_active_column **boolean** - true if the table has an active column



### <a name="method-isLangKey"></a>isLangKey

```php
boolean ConfigurationCore::isLangKey(string $key)
```

Check if a key was loaded as multi lang



* Visibility: **public**
* This method is **static**.
* This method is defined by [ConfigurationCore](class.ConfigurationCore.md).
* Source: [classes/Configuration.php line 485](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/Configuration.php#L485)


#### Arguments
* $key **string**



### <a name="method-isLangMultishop"></a>isLangMultishop

```php
mixed ObjectModelCore::isLangMultishop()
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1169](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L1169)




### <a name="method-isMultishop"></a>isMultishop

```php
mixed ObjectModelCore::isMultishop()
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1164](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L1164)




### <a name="method-isOverridenByCurrentContext"></a>isOverridenByCurrentContext

```php
mixed ConfigurationCore::isOverridenByCurrentContext($key)
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ConfigurationCore](class.ConfigurationCore.md).
* Source: [classes/Configuration.php line 460](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/Configuration.php#L460)


#### Arguments
* $key **mixed**



### <a name="method-loadConfiguration"></a>loadConfiguration

```php
mixed ConfigurationCore::loadConfiguration()
```

Load all configuration data



* Visibility: **public**
* This method is **static**.
* This method is defined by [ConfigurationCore](class.ConfigurationCore.md).
* Source: [classes/Configuration.php line 111](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/Configuration.php#L111)




### <a name="method-makeTranslationFields"></a>makeTranslationFields

```php
mixed ObjectModelCore::makeTranslationFields($fields, $fields_array, $id_language)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 717](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L717)


#### Arguments
* $fields **mixed**
* $fields_array **mixed**
* $id_language **mixed**



### <a name="method-save"></a>save

```php
boolean ObjectModelCore::save(boolean $null_values, boolean $autodate)
```

Save current object to database (add or update)



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 417](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L417)


#### Arguments
* $null_values **boolean**
* $autodate **boolean**



### <a name="method-set"></a>set

```php
mixed ConfigurationCore::set(string $key, mixed $values, integer $id_shop_group, integer $id_shop)
```

Set TEMPORARY a single configuration value (in one language only)



* Visibility: **public**
* This method is **static**.
* This method is defined by [ConfigurationCore](class.ConfigurationCore.md).
* Source: [classes/Configuration.php line 244](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/Configuration.php#L244)


#### Arguments
* $key **string** - Key wanted
* $values **mixed** - $values is an array if the configuration is multilingual, a single string else.
* $id_shop_group **integer**
* $id_shop **integer**



### <a name="method-setDefinitionRetrocompatibility"></a>setDefinitionRetrocompatibility

```php
mixed ObjectModelCore::setDefinitionRetrocompatibility()
```

Retrocompatibility for classes without $definition static
Remove this in 1.6 !



* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1374](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L1374)




### <a name="method-setFieldsToUpdate"></a>setFieldsToUpdate

```php
mixed ObjectModelCore::setFieldsToUpdate(array $fields)
```

Set a list of specific fields to update
array(field1 => true, field2 => false, langfield1 => array(1 => true, 2 => false))



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1454](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L1454)


#### Arguments
* $fields **array**



### <a name="method-sqlRestriction"></a>sqlRestriction

```php
string ConfigurationCore::sqlRestriction(integer $id_shop_group, integer $id_shop)
```

Add SQL restriction on shops for configuration table



* Visibility: **protected**
* This method is **static**.
* This method is defined by [ConfigurationCore](class.ConfigurationCore.md).
* Source: [classes/Configuration.php line 497](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/Configuration.php#L497)


#### Arguments
* $id_shop_group **integer**
* $id_shop **integer**



### <a name="method-toggleStatus"></a>toggleStatus

```php
boolean ObjectModelCore::toggleStatus()
```

Toggle object status in database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 685](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L685)




### <a name="method-update"></a>update

```php
mixed TranslatedConfigurationCore::update($nullValues)
```





* Visibility: **public**
* Source: [classes/TranslatedConfiguration.php line 78](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/TranslatedConfiguration.php#L78)


#### Arguments
* $nullValues **mixed**



### <a name="method-updateGlobalValue"></a>updateGlobalValue

```php
boolean ConfigurationCore::updateGlobalValue(string $key, mixed $values, boolean $html)
```

Update configuration key for global context only



* Visibility: **public**
* This method is **static**.
* This method is defined by [ConfigurationCore](class.ConfigurationCore.md).
* Source: [classes/Configuration.php line 276](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/Configuration.php#L276)


#### Arguments
* $key **string**
* $values **mixed**
* $html **boolean**



### <a name="method-updateMultishopTable"></a>updateMultishopTable

```php
boolean ObjectModelCore::updateMultishopTable(string $classname, array $data, string $where, string $specific_where)
```

Update a table and splits the common datas and the shop datas



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1184](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L1184)


#### Arguments
* $classname **string**
* $data **array**
* $where **string**
* $specific_where **string** - Only executed for common table



### <a name="method-updateValue"></a>updateValue

```php
boolean ConfigurationCore::updateValue(string $key, mixed $values, boolean $html, integer $id_shop_group, integer $id_shop)
```

Update configuration key and value into database (automatically insert if key does not exist)



* Visibility: **public**
* This method is **static**.
* This method is defined by [ConfigurationCore](class.ConfigurationCore.md).
* Source: [classes/Configuration.php line 291](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/Configuration.php#L291)


#### Arguments
* $key **string** - Key
* $values **mixed** - $values is an array if the configuration is multilingual, a single string else.
* $html **boolean** - Specify if html is authorized in value
* $id_shop_group **integer**
* $id_shop **integer**



### <a name="method-validateControler"></a>validateControler

```php
mixed ObjectModelCore::validateControler($htmlentities)
```

TODO: refactor rename all calls to this to validateController



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 884](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L884)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateController"></a>validateController

```php
mixed ObjectModelCore::validateController($htmlentities)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 890](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L890)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateField"></a>validateField

```php
boolean|string ObjectModelCore::validateField(string $field, mixed $value, integer $id_lang)
```

Validate a single field



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 822](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L822)


#### Arguments
* $field **string** - Field name
* $value **mixed** - Field value
* $id_lang **integer**



### <a name="method-validateFields"></a>validateFields

```php
boolean|string ObjectModelCore::validateFields(boolean $die, boolean $error_return)
```

Check for fields validity before database interaction



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 755](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L755)


#### Arguments
* $die **boolean**
* $error_return **boolean**



### <a name="method-validateFieldsLang"></a>validateFieldsLang

```php
boolean|string ObjectModelCore::validateFieldsLang(boolean $die, boolean $error_return)
```

Check for multilingual fields validity before database interaction



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 784](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.13/classes/ObjectModel.php#L784)


#### Arguments
* $die **boolean**
* $error_return **boolean**


