# Mock Service

Управление собеседованиями, участниками и отзывами.

## 🔧 Технологии
- Java 21
- Spring Boot 2.7.11
- Spring Security + OAuth2
- PostgreSQL
- Liquibase
- Eureka Client

## 📦 Порт
9912

## 🗄️ База данных
- Имя: mock
- Пользователь: postgres
- Пароль: password

## 📚 API Endpoints

| Метод | URL | Описание |
|-------|-----|----------|
| GET | /interviews/ | Список собеседований |
| GET | /interviews/last | Последние 5 |
| GET | /interview/{id} | Детали |
| POST | /interview/ | Создать |
| PUT | /interview/ | Обновить |
| PUT | /interview/status/ | Обновить статус |
| POST | /wisher/ | Откликнуться |
| POST | /feedback/ | Оставить отзыв |
| GET | /feedback/{id} | Отзывы собеседования |
| GET | /filter/{userId} | Фильтры пользователя |

## 📄 Swagger
http://localhost:9912/swagger-ui/index.html

## 🔗 Eureka
Регистрируется под именем mock

## 🚀 Запуск
```bash
mvn spring-boot:run