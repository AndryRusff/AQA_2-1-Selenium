## Статус сборки [![Build status](https://ci.appveyor.com/api/projects/status/2ym70o5uh165sfd0?svg=true)](https://ci.appveyor.com/project/AndryRusff/aqa-2-1-selenium-e43t4)
# Тестирование веб-интерфейсов
## Домашнее задание по курсу "Автоматизированное тестирование"
## Тема: «2.1. Тестирование веб-интерфейсов», задание «Заказ карты»
### Задача
Необходимо автоматизировать тестирование формы заказа доставки карты.

Требования к содержимому полей:
1. Поле фамилия и имя - разрешены только русские буквы, дефисы и пробелы.
2. Поле телефон - только цифры (11 цифр), символ + (на первом месте).
3. Флажок согласия должен быть выставлен.
			
### Что сделано:
- Применены инструменты:
	- Selenium;
	- WebDriverManager.
- Тестируемая функциональность:
	1. Отправка формы, если все поля заполнены корректно, то появляется сообщение об успешно отправленной заявке.
	1. Валидация полей перед отправкой, если какое-то поле не заполнено или заполнено неверно, то при нажатии на кнопку "Продолжить" должны появляться сообщения об ошибке (будет подсвечено только первое неправильно заполненное поле).

### Предварительные требования
- На компьютере пользователя должна быть установлена Intellij IDEA
### Установка и запуск
1. Склонировать проект на свой компьютер
	- открыть терминал Intellij IDEA
	- ввести команду git clone https://github.com/AndryRusff/AQA_2-1-Selenium/
1. Открыть склонированный проект 
1. В  перейти во вкладку Terminal (Alt+F12) и запустить SUT командой java -jar artifacts/app-order.jar
1. Запустить авто-тесты в новой вкладке Terminal командой ./gradlew clean test
