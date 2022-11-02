# Перечень автоматизируемых сценариев
* переход к форме через вкладку "Программирование на главной странице
* переход к форме через вкладку "Каталог курсов"
* переход к форме через "Выберите вектор развития"
* переход к форме через футер
* заполнение формы
# Перечень используемых инструментов с обоснованием выбора
*Intellij IDEA* - написание и запуск тестов
*JUnit 5*
*SELENIDE* - удобная конфигурация, наличие селекторов, авто настройка WebDriver
*Allure* - наглядное представление результатов тестов и логов, возможность классифицировать дефекты
*GitHub* - контроль версий, обмен файлами с командой
*Docker* – работа с образами тестовой базы данных (если таковая будет)
*Visual Studio* – чтение кода
*JMeter* – для нагрузочного тестирования (при необходимости)
*Программа для баг-трекинга* (например, **Jira**) – при необходимости
# Перечень необходимых разрешений, данных и доступов 
* Разрешение владельца ресурса на тестирование, в том числе нагрузочного
* Согласованный тест-план
* SUT для тестирования
* Тестовая база данных для проверки получения площадкой заявок на обучение или доступ к работающей системе

# Перечень и описание возможных рисков при автоматизации 
* Несвоевременное получение данных для тестирования
* Изменение в SUT – необходимость актуализации тестов
* Отсутствие необходимого ПО
* Проблемы с «железом» и интернетом

# Перечень необходимых специалистов для автоматизации
* QA инженер, обладающий достаточными навыками и тестовой средой

# Интервальная оценка с учётом рисков в часах
* 20 часов – без учета рисков
* 40 часов – с учетом рисков
