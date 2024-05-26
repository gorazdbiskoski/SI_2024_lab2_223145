# Втора лабораториска вежба по Софтверско инженерство
## Горазд Бишкоски, бр. на индекс 223145

### Control Flow Graph

![Screenshot 2024-05-25 132137](https://github.com/gorazdbiskoski/SI_2024_lab2_223145/assets/126030318/c5846b2e-fb63-4f72-b8ee-18f63f7353c1)

### Цикломатска комплексност

Цикломатската комплексност на овој код е 10, Нејзе ја добив поради тоа што има 9 предикатни јазли и ја искористив формулата бр. на предикатни јазли + 1.

### Тест случаи според критериумот Multiple Condition за условот if (item.getPrice() > 300 && item.getDiscount() > 0 && item.getBarcode().charAt(0) == '0')
-True & True & True     : item.price = 350; item.discount = 0.25; item.barcode = "0123"

-True & True & False    : item.price = 350; item.discount = 0.25; item.barcode = "1234"

-True & False & X       : item.price = 350; item.discount = -1; item.barcode = "1234"

-False & X & X          : item.price = 200; item.discount = -1; item.barcode = "1234"


### Тест случаи според критериумот Every path

![excel-ss](https://github.com/gorazdbiskoski/SI_2024_lab2_223145/assets/126030318/06c2c35d-8e99-41ed-acc5-ff515b1e644a)

### Објаснување на напишаните unit tests
Најпрво почнав со исполување на барањата за Control Flow Graph, Цикломатска комплексност, Multiple Condition tests и Every Path conditions.
Потоа во Inteliij IDEA направив нов проект што build системот ќе е во Gradle i при клик на класата SILab2 го кликнав копчето за креирање на тестови.
При пишување на Unit тестовите јас гледав од Google Sheets-от каде што пишував слични тестови со помош на функциите "AssertTrue" и "AssertFalse" 
