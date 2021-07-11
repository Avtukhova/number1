# Отчёт о тестировании Credit Card Number Validator


## Краткое описание

10.07.2021 - 11.07.2021 было проведено тестирование чек-листа для приложения Credit Card Number Validator.


На тестирование затрачено: 4 часа

В результате тестирования выявлены следующие дефекты:
* <ссылка на описание дефекта>
* <ссылка на описание дефекта>
* <ссылка на описание дефекта>

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты*:
* Карты Visa
* Карты MasterCard
* Карты Maestro
* Карты Visa Electron
* Карты American Express 
* Карты Discover
* Карты JCB
* Карты Diners Club - North America
* Карты Diners Club - Carte Blanche
* Карты Diners Club - International
* Карты InstaPayment
* Нижняя граница поля
* Данные в виде букв
* Данные в виде тех.символов
* Пустое поле
  

В качестве тестовых данных использовались данные freeformatter.com:
* Visa: 4929384533061618 - Result is "OK";
* Visa: 4485641025011930535 - Result is "OK";
* MasterCard: 5584980920676919 - Result is "OK";
* Maestro: 6763695266880096 - Result is "OK";
* Visa Electron: 4913528270260605 - Result is "OK";
* American Express: 340137441397766 - Result is "OK";
* Discover: 6011007453388422 - Result is "OK";
* Discover: 6011050562876631085 - Result is "OK";
* JCB: 3532194671580431 - Result is "OK";
* JCB: 3536497195815437395 - Result is "OK";
* Diners Club - North America: 5561645496172661 - Result is "OK";
* Diners Club - Carte Blanche: 30391644535756  - Result is "OK";
* Diners Club - International: 36413905323997 - Result is "OK";
* InstaPayment: 6383367812382890 - Result is "OK";
* Нижняя граница поля: 4 - Result is "FAIL";
* Данные в виде букв: ввпарвdsrrrrrrrr - Result is "FAIL";
* Данные в виде тех.символов: $$$####***&&&&&& - Result is "FAIL";
* Пустое поле: Result is "FAIL"

Тестирование производилось в следующем окружении:
* Windows 7, 64-разрядная ОС
* Java version "1.8.0_291"
