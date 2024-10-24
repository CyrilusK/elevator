## Тестовое задание IOS
### Задача:
Разработать приложение, которое демонстрирует работу лифтов в здании. В 
этом здании может быть от 2 до 4 лифтов. На каждом этаже есть кнопки 
вызова лифта. Оптимальность выбора лифта должна определяться по 
минимальному времени ожидания. Конфигурация экрана должна загружаться и 
парситься из файла JSON. Время передвижения лифта на один этаж, количество 
этажей и информация о лифтах должны быть взяты из конфигурации 
(timeToElevate, houseLevels, lifts).
Технологии:
- Swift
- Архитектура MVP
- UIKit
- Верстка кодом

![Static Badge](https://img.shields.io/badge/Swift-5.0-orange) ![Static Badge](https://img.shields.io/badge/Xcode-14.3-blue) ![Static Badge](https://img.shields.io/badge/iOS-16.0-green)

Дополнительные задания (необязательные):
Добавить функцию открытия и закрытия дверей лифта (в конфигурации есть 
параметр timeOpenCloseDoor). Реализовать анимацию движения лифтов и 
дверей. Визуализировать очереди вызовов.

Требования:
Приложение должно отображать движение лифтов и иметь интерактивные кнопки 
для каждого этажа, которые вызывают лифт. Скорость движения лифта 
составляет 'timeToElevate' на один этаж. Приложение должно быть стабильным 
и не иметь критических ошибок, которые могут привести к его аварийному 
завершению.
JSON:
Джсон из файла «Lifts» необходимо разместить на любом сервере. Например 
можно использовать https://www.mockable.io

Инструкция:
Управлять лифтами можно с помощью кнопок, расположенных слева. При парсинге джсон стоят ограничения по количеству лифтов (до 6), количеству этажей (до 25), по наличию интернет-соединения, по количеству доступных лифтов, в противном случае появится алерт с описанием ошибки. Цвет кнопки является индикатором, синий цвет означает возможность вызова, а серый цвет - поднятие лифта на нужный этаж.
Присутствует баг - во время закрывания и открывания лифта можно вызвать его на другой этаж, есть определенная сложность с решением из-за разделения на слои, ищу решение.

![End Banner](record.gif)
