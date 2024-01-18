Написать docker-compose со всеми необходимыми составляющими:
- CMS
- Postgres
- Prometheus
- Blackbox exporter
- Postgres exporter

Написать конфиги для для экспортеров:
- Добавить необходимые модули для проверки http и tcp в blackbox exporter
- Добавить модуль авторизации в postgres exporter

Написать конфигурацию для Prometheus:
- Добавить интервалы
- Добавить скрейп конфиги, вызывающие модули из экспортеров
