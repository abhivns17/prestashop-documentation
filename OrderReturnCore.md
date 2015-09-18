OrderReturnCore
===============






* Class name: OrderReturnCore
* Namespace: 
* Parent class: ObjectModel





Properties
----------


### $id

    public integer $id





* Visibility: **public**


### $id_customer

    public integer $id_customer





* Visibility: **public**


### $id_order

    public integer $id_order





* Visibility: **public**


### $state

    public integer $state





* Visibility: **public**


### $question

    public string $question





* Visibility: **public**


### $date_add

    public string $date_add





* Visibility: **public**


### $date_upd

    public string $date_upd





* Visibility: **public**


### $definition

    public mixed $definition = array('table' => 'order_return', 'primary' => 'id_order_return', 'fields' => array('id_customer' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'id_order' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'question' => array('type' => self::TYPE_HTML, 'validate' => 'isCleanHtml'), 'state' => array('type' => self::TYPE_STRING), 'date_add' => array('type' => self::TYPE_DATE, 'validate' => 'isDate'), 'date_upd' => array('type' => self::TYPE_DATE, 'validate' => 'isDate')))





* Visibility: **public**
* This property is **static**.


Methods
-------


### addReturnDetail

    mixed OrderReturnCore::addReturnDetail($order_detail_list, $product_qty_list, $customization_ids, $customization_qty_input)





* Visibility: **public**


#### Arguments
* $order_detail_list **mixed**
* $product_qty_list **mixed**
* $customization_ids **mixed**
* $customization_qty_input **mixed**



### checkEnoughProduct

    mixed OrderReturnCore::checkEnoughProduct($order_detail_list, $product_qty_list, $customization_ids, $customization_qty_input)





* Visibility: **public**


#### Arguments
* $order_detail_list **mixed**
* $product_qty_list **mixed**
* $customization_ids **mixed**
* $customization_qty_input **mixed**



### countProduct

    mixed OrderReturnCore::countProduct()





* Visibility: **public**




### getOrdersReturn

    mixed OrderReturnCore::getOrdersReturn($customer_id, $order_id, $no_denied, \Context $context)





* Visibility: **public**
* This method is **static**.


#### Arguments
* $customer_id **mixed**
* $order_id **mixed**
* $no_denied **mixed**
* $context **Context**



### getOrdersReturnDetail

    mixed OrderReturnCore::getOrdersReturnDetail($id_order_return)





* Visibility: **public**
* This method is **static**.


#### Arguments
* $id_order_return **mixed**



### getOrdersReturnProducts

    array OrderReturnCore::getOrdersReturnProducts(integer $order_return_id, \Order $order)





* Visibility: **public**
* This method is **static**.


#### Arguments
* $order_return_id **integer**
* $order **Order**



### getReturnedCustomizedProducts

    mixed OrderReturnCore::getReturnedCustomizedProducts($id_order)





* Visibility: **public**
* This method is **static**.


#### Arguments
* $id_order **mixed**



### deleteOrderReturnDetail

    mixed OrderReturnCore::deleteOrderReturnDetail($id_order_return, $id_order_detail, $id_customization)





* Visibility: **public**
* This method is **static**.


#### Arguments
* $id_order_return **mixed**
* $id_order_detail **mixed**
* $id_customization **mixed**



### getProductReturnDetail

    mixed OrderReturnCore::getProductReturnDetail($id_order_detail)

Get return details for one product line



* Visibility: **public**
* This method is **static**.


#### Arguments
* $id_order_detail **mixed**



### addReturnedQuantity

    mixed OrderReturnCore::addReturnedQuantity(array $products, integer $id_order)

Add returned quantity to products list



* Visibility: **public**
* This method is **static**.


#### Arguments
* $products **array**
* $id_order **integer**

