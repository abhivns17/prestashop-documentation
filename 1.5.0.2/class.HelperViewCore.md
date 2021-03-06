Class HelperViewCore
=====================





* Class name: HelperViewCore
* Parent class: [Helper](class.HelperCore.md)
* Source: [classes/helper/HelperView.php line 28](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/HelperView.php#L28)


Contents
--------


### Properties

* [$id](#property-$id)
* [$table](#property-$table)
* [$title](#property-$title)
* [$token](#property-$token)
* [$toolbar](#property-$toolbar)
* [$base_folder](#property-$base_folder)
* [$base_tpl](#property-$base_tpl)
* [$context](#property-$context)
* [$currentIndex](#property-$currentIndex)
* [$identifier](#property-$identifier)
* [$override_folder](#property-$override_folder)
* [$ps_help_context](#property-$ps_help_context)
* [$show_toolbar](#property-$show_toolbar)
* [$toolbar_btn](#property-$toolbar_btn)
* [$toolbar_fix](#property-$toolbar_fix)
* [$tpl](#property-$tpl)
* [$tpl_vars](#property-$tpl_vars)

### Methods

* [__construct](#method-__construct)
* [buildHtmlOptions](#method-buildHtmlOptions)
* [createTemplate](#method-createTemplate)
* [generate](#method-generate)
* [generateView](#method-generateView)
* [l](#method-l)
* [renderAdminCategorieTree](#method-renderAdminCategorieTree)
* [renderAssoShop](#method-renderAssoShop)
* [renderRequiredFields](#method-renderRequiredFields)
* [selectInput](#method-selectInput)
* [setTpl](#method-setTpl)




Properties
----------


### <a name="property-$id"></a>$id

```php
public mixed $id
```





* Visibility: **public**
* Source: [classes/helper/HelperView.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/HelperView.php#L30).


### <a name="property-$table"></a>$table

```php
public mixed $table
```





* Visibility: **public**
* Source: [classes/helper/HelperView.php line 32](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/HelperView.php#L32).


### <a name="property-$title"></a>$title

```php
public \if $title = null
```





* Visibility: **public**
* Source: [classes/helper/HelperView.php line 36](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/HelperView.php#L36).


### <a name="property-$token"></a>$token

```php
public mixed $token
```





* Visibility: **public**
* Source: [classes/helper/HelperView.php line 33](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/HelperView.php#L33).


### <a name="property-$toolbar"></a>$toolbar

```php
public mixed $toolbar = true
```





* Visibility: **public**
* Source: [classes/helper/HelperView.php line 31](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/HelperView.php#L31).


### <a name="property-$base_folder"></a>$base_folder

```php
public string $base_folder
```





* Visibility: **public**
* This property is defined by [HelperCore](class.HelperCore.md).
* Source: [classes/helper/Helper.php line 47](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/Helper.php#L47).


### <a name="property-$base_tpl"></a>$base_tpl

```php
public string $base_tpl = 'content.tpl'
```





* Visibility: **public**
* This property is defined by [HelperCore](class.HelperCore.md).
* Source: [classes/helper/Helper.php line 60](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/Helper.php#L60).


### <a name="property-$context"></a>$context

```php
public mixed $context
```





* Visibility: **public**
* This property is defined by [HelperCore](class.HelperCore.md).
* Source: [classes/helper/Helper.php line 43](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/Helper.php#L43).


### <a name="property-$currentIndex"></a>$currentIndex

```php
public mixed $currentIndex
```





* Visibility: **public**
* This property is defined by [HelperCore](class.HelperCore.md).
* Source: [classes/helper/Helper.php line 35](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/Helper.php#L35).


### <a name="property-$identifier"></a>$identifier

```php
public mixed $identifier
```





* Visibility: **public**
* This property is defined by [HelperCore](class.HelperCore.md).
* Source: [classes/helper/Helper.php line 37](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/Helper.php#L37).


### <a name="property-$override_folder"></a>$override_folder

```php
public string $override_folder
```





* Visibility: **public**
* This property is defined by [HelperCore](class.HelperCore.md).
* Source: [classes/helper/Helper.php line 50](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/Helper.php#L50).


### <a name="property-$ps_help_context"></a>$ps_help_context

```php
public mixed $ps_help_context
```





* Visibility: **public**
* This property is defined by [HelperCore](class.HelperCore.md).
* Source: [classes/helper/Helper.php line 40](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/Helper.php#L40).


### <a name="property-$show_toolbar"></a>$show_toolbar

```php
public mixed $show_toolbar = true
```





* Visibility: **public**
* This property is defined by [HelperCore](class.HelperCore.md).
* Source: [classes/helper/Helper.php line 42](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/Helper.php#L42).


### <a name="property-$toolbar_btn"></a>$toolbar_btn

```php
public mixed $toolbar_btn
```





* Visibility: **public**
* This property is defined by [HelperCore](class.HelperCore.md).
* Source: [classes/helper/Helper.php line 39](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/Helper.php#L39).


### <a name="property-$toolbar_fix"></a>$toolbar_fix

```php
public mixed $toolbar_fix = false
```





* Visibility: **public**
* This property is defined by [HelperCore](class.HelperCore.md).
* Source: [classes/helper/Helper.php line 44](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/Helper.php#L44).


### <a name="property-$tpl"></a>$tpl

```php
protected \smartyTemplate $tpl
```





* Visibility: **protected**
* This property is defined by [HelperCore](class.HelperCore.md).
* Source: [classes/helper/Helper.php line 55](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/Helper.php#L55).


### <a name="property-$tpl_vars"></a>$tpl_vars

```php
public mixed $tpl_vars = array()
```





* Visibility: **public**
* This property is defined by [HelperCore](class.HelperCore.md).
* Source: [classes/helper/Helper.php line 62](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/Helper.php#L62).


Methods
-------


### <a name="method-__construct"></a>__construct

```php
mixed HelperViewCore::__construct()
```





* Visibility: **public**
* Source: [classes/helper/HelperView.php line 38](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/HelperView.php#L38)




### <a name="method-buildHtmlOptions"></a>buildHtmlOptions

```php
string HelperCore::buildHtmlOptions(array $html_options)
```

Create html a string containing html options
eg: buildHtmlOptions(array('name' => 'myInputName', 'id' => 'myInputId'));
    return => 'name="myInputName" id="myInputId"'



* Visibility: **protected**
* This method is **static**.
* This method is defined by [HelperCore](class.HelperCore.md).
* Source: [classes/helper/Helper.php line 269](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/Helper.php#L269)


#### Arguments
* $html_options **array**



### <a name="method-createTemplate"></a>createTemplate

```php
\Template HelperCore::createTemplate(string $tpl_name)
```

Create a template from the override file, else from the base file.



* Visibility: **public**
* This method is defined by [HelperCore](class.HelperCore.md).
* Source: [classes/helper/Helper.php line 80](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/Helper.php#L80)


#### Arguments
* $tpl_name **string** - filename



### <a name="method-generate"></a>generate

```php
void HelperCore::generate()
```

default behaviour for helper is to return a tpl fetched



* Visibility: **public**
* This method is defined by [HelperCore](class.HelperCore.md).
* Source: [classes/helper/Helper.php line 94](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/Helper.php#L94)




### <a name="method-generateView"></a>generateView

```php
mixed HelperViewCore::generateView()
```





* Visibility: **public**
* Source: [classes/helper/HelperView.php line 45](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/HelperView.php#L45)




### <a name="method-l"></a>l

```php
string HelperCore::l(mixed $string, string $class, \boolan $addslashes, boolean $htmlentities)
```

use translations files to replace english expression.



* Visibility: **protected**
* This method is defined by [HelperCore](class.HelperCore.md).
* Source: [classes/helper/Helper.php line 288](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/Helper.php#L288)


#### Arguments
* $string **mixed** - term or expression in english
* $class **string**
* $addslashes **boolan** - if set to true, the return value will pass through addslashes(). Otherwise, stripslashes().
* $htmlentities **boolean** - if set to true(default), the return value will pass through htmlentities($string, ENT_QUOTES, &#039;utf-8&#039;)



### <a name="method-renderAdminCategorieTree"></a>renderAdminCategorieTree

```php
string HelperCore::renderAdminCategorieTree(\type $trads, \type $selected_cat, \type $input_name, $use_radio, $use_search, $disabled_categories)
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [HelperCore](class.HelperCore.md).
* Source: [classes/helper/Helper.php line 124](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/Helper.php#L124)


#### Arguments
* $trads **type** - values of translations keys
				For the moment, translation are not automatic
* $selected_cat **type** - array of selected categories
            Format
                Array
                (
                     [0] =&gt; 1
                 [1] =&gt; 2
            )
                OR
            Array
            (
                 [1] =&gt; Array
                      (
                            [id_category] =&gt; 1
                            [name] =&gt; Home page
                            [link_rewrite] =&gt; home
                      )
            )
* $input_name **type** - name of input
* $use_radio **mixed**
* $use_search **mixed**
* $disabled_categories **mixed**



### <a name="method-renderAssoShop"></a>renderAssoShop

```php
string HelperCore::renderAssoShop(string $type)
```

Render an area to determinate shop association



* Visibility: **public**
* This method is defined by [HelperCore](class.HelperCore.md).
* Source: [classes/helper/Helper.php line 315](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/Helper.php#L315)


#### Arguments
* $type **string** - &#039;shop&#039; or &#039;group_shop&#039;



### <a name="method-renderRequiredFields"></a>renderRequiredFields

```php
string HelperCore::renderRequiredFields(string $class_name, string $identifier, array $table_fields)
```

Render a form with potentials required fields



* Visibility: **public**
* This method is defined by [HelperCore](class.HelperCore.md).
* Source: [classes/helper/Helper.php line 357](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/Helper.php#L357)


#### Arguments
* $class_name **string**
* $identifier **string**
* $table_fields **array**



### <a name="method-selectInput"></a>selectInput

```php
string HelperCore::selectInput(array $values, array $html_options, array $select_options)
```

Create a select input field



* Visibility: **public**
* This method is **static**.
* This method is defined by [HelperCore](class.HelperCore.md).
* Source: [classes/helper/Helper.php line 225](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/Helper.php#L225)


#### Arguments
* $values **array**
* $html_options **array** - any key =&gt; value options
* $select_options **array** - 
key: the array value that will be used as a key in my select (optional)
value: the array value that will be used as a label in my select (optional)
empty: the label displayed as an empty value (optional)
selected: the key corresponding to the selected value  (optional)




### <a name="method-setTpl"></a>setTpl

```php
mixed HelperCore::setTpl($tpl)
```





* Visibility: **public**
* This method is defined by [HelperCore](class.HelperCore.md).
* Source: [classes/helper/Helper.php line 69](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/helper/Helper.php#L69)


#### Arguments
* $tpl **mixed**


