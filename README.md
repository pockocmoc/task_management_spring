# Task Manager API

API для управления задачами в Task Manager.

## Работа с API

### Получение списка всех задач

**URL:** /tasks

**Метод:** GET

**Описание:** Получение списка всех задач.

**Ответ:**

- Код 200 OK
- Список задач в формате JSON

### Получение задачи по идентификатору

**URL:** /tasks/{id}

**Метод:** GET

**Описание:** Получение задачи по ее идентификатору.

**Параметры:**

- id - идентификатор задачи

**Ответ:**

- Код 200 OK
- Задача с указанным идентификатором в формате JSON

### Создание новой задачи

**URL:** /tasks/add

**Метод:** POST

**Описание:** Создание новой задачи.

**Тело запроса:** 

- Новая задача в формате JSON

**Ответ:**

- Код 200 OK
- Созданная задача в формате JSON

### Получение списка задач по статусу

**URL:** /tasks/status/{status}

**Метод:** GET

**Описание:** Получение списка задач по их статусу.

**Параметры:**

- status - статус задачи (возможные значения: TODO, IN_PROGRESS, DONE)

**Ответ:**

- Код 200 OK
- Список задач с указанным статусом в формате JSON

### Обновление статуса задачи

**URL:** /tasks/update/{id}

**Метод:** PUT

**Описание:** Обновление статуса задачи.

**Параметры:**

- id - идентификатор задачи

**Тело запроса:**

- Обновленная задача в формате JSON

**Ответ:**

- Код 200 OK
- Обновленная задача в формате JSON

### Удаление задачи по идентификатору

**URL:** /tasks/delete/{id}

**Метод:** DELETE

**Описание:** Удаление задачи по ее идентификатору.

**Параметры:**

- id - идентификатор задачи

**Ответ:**

- Код 200 OK
