# Отчёт о тестировании программы Credit Card Number Validator

## Краткое описание

31 июля 2020г. было проведено функциональное тестирование программы Credit Card Number Validator, а также тестирование установки среды разработки IntelliJ IDEA.

На тестирование затрачено: 2 часа.

В результате тестирования были выявлены следующие дефекты:
* [Появляется ошибка FAIL при вводе валидных номеров кредитных карт длиной более 16 цифр](https://github.com/IrynaV25/Credit-Card-Number-Validator/issues/1#issue-670103550).
* [Появляется ошибка FAIL при вводе валидных номеров кредитных карт длиной менее 16 цифр](https://github.com/IrynaV25/Credit-Card-Number-Validator/issues/2#issue-670131685).

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:
* [инструкция по установке IntelliJ IDEA](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/idea.md);
* баг-репорты;
* отчет о тестировании.

В качестве тестовых данных использовались данные, взятые из открытых генераторов валидных номеров кредитных карт:
* [freeformatter.com](https://www.freeformatter.com/credit-card-number-generator-validator.html);
* [getcreditcardnumbers.com](https://www.getcreditcardnumbers.com/).

Валидные номера карт:
* Result for 5351719427810741: OK
* Result for 4539593873548644: OK
* Result for 4532744507373092: OK
* Result for 5572505114917342: OK
* Result for 2221006922322231: OK
* Result for 3543116122118746345: OK
* Result for 30014807037895: OK

Невалидные номера карт:
* Result for 511489459245651: FAIL
* Result for 5332041703405400: FAIL

Тестирование производилось в следующем окружении:
* Устройство – планшет Surface3pro;
* ОС – Windows 10 Pro, версия 1903 (64 бит);
* браузер – Google Chrome, версия 84.0.4147.105 (64 бит);
* версия Java – openjdk version "11.0.8" 2020-07-14;
* версия Git Bash: mintty 3.1.6 (x86_64-pc-msys);
* версия IntelliJ IDEA: IntelliJ IDEA Community 2020.2.