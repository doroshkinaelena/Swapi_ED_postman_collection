# Swapi_ED_postman_collection
📌 Основные задачи и реализация (Features)
Коллекция swapi_hw_ED включает в себя следующие этапы тестирования:

1. Настройка окружения (Configuration)
Переменные коллекции: Создана и используется переменная base_url для хранения адреса сервиса.

Динамические данные: Реализована переменная dark_side для передачи данных между запросами.

2. Тестирование эндпоинтов (API Endpoints)
Получение списка всех доступных эндпоинтов и персонажей.

Работа с параметрами запроса (Query Params): пагинация (page=5) и выбор формата ответа (format=wookiee).

3. Автоматизированные тесты и скрипты (Scripts & Tests)
В коллекции реализованы следующие проверки на языке JavaScript:

Валидация успешных ответов (Request "Find ObiWan"):

Проверка статус-кода (200 OK).

Проверка времени отклика (Response time < 300ms).

Валидация данных в теле ответа (проверка пола персонажа).

Обработка ошибок (Request "Get invalid Person"):

Проверка корректности возврата ошибки 404 при некорректном ID.

Проверка наличия сообщения "Not found" в тексте ответа.

Сценарии передачи данных:

Запрос к 44-му персонажу с автоматическим сохранением его имени в переменную dark_side через вкладку Tests.

Последующий поиск персонажа по имени, используя сохраненную переменную.

🛠 Технологический стек
Postman (Collection Runner)

JavaScript (Postman API для скриптов)

REST API

🚀 Инструкция по запуску
Импортируйте файл swapi_hw_ED.postman_collection.json в Postman.
Убедитесь, что переменная base_url установлена на https://swapi.dev/api.
Запустите коллекцию через Collection Runner, чтобы увидеть результаты всех автоматизированных тестов.



SWAPI (Star Wars API) Testing Project
This repository contains a Postman collection designed to test the REST API of the Star Wars database (SWAPI). The project demonstrates proficiency in API request construction, automated assertions, and dynamic data handling.

📌 Implementation Details
The swapi_hw_ED collection covers the following testing aspects:

1. Environment & Variables
Collection Variables: Implemented a base_url variable to ensure request flexibility and easy environment switching.

Dynamic Data Chaining: Developed a script to extract character data (ID 44) and automatically store the name in a dark_side collection variable for use in subsequent requests.

2. Endpoint Testing & Parameters
Resource Retrieval: Comprehensive testing of endpoints for characters and general service metadata.

Query Parameters: Implemented and tested pagination (page=5) and specific data formats (Wookiee dialect).

3. Automated Tests (JavaScript)
The collection includes automated scripts in the Tests tab to validate API behavior:

Positive Scenarios (e.g., "Find ObiWan"):

Status Code: Asserts that the response is 200 OK.

Performance: Validates that the response time is within the acceptable threshold (< 300ms).

Data Integrity: Checks for specific character attributes (e.g., gender validation).

Negative Scenarios (e.g., "Get invalid Person"):

Error Handling: Verifies that the system returns a 404 Not Found status for non-existent IDs.

Error Messaging: Asserts that the response body contains the correct "Not found" error message.

🛠 Tech Stack
Postman (Collection Runner & Scripts)

JavaScript (Postman Sandbox API)

REST API / JSON

🚀 How to Run
Import the swapi_hw_ED.postman_collection.json file into your Postman workspace.

Ensure the base_url variable is set to https://swapi.dev/api.

Run the collection using the Postman Runner to view the automated test results.

Убедитесь, что переменная base_url установлена на https://swapi.dev/api.

Запустите коллекцию через Collection Runner, чтобы увидеть результаты всех автоматизированных тестов.
