# Финальный проект по курсу Тестировщик-автоматизатор на Python (QAP)
Данный репозиторий содержит вымученный пример тестирования сайта https://www.labirint.ru/ с использованием паттерна PageObject с Selenium и Python (PyTest + Selenium).
За основу взят шаблон, предоставленный в учебном курсе Тимуром Нурлыгаяновым. Огромная ему за это благодарность.
Файлы base.py, elements.py и conftest.py были взяты практически без изменений. 
Тесты сопровождаются описанием и комментариями на русском языке.

Для работы тестов необходимо предварительно установить следующие библиотеки (pip install):

pytest;

pytest-selenium;

selenium;

termcolor;

allure-python-commons;

Драйвер chromedriver.exe для Chrome Selenium находится в корневой папке проекта.

Файлы:

pages/base.py содержит реализацию шаблона PageObject для Python.

pages/elements.py содержит вспомогательный класс для определения веб-элементов на веб-страницах.

pages/labirint.py содержит локаторы элементов сайта, используемых при тестировании. 

tests/test_labirint.py содержит тесты главной страницы сайта онлайн-магазина "Лабиринт" (https://www.labirint.ru/). Запуск теста: python -m pytest -v --driver Chrome --driver-path chromedriver.exe tests

tests_param/test_parametr_office.py содержит тесты ссылок раздела 'Канцелярские товары' сайта labirint.ru с использованием параметризации.  Запуск теста: python -m pytest -v --driver Chrome --driver-path chromedriver.exe test_param





