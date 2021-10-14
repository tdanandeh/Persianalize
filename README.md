<div dir="rtl">

# فارسی ساز لاراول
و سایر زبان ها
 
**فارسی ساز**
 برای استفاده در اینپوت ها و ورودی ها و حذف عربی و سایر نوشته های مشابه

## نصب

با کامپوزر
<div dir="ltr">
 
``` bash
composer require tdanandeh/persianalize
```
 
</div>
اگر لاراول شما  5.5 (یا پایینتر) است به قسمت
service provider در فایل  config/app.php
رفته و دستور زیر را اضافه کنید.
 <div dir="ltr">
  
``` php
TohidDanandeh\Persianalize\PersianalizeServiceProvider:class
```
  
</div>
اگر نسخه لاراول شما از 5.5+ بیشتر است ، بصورت خودکار از ویژگی لاراول استفاده می کند و نیازی به اضافه کردن نیست.
## طریقه استفاده
<div dir="ltr">

``` php
$result = Persian::numbers_fa('123٤٥٦'); // return ۱۲۳۴۵۶

$result = Persian::numbers_en('۱۲۳٤٥٦'); // return 123456

$result = Persian::text('ي ڲ ڬ'); // return ی گ ک

$result = Persian::persian($text); // make texts and numbers Persian 

$result = Persian::standard($text); // make texts Persian and numbers English 
```

</div>
## تغییرات

توسعه
پکیج برای لاراول 8
</div>
