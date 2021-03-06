# Отчёт о тестировании функционала валидации номера банковской карты

## Краткое описание

01.12.21 - 01.12.21 было проведено позитивное и негативное приложения для валидации номера банковской карты.

На тестирование затрачено: 1 час.

В результате тестирования выявлены следующие дефекты:
* [Баг-репорт №1](https://github.com/imandrik/HomeWork1.2/issues/1);
* [Баг-репорт №2](https://github.com/imandrik/HomeWork1.2/issues/2).


## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты*:
* [генератор номеров банковских карт](https://www.freeformatter.com/credit-card-number-generator-validator.html);
* [тестовые сценарии](https://docs.google.com/spreadsheets/d/1eEN5cjjawsfRiqSg8lN7AYtahwVVAV_R3Pu-moX-F88/edit?usp=sharing).

В качестве тестовых данных использовались данные из [генератора номеров банковских карт](https://www.freeformatter.com/credit-card-number-generator-validator.html):
* Visa 4716558930928779 (ожидаемый результат - Result is OK);
* Visa 4916923879620196828 (ожидаемый результат - Result is OK);
* MasterCard 5359808910040858 (ожидаемый результат - Result is OK);
* American Express 375437645677486 (ожидаемый результат - Result is OK);
* Maestro 6759029072015117 (ожидаемый результат - Result is OK).

Данные для негативного тестирования:
* 5555555555555555 (ожидаемый результат - Result is FAIL);
* номеркарты (ожидаемый результат - Result is FAIL);
* пустое поле (ожидаемый результат - Result is FAIL).

Тестирование производилось в следующем окружении:
* ОС: Windows: 10 Домашняя, 64 -разрядная;
* Версия Java: "11.0.12" 2021-07-20.
