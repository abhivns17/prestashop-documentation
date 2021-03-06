Class SpecificPriceCore
=====================





* Class name: SpecificPriceCore
* Parent class: [ObjectModel](class.ObjectModelCore.md)
* Source: [classes/SpecificPrice.php line 28](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L28)


Contents
--------


### Properties

* [$_cache_priorities](#property-$_cache_priorities)
* [$_specificPriceCache](#property-$_specificPriceCache)
* [$definition](#property-$definition)
* [$from](#property-$from)
* [$from_quantity](#property-$from_quantity)
* [$id_cart](#property-$id_cart)
* [$id_country](#property-$id_country)
* [$id_currency](#property-$id_currency)
* [$id_customer](#property-$id_customer)
* [$id_group](#property-$id_group)
* [$id_group_shop](#property-$id_group_shop)
* [$id_product](#property-$id_product)
* [$id_product_attribute](#property-$id_product_attribute)
* [$id_shop](#property-$id_shop)
* [$id_specific_price_rule](#property-$id_specific_price_rule)
* [$price](#property-$price)
* [$reduction](#property-$reduction)
* [$reduction_type](#property-$reduction_type)
* [$to](#property-$to)
* [$webserviceParameters](#property-$webserviceParameters)
* [$def](#property-$def)
* [$fieldsRequired](#property-$fieldsRequired)
* [$fieldsRequiredDatabase](#property-$fieldsRequiredDatabase)
* [$fieldsRequiredLang](#property-$fieldsRequiredLang)
* [$fieldsSize](#property-$fieldsSize)
* [$fieldsSizeLang](#property-$fieldsSizeLang)
* [$fieldsValidate](#property-$fieldsValidate)
* [$fieldsValidateLang](#property-$fieldsValidateLang)
* [$id](#property-$id)
* [$id_lang](#property-$id_lang)
* [$identifier](#property-$identifier)
* [$image_dir](#property-$image_dir)
* [$image_format](#property-$image_format)
* [$table](#property-$table)
* [$tables](#property-$tables)

### Methods

* [__construct](#method-__construct)
* [_getScoreQuery](#method-_getScoreQuery)
* [add](#method-add)
* [addFieldsRequiredDatabase](#method-addFieldsRequiredDatabase)
* [associateTo](#method-associateTo)
* [clearCache](#method-clearCache)
* [delete](#method-delete)
* [deleteByIdCart](#method-deleteByIdCart)
* [deleteByProductId](#method-deleteByProductId)
* [deleteImage](#method-deleteImage)
* [deletePriorities](#method-deletePriorities)
* [deleteSelection](#method-deleteSelection)
* [displayFieldName](#method-displayFieldName)
* [duplicate](#method-duplicate)
* [duplicateShops](#method-duplicateShops)
* [exists](#method-exists)
* [existsInDatabase](#method-existsInDatabase)
* [formatFields](#method-formatFields)
* [formatValue](#method-formatValue)
* [getByProductId](#method-getByProductId)
* [getDefinition](#method-getDefinition)
* [getFieldByLang](#method-getFieldByLang)
* [getFields](#method-getFields)
* [getFieldsLang](#method-getFieldsLang)
* [getFieldsRequiredDatabase](#method-getFieldsRequiredDatabase)
* [getIdsByProductId](#method-getIdsByProductId)
* [getPriority](#method-getPriority)
* [getProductIdByDate](#method-getProductIdByDate)
* [getQuantityDiscount](#method-getQuantityDiscount)
* [getQuantityDiscounts](#method-getQuantityDiscounts)
* [getSpecificPrice](#method-getSpecificPrice)
* [getTranslationsFields](#method-getTranslationsFields)
* [getValidationRules](#method-getValidationRules)
* [getWebserviceObjectList](#method-getWebserviceObjectList)
* [getWebserviceParameters](#method-getWebserviceParameters)
* [hydrate](#method-hydrate)
* [hydrateCollection](#method-hydrateCollection)
* [isAssociatedToGroupShop](#method-isAssociatedToGroupShop)
* [isAssociatedToShop](#method-isAssociatedToShop)
* [isCurrentlyUsed](#method-isCurrentlyUsed)
* [isFeatureActive](#method-isFeatureActive)
* [isLangMultishop](#method-isLangMultishop)
* [makeTranslationFields](#method-makeTranslationFields)
* [save](#method-save)
* [setDefinitionRetrocompatibility](#method-setDefinitionRetrocompatibility)
* [setPriorities](#method-setPriorities)
* [setSpecificPriority](#method-setSpecificPriority)
* [toggleStatus](#method-toggleStatus)
* [update](#method-update)
* [validateControler](#method-validateControler)
* [validateController](#method-validateController)
* [validateField](#method-validateField)
* [validateFields](#method-validateFields)
* [validateFieldsLang](#method-validateFieldsLang)




Properties
----------


### <a name="property-$_cache_priorities"></a>$_cache_priorities

```php
protected mixed $_cache_priorities = array()
```





* Visibility: **protected**
* This property is **static**.
* Source: [classes/SpecificPrice.php line 91](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L91).


### <a name="property-$_specificPriceCache"></a>$_specificPriceCache

```php
protected mixed $_specificPriceCache = array()
```





* Visibility: **protected**
* This property is **static**.
* Source: [classes/SpecificPrice.php line 90](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L90).


### <a name="property-$definition"></a>$definition

```php
public mixed $definition = array('table' => 'specific_price', 'primary' => 'id_specific_price', 'fields' => array('id_group_shop' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId'), 'id_shop' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'id_cart' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'id_product' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'id_product_attribute' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId'), 'id_currency' => array('type' => self::TYPE_INT, 'required' => true), 'id_specific_price_rule' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId'), 'id_country' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'id_group' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'id_customer' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'price' => array('type' => self::TYPE_FLOAT, 'validate' => 'isPrice', 'required' => true), 'from_quantity' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedInt', 'required' => true), 'reduction' => array('type' => self::TYPE_FLOAT, 'validate' => 'isPrice', 'required' => true), 'reduction_type' => array('type' => self::TYPE_STRING, 'validate' => 'isReductionType', 'required' => true), 'from' => array('type' => self::TYPE_DATE, 'validate' => 'isDateFormat', 'required' => true), 'to' => array('type' => self::TYPE_DATE, 'validate' => 'isDateFormat', 'required' => true)))
```





* Visibility: **public**
* This property is **static**.
* Source: [classes/SpecificPrice.php line 50](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L50).


### <a name="property-$from"></a>$from

```php
public mixed $from
```





* Visibility: **public**
* Source: [classes/SpecificPrice.php line 44](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L44).


### <a name="property-$from_quantity"></a>$from_quantity

```php
public mixed $from_quantity
```





* Visibility: **public**
* Source: [classes/SpecificPrice.php line 41](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L41).


### <a name="property-$id_cart"></a>$id_cart

```php
public mixed $id_cart
```





* Visibility: **public**
* Source: [classes/SpecificPrice.php line 32](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L32).


### <a name="property-$id_country"></a>$id_country

```php
public mixed $id_country
```





* Visibility: **public**
* Source: [classes/SpecificPrice.php line 37](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L37).


### <a name="property-$id_currency"></a>$id_currency

```php
public mixed $id_currency
```





* Visibility: **public**
* Source: [classes/SpecificPrice.php line 36](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L36).


### <a name="property-$id_customer"></a>$id_customer

```php
public mixed $id_customer
```





* Visibility: **public**
* Source: [classes/SpecificPrice.php line 39](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L39).


### <a name="property-$id_group"></a>$id_group

```php
public mixed $id_group
```





* Visibility: **public**
* Source: [classes/SpecificPrice.php line 38](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L38).


### <a name="property-$id_group_shop"></a>$id_group_shop

```php
public mixed $id_group_shop
```





* Visibility: **public**
* Source: [classes/SpecificPrice.php line 35](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L35).


### <a name="property-$id_product"></a>$id_product

```php
public mixed $id_product
```





* Visibility: **public**
* Source: [classes/SpecificPrice.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L30).


### <a name="property-$id_product_attribute"></a>$id_product_attribute

```php
public mixed $id_product_attribute
```





* Visibility: **public**
* Source: [classes/SpecificPrice.php line 33](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L33).


### <a name="property-$id_shop"></a>$id_shop

```php
public mixed $id_shop
```





* Visibility: **public**
* Source: [classes/SpecificPrice.php line 34](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L34).


### <a name="property-$id_specific_price_rule"></a>$id_specific_price_rule

```php
public mixed $id_specific_price_rule
```





* Visibility: **public**
* Source: [classes/SpecificPrice.php line 31](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L31).


### <a name="property-$price"></a>$price

```php
public mixed $price
```





* Visibility: **public**
* Source: [classes/SpecificPrice.php line 40](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L40).


### <a name="property-$reduction"></a>$reduction

```php
public mixed $reduction
```





* Visibility: **public**
* Source: [classes/SpecificPrice.php line 42](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L42).


### <a name="property-$reduction_type"></a>$reduction_type

```php
public mixed $reduction_type
```





* Visibility: **public**
* Source: [classes/SpecificPrice.php line 43](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L43).


### <a name="property-$to"></a>$to

```php
public mixed $to
```





* Visibility: **public**
* Source: [classes/SpecificPrice.php line 45](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L45).


### <a name="property-$webserviceParameters"></a>$webserviceParameters

```php
protected mixed $webserviceParameters = array('objectsNodeName' => 'specific_prices', 'objectNodeName' => 'specific_price', 'fields' => array('id_group_shop' => array('xlink_resource' => 'shop_groups'), 'id_shop' => array('xlink_resource' => 'shops', 'required' => true), 'id_cart' => array('xlink_resource' => 'carts', 'required' => true), 'id_product' => array('xlink_resource' => 'products', 'required' => true), 'id_product_attribute' => array('xlink_resource' => 'product_attributes'), 'id_currency' => array('xlink_resource' => 'currencies', 'required' => true), 'id_country' => array('xlink_resource' => 'countries', 'required' => true), 'id_group' => array('xlink_resource' => 'groups', 'required' => true), 'id_customer' => array('xlink_resource' => 'customers', 'required' => true)))
```





* Visibility: **protected**
* Source: [classes/SpecificPrice.php line 73](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L73).


### <a name="property-$def"></a>$def

```php
protected array $def
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 122](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L122).


### <a name="property-$fieldsRequired"></a>$fieldsRequired

```php
protected mixed $fieldsRequired = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 72](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L72).


### <a name="property-$fieldsRequiredDatabase"></a>$fieldsRequiredDatabase

```php
protected mixed $fieldsRequiredDatabase = null
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 57](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L57).


### <a name="property-$fieldsRequiredLang"></a>$fieldsRequiredLang

```php
protected mixed $fieldsRequiredLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 87](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L87).


### <a name="property-$fieldsSize"></a>$fieldsSize

```php
protected mixed $fieldsSize = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 77](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L77).


### <a name="property-$fieldsSizeLang"></a>$fieldsSizeLang

```php
protected mixed $fieldsSizeLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 92](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L92).


### <a name="property-$fieldsValidate"></a>$fieldsValidate

```php
protected mixed $fieldsValidate = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 82](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L82).


### <a name="property-$fieldsValidateLang"></a>$fieldsValidateLang

```php
protected mixed $fieldsValidateLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 97](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L97).


### <a name="property-$id"></a>$id

```php
public integer $id
```





* Visibility: **public**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 48](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L48).


### <a name="property-$id_lang"></a>$id_lang

```php
protected integer $id_lang = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 51](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L51).


### <a name="property-$identifier"></a>$identifier

```php
protected mixed $identifier
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 67](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L67).


### <a name="property-$image_dir"></a>$image_dir

```php
protected string $image_dir = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 108](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L108).


### <a name="property-$image_format"></a>$image_format

```php
protected string $image_format = 'jpg'
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 111](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L111).


### <a name="property-$table"></a>$table

```php
protected mixed $table
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 62](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L62).


### <a name="property-$tables"></a>$tables

```php
protected mixed $tables = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 102](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L102).


Methods
-------


### <a name="method-__construct"></a>__construct

```php
mixed ObjectModelCore::__construct(integer $id, integer $id_lang, integer $id_shop)
```

Build object



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 150](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L150)


#### Arguments
* $id **integer** - Existing object id in order to load object (optional)
* $id_lang **integer** - Required if object is multilingual (optional)
* $id_shop **integer** - ID shop for objects with multishop on langs



### <a name="method-_getScoreQuery"></a>_getScoreQuery

```php
mixed SpecificPriceCore::_getScoreQuery($id_product, $id_shop, $id_currency, $id_country, $id_group, $id_customer)
```

score generation for quantity discount



* Visibility: **protected**
* This method is **static**.
* Source: [classes/SpecificPrice.php line 164](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L164)


#### Arguments
* $id_product **mixed**
* $id_shop **mixed**
* $id_currency **mixed**
* $id_country **mixed**
* $id_group **mixed**
* $id_customer **mixed**



### <a name="method-add"></a>add

```php
mixed SpecificPriceCore::add($autodate, $nullValues)
```





* Visibility: **public**
* Source: [classes/SpecificPrice.php line 93](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L93)


#### Arguments
* $autodate **mixed**
* $nullValues **mixed**



### <a name="method-addFieldsRequiredDatabase"></a>addFieldsRequiredDatabase

```php
mixed ObjectModelCore::addFieldsRequiredDatabase($fields)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 925](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L925)


#### Arguments
* $fields **mixed**



### <a name="method-associateTo"></a>associateTo

```php
boolean ObjectModelCore::associateTo(integer|array $id_shops, string $type)
```

This function associate an item to its context



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 973](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L973)


#### Arguments
* $id_shops **integer|array**
* $type **string**



### <a name="method-clearCache"></a>clearCache

```php
mixed ObjectModelCore::clearCache($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 939](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L939)


#### Arguments
* $all **mixed**



### <a name="method-delete"></a>delete

```php
mixed SpecificPriceCore::delete()
```





* Visibility: **public**
* Source: [classes/SpecificPrice.php line 119](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L119)




### <a name="method-deleteByIdCart"></a>deleteByIdCart

```php
mixed SpecificPriceCore::deleteByIdCart($id_cart, $id_product, $id_product_attribute)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/SpecificPrice.php line 143](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L143)


#### Arguments
* $id_cart **mixed**
* $id_product **mixed**
* $id_product_attribute **mixed**



### <a name="method-deleteByProductId"></a>deleteByProductId

```php
mixed SpecificPriceCore::deleteByProductId($id_product)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/SpecificPrice.php line 372](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L372)


#### Arguments
* $id_product **mixed**



### <a name="method-deleteImage"></a>deleteImage

```php
boolean ObjectModelCore::deleteImage()
```

Delete images associated with the object



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1047](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L1047)




### <a name="method-deletePriorities"></a>deletePriorities

```php
mixed SpecificPriceCore::deletePriorities()
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/SpecificPrice.php line 250](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L250)




### <a name="method-deleteSelection"></a>deleteSelection

```php
boolean ObjectModelCore::deleteSelection(array $selection)
```

Delete several objects from database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 559](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L559)


#### Arguments
* $selection **array**



### <a name="method-displayFieldName"></a>displayFieldName

```php
mixed ObjectModelCore::displayFieldName($field, $class, $htmlentities, \Context $context)
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 757](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L757)


#### Arguments
* $field **mixed**
* $class **mixed**
* $htmlentities **mixed**
* $context **[Context](class.ContextCore.md)**



### <a name="method-duplicate"></a>duplicate

```php
mixed SpecificPriceCore::duplicate($id_product)
```





* Visibility: **public**
* Source: [classes/SpecificPrice.php line 383](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L383)


#### Arguments
* $id_product **mixed**



### <a name="method-duplicateShops"></a>duplicateShops

```php
mixed ObjectModelCore::duplicateShops($id)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1017](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L1017)


#### Arguments
* $id **mixed**



### <a name="method-exists"></a>exists

```php
mixed SpecificPriceCore::exists($id_product, $id_product_attribute, $id_shop, $id_group, $id_country, $id_currency, $id_customer, $from_quantity, $from, $to)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/SpecificPrice.php line 401](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L401)


#### Arguments
* $id_product **mixed**
* $id_product_attribute **mixed**
* $id_shop **mixed**
* $id_group **mixed**
* $id_country **mixed**
* $id_currency **mixed**
* $id_customer **mixed**
* $from_quantity **mixed**
* $from **mixed**
* $to **mixed**



### <a name="method-existsInDatabase"></a>existsInDatabase

```php
boolean ObjectModelCore::existsInDatabase(integer $id_entity, string $table)
```

Specify if an ObjectModel is already in database



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1081](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L1081)


#### Arguments
* $id_entity **integer**
* $table **string**



### <a name="method-formatFields"></a>formatFields

```php
array ObjectModelCore::formatFields(integer $id_lang)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 272](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L272)


#### Arguments
* $id_lang **integer** - If this parameter is given, only take lang fields



### <a name="method-formatValue"></a>formatValue

```php
mixed ObjectModelCore::formatValue(mixed $value, integer $type, $with_quotes)
```

Format a data



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 319](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L319)


#### Arguments
* $value **mixed**
* $type **integer**
* $with_quotes **mixed**



### <a name="method-getByProductId"></a>getByProductId

```php
mixed SpecificPriceCore::getByProductId($id_product, $id_product_attribute, $id_cart)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/SpecificPrice.php line 133](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L133)


#### Arguments
* $id_product **mixed**
* $id_product_attribute **mixed**
* $id_cart **mixed**



### <a name="method-getDefinition"></a>getDefinition

```php
array ObjectModelCore::getDefinition(string $class, string $field)
```

Get object definition



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1184](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L1184)


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
* Source: [classes/ObjectModel.php line 1261](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L1261)


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
* Source: [classes/ObjectModel.php line 234](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L234)




### <a name="method-getFieldsLang"></a>getFieldsLang

```php
array ObjectModelCore::getFieldsLang()
```

Prepare multilang fields



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 249](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L249)




### <a name="method-getFieldsRequiredDatabase"></a>getFieldsRequiredDatabase

```php
mixed ObjectModelCore::getFieldsRequiredDatabase($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 917](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L917)


#### Arguments
* $all **mixed**



### <a name="method-getIdsByProductId"></a>getIdsByProductId

```php
mixed SpecificPriceCore::getIdsByProductId($id_product, $id_product_attribute, $id_cart)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/SpecificPrice.php line 151](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L151)


#### Arguments
* $id_product **mixed**
* $id_product_attribute **mixed**
* $id_cart **mixed**



### <a name="method-getPriority"></a>getPriority

```php
mixed SpecificPriceCore::getPriority($id_product)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/SpecificPrice.php line 178](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L178)


#### Arguments
* $id_product **mixed**



### <a name="method-getProductIdByDate"></a>getProductIdByDate

```php
mixed SpecificPriceCore::getProductIdByDate($id_shop, $id_currency, $id_country, $id_group, $beginning, $ending, $id_customer, $with_combination_id)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/SpecificPrice.php line 344](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L344)


#### Arguments
* $id_shop **mixed**
* $id_currency **mixed**
* $id_country **mixed**
* $id_group **mixed**
* $beginning **mixed**
* $ending **mixed**
* $id_customer **mixed**
* $with_combination_id **mixed**



### <a name="method-getQuantityDiscount"></a>getQuantityDiscount

```php
mixed SpecificPriceCore::getQuantityDiscount($id_product, $id_shop, $id_currency, $id_country, $id_group, $quantity, $id_product_attribute, $id_customer)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/SpecificPrice.php line 315](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L315)


#### Arguments
* $id_product **mixed**
* $id_shop **mixed**
* $id_currency **mixed**
* $id_country **mixed**
* $id_group **mixed**
* $quantity **mixed**
* $id_product_attribute **mixed**
* $id_customer **mixed**



### <a name="method-getQuantityDiscounts"></a>getQuantityDiscounts

```php
mixed SpecificPriceCore::getQuantityDiscounts($id_product, $id_shop, $id_currency, $id_country, $id_group, $id_product_attribute, $all_combinations, $id_customer)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/SpecificPrice.php line 270](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L270)


#### Arguments
* $id_product **mixed**
* $id_shop **mixed**
* $id_currency **mixed**
* $id_country **mixed**
* $id_group **mixed**
* $id_product_attribute **mixed**
* $all_combinations **mixed**
* $id_customer **mixed**



### <a name="method-getSpecificPrice"></a>getSpecificPrice

```php
mixed SpecificPriceCore::getSpecificPrice($id_product, $id_shop, $id_currency, $id_country, $id_group, $quantity, $id_product_attribute, $id_customer, $id_cart)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/SpecificPrice.php line 202](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L202)


#### Arguments
* $id_product **mixed**
* $id_shop **mixed**
* $id_currency **mixed**
* $id_country **mixed**
* $id_group **mixed**
* $quantity **mixed**
* $id_product_attribute **mixed**
* $id_customer **mixed**
* $id_cart **mixed**



### <a name="method-getTranslationsFields"></a>getTranslationsFields

```php
mixed ObjectModelCore::getTranslationsFields($fields_array)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 595](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L595)


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
* Source: [classes/ObjectModel.php line 130](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L130)


#### Arguments
* $class **string** - Child class name for static use (optional)



### <a name="method-getWebserviceObjectList"></a>getWebserviceObjectList

```php
mixed ObjectModelCore::getWebserviceObjectList($sql_join, $sql_filter, $sql_sort, $sql_limit)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 890](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L890)


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
* Source: [classes/ObjectModel.php line 816](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L816)


#### Arguments
* $ws_params_attribute_name **mixed**



### <a name="method-hydrate"></a>hydrate

```php
mixed ObjectModelCore::hydrate(array $data, integer $id_lang)
```

Fill an object with given data. Data must be an array with this syntax: array(objProperty => value, objProperty2 => value, etc.)



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1116](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L1116)


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
* Source: [classes/ObjectModel.php line 1135](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L1135)


#### Arguments
* $class **string** - Class of objects to hydrate
* $datas **array** - List of data (multi-dimensional array)
* $id_lang **integer**



### <a name="method-isAssociatedToGroupShop"></a>isAssociatedToGroupShop

```php
boolean ObjectModelCore::isAssociatedToGroupShop(integer $id_group_shop)
```

Check if current object is associated to a group shop



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1003](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L1003)


#### Arguments
* $id_group_shop **integer**



### <a name="method-isAssociatedToShop"></a>isAssociatedToShop

```php
boolean ObjectModelCore::isAssociatedToShop(integer $id_shop)
```

Check if current object is associated to a shop



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 954](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L954)


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
* Source: [classes/ObjectModel.php line 1099](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L1099)


#### Arguments
* $table **string** - name of table linked to entity
* $has_active_column **boolean** - true if the table has an active column



### <a name="method-isFeatureActive"></a>isFeatureActive

```php
boolean SpecificPriceCore::isFeatureActive()
```

This method is allow to know if a feature is used or active



* Visibility: **public**
* This method is **static**.
* Source: [classes/SpecificPrice.php line 396](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L396)




### <a name="method-isLangMultishop"></a>isLangMultishop

```php
mixed ObjectModelCore::isLangMultishop()
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1037](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L1037)




### <a name="method-makeTranslationFields"></a>makeTranslationFields

```php
mixed ObjectModelCore::makeTranslationFields($fields, $fields_array, $id_language)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 611](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L611)


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
* Source: [classes/ObjectModel.php line 360](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L360)


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
* Source: [classes/ObjectModel.php line 1207](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L1207)




### <a name="method-setPriorities"></a>setPriorities

```php
mixed SpecificPriceCore::setPriorities($priorities)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/SpecificPrice.php line 238](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L238)


#### Arguments
* $priorities **mixed**



### <a name="method-setSpecificPriority"></a>setSpecificPriority

```php
mixed SpecificPriceCore::setSpecificPriority($id_product, $priorities)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/SpecificPrice.php line 257](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L257)


#### Arguments
* $id_product **mixed**
* $priorities **mixed**



### <a name="method-toggleStatus"></a>toggleStatus

```php
boolean ObjectModelCore::toggleStatus()
```

Toggle object status in database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 575](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L575)




### <a name="method-update"></a>update

```php
mixed SpecificPriceCore::update($null_values)
```





* Visibility: **public**
* Source: [classes/SpecificPrice.php line 107](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/SpecificPrice.php#L107)


#### Arguments
* $null_values **mixed**



### <a name="method-validateControler"></a>validateControler

```php
mixed ObjectModelCore::validateControler($htmlentities)
```

TODO: refactor rename all calls to this to validateController



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 772](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L772)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateController"></a>validateController

```php
mixed ObjectModelCore::validateController($htmlentities)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 778](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L778)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateField"></a>validateField

```php
boolean|string ObjectModelCore::validateField(string $field, mixed $value, integer $id_lang)
```

Validate a single field



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 710](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L710)


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
* Source: [classes/ObjectModel.php line 649](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L649)


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
* Source: [classes/ObjectModel.php line 675](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.9/classes/ObjectModel.php#L675)


#### Arguments
* $die **boolean**
* $error_return **boolean**


