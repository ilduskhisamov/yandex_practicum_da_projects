# Проект по анализу поведения пользователей мобильного приложения

## Ссылки: [ipynb](https://github.com/ilduskhisamov/Portfolio/blob/149c0943a7e64b04ac926b2be6225fa638f1a7b5/project_mobile_app/mobile_app_project.ipynb) [html](https://github.com/ilduskhisamov/Portfolio/blob/149c0943a7e64b04ac926b2be6225fa638f1a7b5/project_mobile_app/mobile_app_project.html)

## Навыки и инструменты:
Python:
- pandas
- numpy
- scipy
- math
- datetime
- matplotlib
- seaborn
- plotly

Анализ бизнес показателей:
- Событийная аналитика
- Когортный анализ
- Юнит экономика
- Продуктовые метрики

## Описание проекта
В приложении пользователи продают свои ненужные вещи, размещая их на доске объявлений.
Заказчиком является продакт менеджер, который занимается вовлеченностью пользователей.
Основной целью исследования является получение на основе поведения пользователей гипотезы о том как можно было бы улучшить приложение с точки зрения пользовательского опыта.
Для начала нужно разбить пользователей на отдельные сегменты по поведению и выделить основные сценарии (последовательности событий) использования приложения.
В дальнейшем заказчик будет проводить свои исследования на основе нашей сегментации.

## Ход исследования:
В данном проекте были проделана следующая работа:
- Загрузка данных и изучение общей информации;
- Выполнена предобработка данных;
- Созданы функции для удобства расчетов;
- Исследовательский анализ данных: описана и визуализирована общая информация о пользователях (профили пользователей, расчет и визуализация Retention Rate);
- В разрезе сессий отобраны основные сценарии\паттерны, которые приводят к целевому действие и также построены по ним воронки;
- Рассчитана относительная частота событий в разрезе двух групп пользователей (достигших/не достигших целевого действия): выявлены разницы между данными группами в **совершенных действиях**, **датами совершения действий** и **источниками которыми они пользовались**
- Проверены статистические гипотезы:
1. О различии конверсии в целевое действие между двумя группами (прошедшими/не прошедшими по рекомендациям приложения) - в данном случае использовался z-test, т.к. нужно было сравненить две доли между группами.
2. О различии медианной длительности сессии между двумя группам (достигших/не достигших целевого действия) - для сравнения медианной длительности между группами я использовал непараметрический тест Уилкоксона-Манна-Уитни.
- Общий вывод и рекомендации: резюмирование полученных результатов, формулировка ключевых выводов и рекомендаций.

## Общий вывод
В данном анализе были найдены и рассмотрены самые популярные сценарии с конечным целевым действием. По ним были построены воронки, расчитаны CR(от действия к действию) и RR(для каждого действия). Анализ сценарий показал, что рекомендательная система приложения работает не лучшим образом и стоит её доработать.
Были проверены нужные для бизнеса статистические гипотезы, благодаря которым в моих рекомендациях стало ещё больше аргументов.
Весь список моих рекомендаций можно увидеть в самом проекте.

С помощью данного исследования я стремился дать всестороннний анализ пользователей мобильного приложения, что стало отправной точкой для дальнейшего развития приложения.
