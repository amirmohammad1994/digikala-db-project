Libraries used :

1-mysql-connector
$ sudo pip install mysql-connector


2-openpyxl
For reading xlxs files
$ sudo pip install openpyxl

---------------------------------------

MySQL version :
 mysql  Ver 14.14 Distrib 5.7.26, for Linux (x86_64) using  EditLine wrapper

---------------------------------------

فرض شده است داده ها در فایلی به نام
product-list
در پوشه
data
قرار دارد.

  اطلاعات اتصال به دیتابیس
در فایل
create_database.py
اصلاح شود.

dbconn = mysql.connector.connect(
  host="localhost",
  user="amir",
  passwd="1234",
  charset='utf8'
)
print(dbconn)
mycursor = dbconn.cursor()
mycursor.execute("CREATE DATABASE amir-mahdi-db-project")


---------------------------------------

فایل
extract-attributes.py
برای هر موضوع مثل کتاب چاپی مجموعه تمامی کلید های موجود در ستون های آخر این موضوع را استخراج و به همراه تعداد رکوردی که شامل این کلید است در فایل
attributes.txt
ذخیره می کند.

---------------------------------------
