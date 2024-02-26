# Задание
Для Prometheus необходимо установить отдельно хранилище метрик (Victoria Metrics, Grafana Mimir, Thanos, etc.).
Во время записи метрики в хранилище Prometheus должен дополнительно добавлять лейбл site: prod.
Дополнительные параметры хранилища: Metrics retention - 2 weeks

# Решение
### docker-compose с минимально необходимыми составляющими:
- CMS
- Prometheus
- Blackbox exporter
- Thanos sidecar
- Thanos query
- Thanos compactor

### Конфигурация для экспортера:
- Проверка october-cms на 2хх
- external_labels "site: prod"

### Конфигурацию для Prometheus:
- Скрейп конфиги
