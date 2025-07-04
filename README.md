# Kafka + Zookeeper + Redpanda Console (Kowl) Docker Compose

Минимальная конфигурация для локальной разработки с Apache Kafka, включающая:

- **Apache Kafka** (на базе Bitnami образа)
- **Zookeeper** (необходим для управления Kafka-кластером)
- **Redpanda Console** (ранее Kowl - веб-интерфейс для управления Kafka)

## Особенности конфигурации

- Использует официальные Bitnami образы (Apache-лицензия)
- Автоматическое создание топиков при первом обращении
- Healthcheck для корректного порядка запуска сервисов
- Готов к работе в Docker-сети (внутренняя маршрутизация по именам сервисов)
- Внешний доступ через `localhost:9092` (Kafka) и `localhost:8080` (Web UI)

## Быстрый старт

1. Запустите стек:
```bash
docker-compose up
