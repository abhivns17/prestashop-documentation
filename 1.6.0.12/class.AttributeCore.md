Class AttributeCore
=====================





* Class name: AttributeCore
* Parent class: [ObjectModel](class.ObjectModelCore.md)
* Source: [classes/Attribute.php line 27](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/Attribute.php#L27)


Contents
--------


### Properties

* [$color](#property-$color)
* [$default](#property-$default)
* [$definition](#property-$definition)
* [$id_attribute_group](#property-$id_attribute_group)
* [$image_dir](#property-$image_dir)
* [$name](#property-$name)
* [$position](#property-$position)
* [$webserviceParameters](#property-$webserviceParameters)
* [$cache_objects](#property-$cache_objects)
* [$db](#property-$db)
* [$def](#property-$def)
* [$fieldsRequired](#property-$fieldsRequired)
* [$fieldsRequiredDatabase](#property-$fieldsRequiredDatabase)
* [$fieldsRequiredLang](#property-$fieldsRequiredLang)
* [$fieldsSize](#property-$fieldsSize)
* [$fieldsSizeLang](#property-$fieldsSizeLang)
* [$fieldsValidate](#property-$fieldsValidate)
* [$fieldsValidateLang](#property-$fieldsValidateLang)
* [$force_id](#property-$force_id)
* [$get_shop_from_context](#property-$get_shop_from_context)
* [$id](#property-$id)
* [$id_lang](#property-$id_lang)
* [$id_shop](#property-$id_shop)
* [$id_shop_list](#property-$id_shop_list)
* [$identifier](#property-$identifier)
* [$image_format](#property-$image_format)
* [$loaded_classes](#property-$loaded_classes)
* [$table](#property-$table)
* [$tables](#property-$tables)
* [$update_fields](#property-$update_fields)

### Methods

* [__construct](#method-__construct)
* [add](#method-add)
* [addFieldsRequiredDatabase](#method-addFieldsRequiredDatabase)
* [associateTo](#method-associateTo)
* [cacheFieldsRequiredDatabase](#method-cacheFieldsRequiredDatabase)
* [checkAttributeQty](#method-checkAttributeQty)
* [cleanPositions](#method-cleanPositions)
* [clearCache](#method-clearCache)
* [delete](#method-delete)
* [deleteImage](#method-deleteImage)
* [deleteSelection](#method-deleteSelection)
* [disableCache](#method-disableCache)
* [displayFieldName](#method-displayFieldName)
* [duplicateObject](#method-duplicateObject)
* [duplicateShops](#method-duplicateShops)
* [enableCache](#method-enableCache)
* [existsInDatabase](#method-existsInDatabase)
* [formatFields](#method-formatFields)
* [formatValue](#method-formatValue)
* [getAssociatedShops](#method-getAssociatedShops)
* [getAttributeMinimalQty](#method-getAttributeMinimalQty)
* [getAttributeQty](#method-getAttributeQty)
* [getAttributes](#method-getAttributes)
* [getDefinition](#method-getDefinition)
* [getFieldByLang](#method-getFieldByLang)
* [getFields](#method-getFields)
* [getFieldsLang](#method-getFieldsLang)
* [getFieldsRequiredDatabase](#method-getFieldsRequiredDatabase)
* [getFieldsShop](#method-getFieldsShop)
* [getHigherPosition](#method-getHigherPosition)
* [getTranslationsFields](#method-getTranslationsFields)
* [getValidationRules](#method-getValidationRules)
* [getWebserviceObjectList](#method-getWebserviceObjectList)
* [getWebserviceParameters](#method-getWebserviceParameters)
* [hasMultishopEntries](#method-hasMultishopEntries)
* [hydrate](#method-hydrate)
* [hydrateCollection](#method-hydrateCollection)
* [isAssociatedToShop](#method-isAssociatedToShop)
* [isAttribute](#method-isAttribute)
* [isColorAttribute](#method-isColorAttribute)
* [isCurrentlyUsed](#method-isCurrentlyUsed)
* [isLangMultishop](#method-isLangMultishop)
* [isMultiShopField](#method-isMultiShopField)
* [isMultishop](#method-isMultishop)
* [makeTranslationFields](#method-makeTranslationFields)
* [save](#method-save)
* [setDefinitionRetrocompatibility](#method-setDefinitionRetrocompatibility)
* [setFieldsToUpdate](#method-setFieldsToUpdate)
* [toggleStatus](#method-toggleStatus)
* [update](#method-update)
* [updateMultishopTable](#method-updateMultishopTable)
* [updatePosition](#method-updatePosition)
* [updateQtyProduct](#method-updateQtyProduct)
* [validateControler](#method-validateControler)
* [validateController](#method-validateController)
* [validateField](#method-validateField)
* [validateFields](#method-validateFields)
* [validateFieldsLang](#method-validateFieldsLang)
* [validateFieldsRequiredDatabase](#method-validateFieldsRequiredDatabase)




Properties
----------


### <a name="property-$color"></a>$color

```php
public mixed $color
```





* Visibility: **public**
* Source: [classes/Attribute.php line 34](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/Attribute.php#L34).


### <a name="property-$default"></a>$default

```php
public mixed $default
```





* Visibility: **public**
* Source: [classes/Attribute.php line 36](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/Attribute.php#L36).


### <a name="property-$definition"></a>$definition

```php
public mixed $definition = array('table' => 'attribute', 'primary' => 'id_attribute', 'multilang' => true, 'fields' => array('id_attribute_group' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'color' => array('type' => self::TYPE_STRING, 'validate' => 'isColor'), 'position' => array('type' => self::TYPE_INT, 'validate' => 'isInt'), 'name' => array('type' => self::TYPE_STRING, 'lang' => true, 'validate' => 'isGenericName', 'required' => true, 'size' => 128)))
```





* Visibility: **public**
* This property is **static**.
* Source: [classes/Attribute.php line 41](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/Attribute.php#L41).


### <a name="property-$id_attribute_group"></a>$id_attribute_group

```php
public integer $id_attribute_group
```





* Visibility: **public**
* Source: [classes/Attribute.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/Attribute.php#L30).


### <a name="property-$image_dir"></a>$image_dir

```php
protected mixed $image_dir = _PS_COL_IMG_DIR_
```





* Visibility: **protected**
* Source: [classes/Attribute.php line 56](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/Attribute.php#L56).


### <a name="property-$name"></a>$name

```php
public string $name
```





* Visibility: **public**
* Source: [classes/Attribute.php line 33](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/Attribute.php#L33).


### <a name="property-$position"></a>$position

```php
public mixed $position
```





* Visibility: **public**
* Source: [classes/Attribute.php line 35](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/Attribute.php#L35).


### <a name="property-$webserviceParameters"></a>$webserviceParameters

```php
protected mixed $webserviceParameters = array('objectsNodeName' => 'product_option_values', 'objectNodeName' => 'product_option_value', 'fields' => array('id_attribute_group' => array('xlink_resource' => 'product_options')))
```





* Visibility: **protected**
* Source: [classes/Attribute.php line 58](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/Attribute.php#L58).


### <a name="property-$cache_objects"></a>$cache_objects

```php
protected boolean $cache_objects = true
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 153](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L153).


### <a name="property-$db"></a>$db

```php
protected \Db $db = false
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 143](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L143).


### <a name="property-$def"></a>$def

```php
protected array $def
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 133](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L133).


### <a name="property-$fieldsRequired"></a>$fieldsRequired

```php
protected mixed $fieldsRequired = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 81](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L81).


### <a name="property-$fieldsRequiredDatabase"></a>$fieldsRequiredDatabase

```php
protected mixed $fieldsRequiredDatabase = null
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 66](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L66).


### <a name="property-$fieldsRequiredLang"></a>$fieldsRequiredLang

```php
protected mixed $fieldsRequiredLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 96](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L96).


### <a name="property-$fieldsSize"></a>$fieldsSize

```php
protected mixed $fieldsSize = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 86](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L86).


### <a name="property-$fieldsSizeLang"></a>$fieldsSizeLang

```php
protected mixed $fieldsSizeLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 101](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L101).


### <a name="property-$fieldsValidate"></a>$fieldsValidate

```php
protected mixed $fieldsValidate = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 91](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L91).


### <a name="property-$fieldsValidateLang"></a>$fieldsValidateLang

```php
protected mixed $fieldsValidateLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 106](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L106).


### <a name="property-$force_id"></a>$force_id

```php
public \boolean, $force_id = false
```





* Visibility: **public**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 148](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L148).


### <a name="property-$get_shop_from_context"></a>$get_shop_from_context

```php
protected mixed $get_shop_from_context = true
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 64](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L64).


### <a name="property-$id"></a>$id

```php
public integer $id
```





* Visibility: **public**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 55](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L55).


### <a name="property-$id_lang"></a>$id_lang

```php
protected integer $id_lang = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 58](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L58).


### <a name="property-$id_shop"></a>$id_shop

```php
protected mixed $id_shop = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 60](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L60).


### <a name="property-$id_shop_list"></a>$id_shop_list

```php
public mixed $id_shop_list = null
```





* Visibility: **public**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 62](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L62).


### <a name="property-$identifier"></a>$identifier

```php
protected mixed $identifier
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 76](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L76).


### <a name="property-$image_format"></a>$image_format

```php
protected string $image_format = 'jpg'
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 120](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L120).


### <a name="property-$loaded_classes"></a>$loaded_classes

```php
protected mixed $loaded_classes = array()
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 128](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L128).


### <a name="property-$table"></a>$table

```php
protected mixed $table
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 71](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L71).


### <a name="property-$tables"></a>$tables

```php
protected mixed $tables = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 111](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L111).


### <a name="property-$update_fields"></a>$update_fields

```php
protected array $update_fields = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 138](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L138).


Methods
-------


### <a name="method-__construct"></a>__construct

```php
mixed AttributeCore::__construct($id, $id_lang, $id_shop)
```





* Visibility: **public**
* Source: [classes/Attribute.php line 66](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/Attribute.php#L66)


#### Arguments
* $id **mixed**
* $id_lang **mixed**
* $id_shop **mixed**



### <a name="method-add"></a>add

```php
mixed AttributeCore::add($autodate, $null_values)
```





* Visibility: **public**
* Source: [classes/Attribute.php line 124](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/Attribute.php#L124)


#### Arguments
* $autodate **mixed**
* $null_values **mixed**



### <a name="method-addFieldsRequiredDatabase"></a>addFieldsRequiredDatabase

```php
mixed ObjectModelCore::addFieldsRequiredDatabase($fields)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1244](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1244)


#### Arguments
* $fields **mixed**



### <a name="method-associateTo"></a>associateTo

```php
boolean ObjectModelCore::associateTo(integer|array $id_shops)
```

This function associate an item to its context



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1302](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1302)


#### Arguments
* $id_shops **integer|array**



### <a name="method-cacheFieldsRequiredDatabase"></a>cacheFieldsRequiredDatabase

```php
mixed ObjectModelCore::cacheFieldsRequiredDatabase($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1231](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1231)


#### Arguments
* $all **mixed**



### <a name="method-checkAttributeQty"></a>checkAttributeQty

```php
boolean AttributeCore::checkAttributeQty(integer $id_product_attribute, integer $qty, \Shop $shop)
```

Get quantity for a given attribute combination
Check if quantity is enough to deserve customer



* Visibility: **public**
* This method is **static**.
* Source: [classes/Attribute.php line 196](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/Attribute.php#L196)


#### Arguments
* $id_product_attribute **integer** - Product attribute combination id
* $qty **integer** - Quantity needed
* $shop **[Shop](class.ShopCore.md)**



### <a name="method-cleanPositions"></a>cleanPositions

```php
boolean AttributeCore::cleanPositions(integer $id_attribute_group, boolean $use_last_attribute)
```

Reorder attribute position in group $id_attribute_group.

Call it after deleting an attribute from a group.

* Visibility: **public**
* Source: [classes/Attribute.php line 340](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/Attribute.php#L340)


#### Arguments
* $id_attribute_group **integer**
* $use_last_attribute **boolean**



### <a name="method-clearCache"></a>clearCache

```php
mixed ObjectModelCore::clearCache($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1258](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1258)


#### Arguments
* $all **mixed**



### <a name="method-delete"></a>delete

```php
mixed AttributeCore::delete()
```





* Visibility: **public**
* Source: [classes/Attribute.php line 73](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/Attribute.php#L73)




### <a name="method-deleteImage"></a>deleteImage

```php
boolean ObjectModelCore::deleteImage($force_delete)
```

Delete images associated with the object



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1433](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1433)


#### Arguments
* $force_delete **mixed**



### <a name="method-deleteSelection"></a>deleteSelection

```php
boolean ObjectModelCore::deleteSelection(array $selection)
```

Delete several objects from database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 769](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L769)


#### Arguments
* $selection **array**



### <a name="method-disableCache"></a>disableCache

```php
mixed ObjectModelCore::disableCache()
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1719](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1719)




### <a name="method-displayFieldName"></a>displayFieldName

```php
mixed ObjectModelCore::displayFieldName($field, $class, $htmlentities, \Context $context)
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1014](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1014)


#### Arguments
* $field **mixed**
* $class **mixed**
* $htmlentities **mixed**
* $context **[Context](class.ContextCore.md)**



### <a name="method-duplicateObject"></a>duplicateObject

```php
\new ObjectModelCore::duplicateObject()
```

Duplicate current object to database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 549](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L549)




### <a name="method-duplicateShops"></a>duplicateShops

```php
mixed ObjectModelCore::duplicateShops($id)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1346](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1346)


#### Arguments
* $id **mixed**



### <a name="method-enableCache"></a>enableCache

```php
mixed ObjectModelCore::enableCache()
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1714](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1714)




### <a name="method-existsInDatabase"></a>existsInDatabase

```php
boolean ObjectModelCore::existsInDatabase(integer $id_entity, string $table)
```

Specify if an ObjectModel is already in database



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1470](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1470)


#### Arguments
* $id_entity **integer**
* $table **string**



### <a name="method-formatFields"></a>formatFields

```php
array ObjectModelCore::formatFields(integer $type, integer $id_lang)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 348](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L348)


#### Arguments
* $type **integer** - FORMAT_COMMON or FORMAT_LANG or FORMAT_SHOP
* $id_lang **integer** - If this parameter is given, only take lang fields



### <a name="method-formatValue"></a>formatValue

```php
mixed ObjectModelCore::formatValue(mixed $value, integer $type, $with_quotes, $purify)
```

Format a data



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 395](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L395)


#### Arguments
* $value **mixed**
* $type **integer**
* $with_quotes **mixed**
* $purify **mixed**



### <a name="method-getAssociatedShops"></a>getAssociatedShops

```php
array ObjectModelCore::getAssociatedShops()
```

Get the list of associated id_shop



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1331](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1331)




### <a name="method-getAttributeMinimalQty"></a>getAttributeMinimalQty

```php
mixed AttributeCore::getAttributeMinimalQty(integer $id_product_attribute)
```

Get minimal quantity for product with attributes quantity



* Visibility: **public**
* This method is **static**.
* Source: [classes/Attribute.php line 267](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/Attribute.php#L267)


#### Arguments
* $id_product_attribute **integer**



### <a name="method-getAttributeQty"></a>getAttributeQty

```php
mixed AttributeCore::getAttributeQty($id_product)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Attribute.php line 209](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/Attribute.php#L209)


#### Arguments
* $id_product **mixed**



### <a name="method-getAttributes"></a>getAttributes

```php
array AttributeCore::getAttributes(integer $id_lang, $not_null)
```

Get all attributes for a given language



* Visibility: **public**
* This method is **static**.
* Source: [classes/Attribute.php line 144](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/Attribute.php#L144)


#### Arguments
* $id_lang **integer** - Language id
* $not_null **mixed**



### <a name="method-getDefinition"></a>getDefinition

```php
array ObjectModelCore::getDefinition(string $class, string $field)
```

Get object definition



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1576](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1576)


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
* Source: [classes/ObjectModel.php line 1683](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1683)


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
* Source: [classes/ObjectModel.php line 276](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L276)




### <a name="method-getFieldsLang"></a>getFieldsLang

```php
array ObjectModelCore::getFieldsLang()
```

Prepare multilang fields



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 313](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L313)




### <a name="method-getFieldsRequiredDatabase"></a>getFieldsRequiredDatabase

```php
mixed ObjectModelCore::getFieldsRequiredDatabase($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1223](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1223)


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
* Source: [classes/ObjectModel.php line 299](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L299)




### <a name="method-getHigherPosition"></a>getHigherPosition

```php
integer AttributeCore::getHigherPosition(integer $id_attribute_group)
```

getHigherPosition

Get the higher attribute position from a group attribute

* Visibility: **public**
* This method is **static**.
* Source: [classes/Attribute.php line 360](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/Attribute.php#L360)


#### Arguments
* $id_attribute_group **integer**



### <a name="method-getTranslationsFields"></a>getTranslationsFields

```php
mixed ObjectModelCore::getTranslationsFields($fields_array)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 804](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L804)


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
* Source: [classes/ObjectModel.php line 161](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L161)


#### Arguments
* $class **string** - Child class name for static use (optional)



### <a name="method-getWebserviceObjectList"></a>getWebserviceObjectList

```php
mixed ObjectModelCore::getWebserviceObjectList($sql_join, $sql_filter, $sql_sort, $sql_limit)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1164](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1164)


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
* Source: [classes/ObjectModel.php line 1086](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1086)


#### Arguments
* $ws_params_attribute_name **mixed**



### <a name="method-hasMultishopEntries"></a>hasMultishopEntries

```php
boolean ObjectModelCore::hasMultishopEntries()
```

Check if there is more than one entries in associated shop table for current entity



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1371](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1371)




### <a name="method-hydrate"></a>hydrate

```php
mixed ObjectModelCore::hydrate(array $data, integer $id_lang)
```

Fill an object with given data. Data must be an array with this syntax: array(objProperty => value, objProperty2 => value, etc.)



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1508](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1508)


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
* Source: [classes/ObjectModel.php line 1527](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1527)


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
* Source: [classes/ObjectModel.php line 1273](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1273)


#### Arguments
* $id_shop **integer**



### <a name="method-isAttribute"></a>isAttribute

```php
mixed AttributeCore::isAttribute($id_attribute_group, $name, $id_lang)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Attribute.php line 165](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/Attribute.php#L165)


#### Arguments
* $id_attribute_group **mixed**
* $name **mixed**
* $id_lang **mixed**



### <a name="method-isColorAttribute"></a>isColorAttribute

```php
boolean AttributeCore::isColorAttribute()
```

Return true if attribute is color type



* Visibility: **public**
* Source: [classes/Attribute.php line 245](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/Attribute.php#L245)




### <a name="method-isCurrentlyUsed"></a>isCurrentlyUsed

```php
boolean ObjectModelCore::isCurrentlyUsed(string $table, boolean $has_active_column)
```

This method is allow to know if a entity is currently used



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1488](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1488)


#### Arguments
* $table **string** - name of table linked to entity
* $has_active_column **boolean** - true if the table has an active column



### <a name="method-isLangMultishop"></a>isLangMultishop

```php
mixed ObjectModelCore::isLangMultishop()
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1388](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1388)




### <a name="method-isMultiShopField"></a>isMultiShopField

```php
mixed ObjectModelCore::isMultiShopField($field)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1383](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1383)


#### Arguments
* $field **mixed**



### <a name="method-isMultishop"></a>isMultishop

```php
mixed ObjectModelCore::isMultishop()
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1378](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1378)




### <a name="method-makeTranslationFields"></a>makeTranslationFields

```php
mixed ObjectModelCore::makeTranslationFields($fields, $fields_array, $id_language)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 820](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L820)


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
* Source: [classes/ObjectModel.php line 446](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L446)


#### Arguments
* $null_values **boolean**
* $autodate **boolean**



### <a name="method-setDefinitionRetrocompatibility"></a>setDefinitionRetrocompatibility

```php
mixed ObjectModelCore::setDefinitionRetrocompatibility()
```

Retrocompatibility for classes without $definition static
Remove this in 1.6 !



* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1614](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1614)




### <a name="method-setFieldsToUpdate"></a>setFieldsToUpdate

```php
mixed ObjectModelCore::setFieldsToUpdate(array $fields)
```

Set a list of specific fields to update
array(field1 => true, field2 => false, langfield1 => array(1 => true, 2 => false))



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1709](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1709)


#### Arguments
* $fields **array**



### <a name="method-toggleStatus"></a>toggleStatus

```php
boolean ObjectModelCore::toggleStatus()
```

Toggle object status in database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 785](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L785)




### <a name="method-update"></a>update

```php
mixed AttributeCore::update($null_values)
```





* Visibility: **public**
* Source: [classes/Attribute.php line 114](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/Attribute.php#L114)


#### Arguments
* $null_values **mixed**



### <a name="method-updateMultishopTable"></a>updateMultishopTable

```php
boolean ObjectModelCore::updateMultishopTable(string $classname, array $data, string $where, string $specific_where)
```

Update a table and splits the common datas and the shop datas



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1403](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1403)


#### Arguments
* $classname **string**
* $data **array**
* $where **string**
* $specific_where **string** - Only executed for common table



### <a name="method-updatePosition"></a>updatePosition

```php
boolean AttributeCore::updatePosition(boolean $way, integer $position)
```

Move an attribute inside its group



* Visibility: **public**
* Source: [classes/Attribute.php line 288](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/Attribute.php#L288)


#### Arguments
* $way **boolean** - Up (1)  or Down (0)
* $position **integer**



### <a name="method-updateQtyProduct"></a>updateQtyProduct

```php
boolean AttributeCore::updateQtyProduct($arr)
```

Update array with veritable quantity



* Visibility: **public**
* This method is **static**.
* Source: [classes/Attribute.php line 223](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/Attribute.php#L223)


#### Arguments
* $arr **mixed**



### <a name="method-validateControler"></a>validateControler

```php
mixed ObjectModelCore::validateControler($htmlentities)
```

TODO: refactor rename all calls to this to validateController



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1032](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1032)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateController"></a>validateController

```php
mixed ObjectModelCore::validateController($htmlentities)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1038](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1038)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateField"></a>validateField

```php
boolean|string ObjectModelCore::validateField(string $field, mixed $value, integer $id_lang, $skip, $human_errors)
```

Validate a single field



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 931](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L931)


#### Arguments
* $field **string** - Field name
* $value **mixed** - Field value
* $id_lang **integer**
* $skip **mixed**
* $human_errors **mixed**



### <a name="method-validateFields"></a>validateFields

```php
boolean|string ObjectModelCore::validateFields(boolean $die, boolean $error_return)
```

Check for fields validity before database interaction



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 858](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L858)


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
* Source: [classes/ObjectModel.php line 887](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L887)


#### Arguments
* $die **boolean**
* $error_return **boolean**



### <a name="method-validateFieldsRequiredDatabase"></a>validateFieldsRequiredDatabase

```php
mixed ObjectModelCore::validateFieldsRequiredDatabase($htmlentities)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1200](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.12/classes/ObjectModel.php#L1200)


#### Arguments
* $htmlentities **mixed**


