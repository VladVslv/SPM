**Определение основных процессов и функций управления проектом согласно PMBOK и ScrumBOK для проекта «Сервис интеграции дополнительных источников документов в Поиск Яндекс Маркета»**

---

### **Шаги проекта**

**Аналитика:**

- Обучение модели **Userbody KNN**
- Обучение модели **Mixigen**

**Разработка:**

- Разработка кода для переноса исходного источника
- Поднятие сервиса
- Настройка доставки данных
- Разработка кода для использования моделей в сервисе
- Интеграция сервиса кандидатогенерации в Поиск

---

## **Управление проектом согласно PMBOK**

**Группы процессов:**

1. **Инициация**
2. **Планирование**
3. **Исполнение**
4. **Мониторинг и контроль**
5. **Завершение**

**Области знаний:**

1. Управление интеграцией проекта
2. Управление содержанием проекта
3. Управление расписанием проекта
4. Управление стоимостью проекта
5. Управление качеством проекта
6. Управление ресурсами проекта
7. Управление коммуникациями проекта
8. Управление рисками проекта
9. Управление закупками проекта
10. Управление заинтересованными сторонами проекта

### **Применение PMBOK к проекту**

**Инициация:**

- Определение целей проекта
- Идентификация заинтересованных сторон

**Планирование:**

- Разработка плана управления проектом
- Определение объема работ, расписания и бюджета
- Планирование ресурсов, качества, рисков и коммуникаций

**Исполнение:**

- Обучение моделей
- Разработка кода и сервисов
- Интеграция сервиса в Поиск

**Мониторинг и контроль:**

- Отслеживание прогресса
- Контроль качества и управления рисками
- Управление изменениями

**Завершение:**

- Финальное тестирование и внедрение
- Документирование результатов
- Официальное закрытие проекта

### **Схема процессов PMBOK**

```mermaid
graph TD
    Start[Инициация] --> Planning[Планирование]
    Planning --> Execution[Исполнение]
    Execution --> Monitoring[Мониторинг и контроль]
    Monitoring --> Execution
    Monitoring --> Planning
    Execution --> Closing[Завершение]
```
---

## **Управление проектом согласно ScrumBOK**

**Основные компоненты Scrum:**

- **Роли:**
  - **Product Owner**
  - **Scrum Master**
  - **Development Team**

- **События:**
  - **Sprint**
  - **Sprint Planning**
  - **Daily Scrum**
  - **Sprint Review**
  - **Sprint Retrospective**

- **Артефакты:**
  - **Product Backlog**
  - **Sprint Backlog**
  - **Increment**

### **Применение Scrum к проекту**

**Инициация:**

- Назначение ролей
- Создание **Product Backlog** с задачами проекта

**Спринты:**

```mermaid
graph TD
    A[Инициация] --> B[Спринт 1]
    B --> C[Спринт 2]
    C --> D[Спринт 3]
    D --> E[Спринт 4]
    E --> F[Релиз]

    subgraph Спринт 1
        B1[Планирование]
        B2[Работа над задачами]
        B3[Обзор и ретроспектива]
        B1 --> B2 --> B3
    end
    subgraph Спринт 2
        C1[Планирование]
        C2[Работа над задачами]
        C3[Обзор и ретроспектива]
        C1 --> C2 --> C3
    end
    subgraph Спринт 3
        D1[Планирование]
        D2[Работа над задачами]
        D3[Обзор и ретроспектива]
        D1 --> D2 --> D3
    end
    subgraph Спринт 4
        E1[Планирование]
        E2[Работа над задачами]
        E3[Обзор и ретроспектива]
        E1 --> E2 --> E3
    end
```

**Разбиение задач по спринтам:**

- **Спринт 1:**
  - Обучение модели **Userbody KNN**
  - Разработка кода для переноса источника

- **Спринт 2:**
  - Обучение модели **Mixigen**
  - Поднятие сервиса

- **Спринт 3:**
  - Настройка доставки данных
  - Разработка кода для использования **Userbody KNN** в сервисе

- **Спринт 4:**
  - Разработка кода для **Mixigen**
  - Интеграция сервиса в Поиск

---

## **Функции управления проектом**

### **В PMBOK:**

- **Управление интеграцией**
- **Управление содержанием**
- **Управление расписанием**
- **Управление стоимостью**
- **Управление качеством**
- **Управление ресурсами**
- **Управление коммуникациями**
- **Управление рисками**
- **Управление закупками**
- **Управление заинтересованными сторонами**

### **В Scrum:**

- **Управление бэклогом продукта**
- **Планирование спринтов**
- **Ежедневные Scrum-встречи**
- **Обзор и ретроспектива**
- **Управление качеством и рисками через итерации**

---

## **Интегрированная схема управления проектом**

```mermaid
graph LR
    Initiation["Инициация (PMBOK)"] --> Planning["Планирование (PMBOK)"]
    Planning --> Sprint1["Спринт 1 (Scrum)"]
    Sprint1 --> Sprint2["Спринт 2 (Scrum)"]
    Sprint2 --> Sprint3["Спринт 3 (Scrum)"]
    Sprint3 --> Sprint4["Спринт 4 (Scrum)"]
    Sprint4 --> Closing["Завершение (PMBOK)"]

    subgraph "Мониторинг и контроль (PMBOK)"
        M[Мониторинг спринтов]
    end

    Sprint1 --> M
    Sprint2 --> M
    Sprint3 --> M
    Sprint4 --> M
```