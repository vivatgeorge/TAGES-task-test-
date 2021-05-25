## Курсовой проект по дисциплине "Проектирование информационных систем"

## ФИО, ИДБ-17-06

### 1. Определение требований к модели [✋](https://github.com/stankin/design-part-2/wiki/LR-1)

**Тема ВКР:** Разработка интеллектуальной информационной системы обработки сообщений пользователей для мессенджера Telegram

**Объект исследований:** системы электронно-информационных коммуникаций.

**Предмет исследований:** средства мгновенного обмена сообщениями.

**Процессы верхнего уровня:** [✋](https://github.com/stankin/design-part-2/wiki/sem1)
* **А1 ** Управлять коммуникациями.
* **А2 ** Подготовить коммуникации.
* **А3 ** Провести коммуникации.
* **А4 ** Оценить качество коммуникаций.
* **А5 ** Выявить проблемы.

**Точка зрения:** Проректор универсистета.

**Цель моделирования:** Определение автоматизируемых функций.

### 2. Функциональное моделирование процессов (IDEF0) [✋](https://github.com/stankin/design-part-2/wiki/LR-1)

* A-0 (контекстная диаграмма)

![A-0](https://github.com/vivatgeorge/nikitin/blob/main/01_A-0.jpg
)

* A0 (диаграмма верхнего уровня)

![A0](https://github.com/vivatgeorge/nikitin/blob/main/02_A0.jpg)

* A2 (декомпозиция процесса/процессов внутренней среды)

![A2](https://github.com/vivatgeorge/nikitin/blob/main/04_A2.jpg)

* A3 (декомпозиция процесса/процессов внутренней среды)

![A3](https://github.com/vivatgeorge/nikitin/blob/main/05_A3.jpg)

* A4 (декомпозиция процесса/процессов внутренней среды)

![A4](https://github.com/vivatgeorge/nikitin/blob/main/08_A4.jpg)





### 3. Функциональное моделирование программных и информационных средств (DFD) [✋](https://github.com/stankin/design-part-2/wiki/LR-2)

**Конфигурация технических средств:** Рабочие станции (ПК).

**Конфигурация программных средств:** Многоуровневые.

**Допустимые виды хранилищ и их размещение:** Почтовый сервер, сервер Amazon AWS, запоминающее устройство ПК.

* A32 Автоматизация процесса А32

![A32](https://github.com/vivatgeorge/nikitin/blob/main/06_A32.jpg)

* A33 Автоматизация процесса А33

![A33](https://github.com/vivatgeorge/nikitin/blob/main/07_A33.jpg)

### 4. Описание выбранного процесса [✋](https://github.com/stankin/design-part-2/wiki/LR-3) в формате прецедента (Use Case) [✋](https://github.com/stankin/design-part-2/wiki/LR-4)

Диаграмма UML Use Case
![p4](http://www.plantuml.com/plantuml/png/ZP11JlCm48NtFeNbVHT_smFqAbRgdqOaCNASFKaN4GA1E07Y1Y5gr53KdE7DZR1hXP05WaIQqSoyJyypcznAOuiqOVbrdDr88rEUwan7EwDJnQqf54lKVykjvYQ-sbc-ZOsARAmpncHajU42BnZmGGyukjoYeGgThyMNu1a3LUAxdcgdQWHpNv6hIEQA-_2FozmBw1O3UXpHkdn0JnN76GsLL5r6xpZHNipGPK33M_PKeq7dC2enkF-Dxj3XZ1xT75i5x9LgxqBtQFy8hYU_0qxEyt7qf9AU16C_dOKl5c5NTec-30VwbLYoiEX4X3JELsmwxTIRQzOppTZRg6nRfCad)

**4.1 Идентификатор прецедента:** А33

**4.2 Название прецедента:** Отправка сообщения пользователям Telegram

**4.3 Контекст:** А3

**4.4 Участники (actors) и цели (goals):**

| Участник  | Категория  | Цель (goal) |
|---|---|---|
| <роль> | Основной  | <основная цель для роли> |
| <роль> | Внешний  | <основная внешняя цель> |
| <наименование> | Инструмент| <основная функция инструмента> |

**4.5 Предусловия (pre-conditions):**

* <условие наличия потока управления>

* <условие наличия входного потока>

* <условие наличия потока исполнителя>

* <условие наличия потока механизма>

**4.6 Постусловия (post-conditions):**

* <выходной поток>

**4.7 Основной поток выполнения (main flow)**:

| Участник  | Действие (activity)  | Ожидаемый результат |
|---|---|---|
| <роль> | <действие> | <результат с указанием его места размещения> |

**4.8 Исключения (exceptions):**

| Условие (риск) | Последствия | Реакция |
|---|---|---|
| <описание риска> | <описание последствий> | <описание потока сообщений о проблемах> |

**4.9 Альтернативы (alternates):**

| Участник  | Действие (activity)  | Ожидаемый результат |
|---|---|---|
| <роль> | <действие> | <результат с указанием его места размещения> |

**4.10 Временные параметры:**

* **Триггер (событие, стартующее прецедент):** <управляющий поток>

* **Номинальная частота повторения прецедента:** <n раз в смену/сутки/месяц/квартал/год...>

* **Продолжительность прецедента:** <n нормочасов>

### 5. Описание структуры объекта [✋](https://github.com/stankin/design-part-2/wiki/LR-3) в формате ERD (Class) [✋](https://github.com/stankin/design-part-2/wiki/LR-5)

* **Описываемый объект:** <программа, модуль, сообщение, база данных...>

* **Диаграмма UML Class:**
![p5](http://www.plantuml.com/plantuml/proxy?idx=0&src=https://raw.githubusercontent.com/<user/user.github.io/master/<path><file>)

### 6. Описание алгоритма [✋](https://github.com/stankin/design-part-2/wiki/LR-3) в формате UML (Sequence) [✋](https://github.com/stankin/design-part-2/wiki/LR-6)

* **Описываемые процессы и потоки данных:** ???

* **Диаграмма UML Sequence:**
![p6](http://www.plantuml.com/plantuml/proxy?idx=0&src=https://raw.githubusercontent.com/<user/user.github.io/master/<path><file>)

### 7. Описание состава [✋](https://github.com/stankin/design-part-2/wiki/LR-3) в формате UML (Component) [✋](https://github.com/stankin/design-part-2/wiki/LR-7)

* **Описываемый объект:** <комплект поставки>

* **Диаграмма UML Component:**
![p7](http://www.plantuml.com/plantuml/proxy?idx=0&src=https://raw.githubusercontent.com/<user/user.github.io/master/<path><file>)

### 8. Демонстрация реализации (личная страница)

<ссылка или скриншоты>

### 9. Подготовка к интерпретации построенных моделей

**9.1 Используемые паттерны проектирования и разработки [✋](https://github.com/stankin/design-part-2/wiki/sem2):**

**9.1.1 Процессная модель для сравнения:**

**9.1.2 Используемые в разработке паттерны и фреймворки:**

**9.2 Используемые паттерны выявления проблем [✋](https://github.com/stankin/design-part-2/wiki/sem3):**
* Муда: <муда>
* Мура: <мура>
* Мури: <мури>

**9.3 Возможные антипаттерны [✋](https://github.com/stankin/design-part-2/wiki/sem4):**

| Категория  | Антипаттерн (риск) | Действие по избежанию |
|---|---|---|
| Разработка | <антипаттерн> | <действие> |
| Архитектура | <антипаттерн> | <действие> |
| Организация | <антипаттерн> | <действие> |
| Среда | <антипаттерн> | <действие> |

### 10. Интерпретация построенных моделей [✋](https://github.com/stankin/design-part-2/wiki/cp-guide)

**10.1 Определение числовых показателей для поставленной цели моделирования:**

**10.2 Определение числовых показателей для цели потенциального проекта автоматизации: [✋](https://github.com/stankin/design-part-2/wiki/interpret_process)**

**10.3 Расчет потенциального эффекта от автоматизации:**

**10.4 Определение числовых показателей и расчет затрат на реализацию проекта автоматизации:**

**10.5 План-факт сравнение для затрат на реализацию: [💻](https://docs.google.com/spreadsheets/d/11KghKnPycU-EtbHJ3dKK5FQjPntsd9ZQ9LVSzg9Ou5E/edit#gid=1983994942)**

**ВЫВОДЫ**

