Тестовое задание
=================

уточнения/заметки по ТЗ, тестовые сценарии и отчеты в соответствующих .rst файлах
(к примеру заметки_по_ТЗ_фронт.rst  и тд.)

что не оформлено/реализовано отмечено как TODO и реализуется по аналогии

----

выполнение UI автотестов (с учетом, что уже запущен сервис https://github.com/imhio-ltd/tester_test_task ):

  ::

    cd autotests
    docker-compose up -d --build
    docker-compose run --rm tests bash
    cd front/ && pytest

| "интерактивные" алюр отчеты: http://127.0.0.1:4040
| vnc к автотестовому браузеру vnc://127.0.0.1:5900

----

сгенерированный (для примера) отчет автотестов:

  ::

    cd autotests/allure-report/
    python -m http.server 8080

в браузере 127.0.0.1:8080
