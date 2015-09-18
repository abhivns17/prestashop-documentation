Mail
===============

DISCLAIMER

Do not edit or add to this file if you wish to upgrade this module to newer
versions in the future. If you wish to customize this module for your
needs please refer to http://doc.prestashop.com/display/PS15/Overriding+default+behaviors
#Overridingdefaultbehaviors-Overridingamodule%27sbehavior for more information.


* Class name: Mail
* Namespace: 
* Parent class: [MailCore](MailCore.md)



Constants
----------


### TYPE_HTML

    const TYPE_HTML = 1





### TYPE_TEXT

    const TYPE_TEXT = 2





### TYPE_BOTH

    const TYPE_BOTH = 3





Properties
----------


### $id

    public mixed $id





* Visibility: **public**


### $recipient

    public string $recipient





* Visibility: **public**


### $template

    public string $template





* Visibility: **public**


### $subject

    public string $subject





* Visibility: **public**


### $id_lang

    public integer $id_lang





* Visibility: **public**


### $date_add

    public integer $date_add





* Visibility: **public**


### $definition

    public mixed $definition = array('table' => 'mail', 'primary' => 'id_mail', 'fields' => array('recipient' => array('type' => self::TYPE_STRING, 'validate' => 'isEmail', 'copy_post' => false, 'required' => true, 'size' => 126), 'template' => array('type' => self::TYPE_STRING, 'validate' => 'isTplName', 'copy_post' => false, 'required' => true, 'size' => 62), 'subject' => array('type' => self::TYPE_STRING, 'validate' => 'isMailSubject', 'copy_post' => false, 'required' => true, 'size' => 254), 'id_lang' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'copy_post' => false, 'required' => true), 'date_add' => array('type' => self::TYPE_DATE, 'validate' => 'isDate', 'copy_post' => false, 'required' => true)))





* Visibility: **public**
* This property is **static**.


Methods
-------


### send

    mixed Mail::send($id_lang, $template, $subject, $template_vars, $to, $to_name, $from, $from_name, $file_attachment, $mode_smtp, $template_path, $die, $id_shop, $bcc, $reply_to)





* Visibility: **public**
* This method is **static**.


#### Arguments
* $id_lang **mixed**
* $template **mixed**
* $subject **mixed**
* $template_vars **mixed**
* $to **mixed**
* $to_name **mixed**
* $from **mixed**
* $from_name **mixed**
* $file_attachment **mixed**
* $mode_smtp **mixed**
* $template_path **mixed**
* $die **mixed**
* $id_shop **mixed**
* $bcc **mixed**
* $reply_to **mixed**



### Send

    mixed MailCore::Send(integer $id_lang, string $template, string $subject, string $template_vars, string $to, string $to_name, string $from, string $from_name, array $file_attachment, $mode_smtp, string $template_path, boolean $die, $id_shop, string $bcc, $reply_to)

Send Email



* Visibility: **public**
* This method is **static**.
* This method is defined by [MailCore](MailCore.md)


#### Arguments
* $id_lang **integer** - &lt;p&gt;Language of the email (to translate the template)&lt;/p&gt;
* $template **string** - &lt;p&gt;Template: the name of template not be a var but a string !&lt;/p&gt;
* $subject **string**
* $template_vars **string**
* $to **string**
* $to_name **string**
* $from **string**
* $from_name **string**
* $file_attachment **array** - &lt;p&gt;Array with three parameters (content, mime and name). You can use an array of array to attach multiple files&lt;/p&gt;
* $mode_smtp **mixed**
* $template_path **string**
* $die **boolean**
* $id_shop **mixed**
* $bcc **string** - &lt;p&gt;Bcc recipient&lt;/p&gt;
* $reply_to **mixed**



### eraseLog

    mixed MailCore::eraseLog($id_mail)





* Visibility: **public**
* This method is **static**.
* This method is defined by [MailCore](MailCore.md)


#### Arguments
* $id_mail **mixed**



### eraseAllLogs

    mixed MailCore::eraseAllLogs()





* Visibility: **public**
* This method is **static**.
* This method is defined by [MailCore](MailCore.md)




### sendMailTest

    mixed MailCore::sendMailTest($smtpChecked, $smtpServer, $content, $subject, $type, $to, $from, $smtpLogin, $smtpPassword, $smtpPort, $smtpEncryption)





* Visibility: **public**
* This method is **static**.
* This method is defined by [MailCore](MailCore.md)


#### Arguments
* $smtpChecked **mixed**
* $smtpServer **mixed**
* $content **mixed**
* $subject **mixed**
* $type **mixed**
* $to **mixed**
* $from **mixed**
* $smtpLogin **mixed**
* $smtpPassword **mixed**
* $smtpPort **mixed**
* $smtpEncryption **mixed**



### l

    mixed MailCore::l(string $string, $id_lang, \Context $context)

This method is used to get the translation for email Object.

For an object is forbidden to use htmlentities,
we have to return a sentence with accents.

* Visibility: **public**
* This method is **static**.
* This method is defined by [MailCore](MailCore.md)


#### Arguments
* $string **string** - &lt;p&gt;raw sentence (write directly in file)&lt;/p&gt;
* $id_lang **mixed**
* $context **Context**



### generateId

    mixed MailCore::generateId($idstring)





* Visibility: **protected**
* This method is **static**.
* This method is defined by [MailCore](MailCore.md)


#### Arguments
* $idstring **mixed**



### isMultibyte

    mixed MailCore::isMultibyte($data)





* Visibility: **public**
* This method is **static**.
* This method is defined by [MailCore](MailCore.md)


#### Arguments
* $data **mixed**



### mimeEncode

    mixed MailCore::mimeEncode($string, $charset, $newline)





* Visibility: **public**
* This method is **static**.
* This method is defined by [MailCore](MailCore.md)


#### Arguments
* $string **mixed**
* $charset **mixed**
* $newline **mixed**

