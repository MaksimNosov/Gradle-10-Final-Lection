# **План автоматизации тестирования** сценария перехода и заполнения формы записи на профессию *Тестировщик ПО* на сайте [Link](https://netology.ru/)

## Перечень автоматизируемых сценариев

### Сценарии навигации к форме
1. ***переход к форме через вкладку "Программирование на главной странице"***
* пролистнуть страницу до блока "Направления обучения"
* кликнуть на блоке "Программирование"
* пролистнуть страницу до блока "Тестировщик ПО"
* кликнуть по нему
* кликнуть на кнопку "Записаться" или прокрутить страницу до формы записи

2. ***переход к форме через вкладку "Каталог курсов"***
* кликнуть по кнопке "Каталог курсов"
* навести курсор на блок "Программирование", не нажимая на него
* в поле справа кликнуть по "Тестировщик ПО"
* кликнуть на кнопку "Записаться" или прокрутить страницу до формы записи

3. ***переход к форме через блок "Выберите вектор развития"***
* пролистнуть страницу до блока "Выберите вектор развития"
* кликнуть кнопку "Выбрать курс"
* пролистнуть страницу до блока "Тестировщик ПО"
* кликнуть по нему
* кликнуть на кнопку "Записаться" или прокрутить страницу до формы записи

4. ***переход к форме через футер***
* пролистнуть страницу до футера
* в футере кликнуть по кнопке "Программирование"
* пролистнуть страницу до блока "Тестировщик ПО"
* кликнуть по нему
* кликнуть на кнопку "Записаться" или прокрутить страницу до формы записи

### Сценарии заполнения и отправки формы
***Входные данные*** - *осуществлен переход к форме записи любым доступным способом*

1. ***Заполнение и отправка формы с валидными данными***
* заполнение поля "Имя" (например, "Иван")
* заполнение поля "Телефон" (например, "+7(999)999-99-99")
* клик по кнопке "Записаться"

*Ожидаемый результат: форма успешно отправилась, появилось соответствующее уведомление*

2. ***Заполнение и отправка формы с невалидными данными (невалидное имя)***
* заполнение поля "Имя" невалидным значением (например, "564,")
* заполнение поля "Телефон" (например, +7(999)999-99-99)
* клик по кнопке "Записаться"

*Ожидаемый результат: форма не отправляется, под полем "Имя" сообщение об ошибке "Должно состоять из букв*

3. ***Заполнение и отправка формы с невалидными данными (невалидный телефон)***
* заполнение поля "Имя" валидным значением (например, "Иван")
* заполнение поля "Телефон" невалидным значением (например, "666")
* клик по кнопке "Записаться"

*Ожидаемый результат: форма не отправляется, под полем "Телефон" сообщение об ошибке "Номер в формате +9(999)999-99-99"*

4. ***Заполнение и отправка формы с невалидными данными (пустое имя)***
* заполнение поля "Телефон" валидным значением (например, +7(999)999-99-99)
* клик по кнопке "Записаться"

*Ожидаемый результат: форма не отправляется, под полем "Имя" сообщение об ошибке "Обязательное поле"*

5. ***Заполнение и отправка формы с невалидными данными (пустой телефон)***
* заполнение поля "Имя" валидным значением (например, "Иван")
* клик по кнопке "Записаться"

*Ожидаемый результат: форма не отправляется, под полем "Телефон" сообщение об ошибке "Обязательное поле"*


## Перечень используемых инструментов с обоснованием выбора

* *Java* - язык программирования
* *Intellij IDEA Ultimate* - написание и запуск тестов
* *JUnit 5*
* *SELENIDE* - удобная конфигурация, наличие селекторов, авто настройка WebDriver
* *GitHub* - контроль версий, обмен файлами с командой
* *Docker* – работа с образами тестовой базы данных (если таковая будет)
* *Visual Studio* – чтение кода
* *JMeter* – для нагрузочного тестирования (при необходимости)
* *Программа для баг-трекинга* (например, **Jira**) – при необходимости

## Перечень необходимых разрешений, данных и доступов 

* Разрешение владельца ресурса на тестирование, в том числе нагрузочного
* Согласованный тест-план
* SUT для тестирования
* Тестовая база данных для проверки получения площадкой заявок на обучение или доступ к работающей системе

## Перечень и описание возможных рисков при автоматизации 

* Несвоевременное получение данных для тестирования
* Изменение в SUT – необходимость актуализации тестов
* Отсутствие необходимого ПО
* Проблемы с «железом» и интернетом

## Перечень необходимых специалистов для автоматизации

* QA инженер, обладающий достаточными навыками и тестовой средой

## Интервальная оценка с учётом рисков в часах

* 20 часов – без учета рисков
* 40 часов – с учетом рисков
