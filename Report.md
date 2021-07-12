# Отчёт о тестировании Credit Card Number Validator


## Краткое описание

10.07.2021 - 11.07.2021 было проведено тестирование чек-листа для приложения Credit Card Number Validator.


На тестирование (включая подготовку и описание) затрачено: 4 часа

В результате тестирования выявлены следующие дефекты:

* [Признание невалидными действительных 19-значных карт Visa, Discover, JCB](https://github.com/Avtukhova/number1/issues/1)
* [Признание невалидными действительных карт American Express](https://github.com/Avtukhova/number1/issues/2)
* [Признание невалидными действительных карт Diners Club - Carte Blanche](https://github.com/Avtukhova/number1/issues/3)
* [Признание невалидными действительных карт Diners Club - International](https://github.com/Avtukhova/number1/issues/4)
* [Отсутствие сообщений об ошибке при вводе граничных значений поля карты](https://github.com/Avtukhova/number1/issues/5)
* [Отсутствие сообщений об ошибке при вводе тех.символов в поле карты](https://github.com/Avtukhova/number1/issues/6)
* [Отсутствие сообщения об ошибке при отправке пустого поля карты](https://github.com/Avtukhova/number1/issues/7)


## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты*:
* [Подтверждение валидности действительных карт (кейсы А1-А14)](https://docs.google.com/spreadsheets/d/1NijXGhQb4M6VwtWZYAYUPOWVGUHQz6RwjFXJuVYwSPI/edit?usp=sharing)
* [Проверка граничных значений (кейс А15)](https://docs.google.com/spreadsheets/d/1NijXGhQb4M6VwtWZYAYUPOWVGUHQz6RwjFXJuVYwSPI/edit?usp=sharing)
* [Проверка особых условий (кейсы А17, А18)](https://docs.google.com/spreadsheets/d/1NijXGhQb4M6VwtWZYAYUPOWVGUHQz6RwjFXJuVYwSPI/edit?usp=sharing)


В качестве тестовых данных использовались данные freeformatter.com:
* Visa: 4929384533061618 - Result is "OK";
* Visa: 4532131566441723 - Result is "OK";
* Visa: 4485566207259751 - Result is "OK";
* Visa: 4485641025011930535 - Result is "OK";
* Visa: 4539314511056139272 - Result is "OK";
* Visa: 4716125740644639773 - Result is "OK";
* MasterCard: 5584980920676919 - Result is "OK";
* MasterCard: 5483813139035589 - Result is "OK";
* MasterCard: 2221006932178938 - Result is "OK";
* Maestro: 6763695266880096 - Result is "OK";
* Maestro: 6304671100541034 - Result is "OK";
* Maestro: 5893953153506034 - Result is "OK";
* Visa Electron: 4913528270260605 - Result is "OK";
* Visa Electron: 4913281834231536 - Result is "OK";
* Visa Electron: 4508268670964974 - Result is "OK";
* American Express: 340137441397766 - Result is "OK";
* American Express: 342255277173354 - Result is "OK";
* American Express: 343981382263116 - Result is "OK";
* Discover: 6011007453388422 - Result is "OK";
* Discover: 6011412598873132 - Result is "OK";
* Discover: 6011833990395772 - Result is "OK";
* Discover: 6011050562876631085 - Result is "OK";
* Discover: 6011225058607822424 - Result is "OK";
* Discover: 6011343414181434630 - Result is "OK";
* JCB: 3532194671580431 - Result is "OK";
* JCB: 3536052923854085 - Result is "OK";
* JCB: 3536287606261428 - Result is "OK";
* JCB: 3536497195815437395 - Result is "OK";
* JCB: 3544909009139133257 - Result is "OK";
* JCB: 3533427006721668191 - Result is "OK";
* Diners Club - North America: 5561645496172661 - Result is "OK";
* Diners Club - North America: 5529471812555906 - Result is "OK";
* Diners Club - North America: 5484948769505250 - Result is "OK";
* Diners Club - Carte Blanche: 30391644535756 - Result is "OK";
* Diners Club - Carte Blanche: 30586186363729 - Result is "OK";
* Diners Club - Carte Blanche: 30257053093449 - Result is "OK";
* Diners Club - International: 36413905323997 - Result is "OK";
* Diners Club - International: 36791074143506 - Result is "OK";
* Diners Club - International: 36344574835294 - Result is "OK";
* InstaPayment: 6383367812382890 - Result is "OK";
* InstaPayment: 6388232763937180 - Result is "OK";
* InstaPayment: 6383142978961385 - Result is "OK".

Тестирование производилось в следующем окружении:
* Windows 7, 64-разрядная ОС
* Java version "1.8.0_291"
