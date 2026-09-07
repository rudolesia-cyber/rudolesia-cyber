# Контракты API вложений ОКТУС

Публичные описания выпуска **1.2** для защиты итогового проекта: обмен файлами по заявкам между ОКТУС и внешними сервисными компаниями (ВСК).

Это **аддитивное** расширение действующего контракта задач `v1.1`. Старые методы продолжают работать.

| Файл | Что внутри |
|---|---|
| [contracts/open-api-oktus-attachments-v1.2.yaml](contracts/open-api-oktus-attachments-v1.2.yaml) | OpenAPI 3.0: загрузка, временная ссылка на скачивание, удаление |
| [contracts/asyncapi-oktus-attachments.yaml](contracts/asyncapi-oktus-attachments.yaml) | AsyncAPI 2.6: события ПАРУС ↔ ОКТУС, топики COMMONTASKCHANGEDUPDATE; вложения — необязательный attachments[] |
| [open-api-oktus_2026_08_26.yaml](open-api-oktus_2026_08_26.yaml) | Базовый контракт задач v1.1 |

Просмотр в браузере:

- [Swagger UI — OpenAPI 1.2](https://rudolesia-cyber.github.io/rudolesia-cyber/swagger.html)
- [Swagger Editor](https://editor.swagger.io/?url=https://raw.githubusercontent.com/rudolesia-cyber/rudolesia-cyber/main/contracts/open-api-oktus-attachments-v1.2.yaml)
- [AsyncAPI Studio](https://studio.asyncapi.com/?url=https://raw.githubusercontent.com/rudolesia-cyber/rudolesia-cyber/main/contracts/asyncapi-oktus-attachments.yaml)

Swagger умеет OpenAPI. События смотрите в AsyncAPI Studio, не в Swagger.

Скачивание файла ВСК — по временной ссылке ФИР (HTTP GET, TTL 15 мин). Загрузка — JSON + base64 через шлюз и антивирус. Отказ валидации SOWA — 403.
