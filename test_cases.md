# Тест-кейсы для импорта облака точек.

## Тест-кейс 1: Импорт mgu_1.las
- **Описание**: Проверка успешного импорта файла `mgu_1.las`.
- **Предусловия**: Файл `mgu_1.las` доступен для импорта.
- **Шаги**:
  1. Перейти во вкладку "Облака точек".
  2. Выбрать команду "Импорта облака точек".![image](https://github.com/user-attachments/assets/8fe52627-83fe-4b00-b609-35ed8e6e2c23)
  3. Импортировать файл `mgu_1.las`.
- **Ожидаемый результат**: Облако точек отображается корректно.
- **Фактический результат**: Успешно, данные корректны.
- **Статус**: Пройден.

## Тест-кейс 2: Импорт mgu_2.las
- **Описание**: Проверка успешного импорта файла `mgu_2.las`.
- **Предусловия**: Файл `mgu_2.las` доступен для импорта.
- **Шаги**:
  1. Перейти во вкладку "Облака точек".
  2. Выбрать команду "Импорта облака точек".![image](https://github.com/user-attachments/assets/203f413c-1eb8-406c-8981-f31dc165a2fd)
  3. Импортировать файл `mgu_2.las`.
- **Ожидаемый результат**: Облако точек отображается корректно.
- **Фактический результат**: Успешно, данные корректны.
- **Статус**: Пройден.

## Тест-кейс 3: Импорт mgu_1.las, mgu_2.las
- **Описание**: Проверка успешного импорта файла mgu_1.las, mgu_2.las.
- **Предусловия**: Файлы `mgu_1.las`, `mgu_2.las` доступны для импорта.
- **Шаги**:
  1. Перейти во вкладку "Облака точек".
  2. Выбрать команду "Импорта облака точек".![image](https://github.com/user-attachments/assets/203f413c-1eb8-406c-8981-f31dc165a2fd)
  3. Импортировать файлы `mgu_1.las`, `mgu_2.las`.
- **Ожидаемый результат**: Облака точек отображается корректно.
- **Фактический результат**: Успешно, данные корректны.
- **Статус**: Пройден.
  
## Тест-кейс 4: Импорт mgu_1.las
- **Описание**: Проверка успешного импорта файла mgu_1.las.
- **Предусловия**: Файл mgu_1.las доступен для импорта.
- **Шаги**:
  1. Перейти в консоль.
  2. Прописать команду `NPC_IMPORT`.
  3. Импортировать файл mgu_1.las.
- **Ожидаемый результат**: Облако точек отображается корректно.
- **Фактический результат**: Успешно, данные корректны.
- **Статус**: Пройден.

  ## Тест-кейс 5: Импорт mgu_2.las
- **Описание**: Проверка успешного импорта файла mgu_2.las.
- **Предусловия**: Файл mgu_2.las доступен для импорта.
- **Шаги**:
  1. Перейти в консоль.
  2. Прописать команду `NPC_IMPORT`.
  3. Импортировать файл mgu_2.las.
- **Ожидаемый результат**: Облако точек отображается корректно.
- **Фактический результат**: Успешно, данные корректны.
- **Статус**: Пройден.

# Группа тест-кейсов: Регистрация по парам соответствующих точек.

## Тест-кейс 6.1: Успешная сшивка - три пары точек, минимальное расхождение.

- **Описание:** Проверка успешной попарной сшивки с минимальным расхождением между тремя парами точек.
- **Предусловия:**
    * Облака точек `mgu_1.las` и `mgu_2.las` успешно импортированы. 
    * Выбрана команда `PC_REGISTRATION_MANUAL`.![image](https://github.com/user-attachments/assets/951bda09-fa54-422e-a685-f4d419b83841)
- **Шаги:**
    1. Указать базовое облако (`mgu_1.las`).
    2. Указать вторичное облако (`mgu_2.las`).
    3. Указать три пары соответствующих точек с минимальным расхождением.![image](https://github.com/user-attachments/assets/4f0d4302-9091-4178-9beb-05ee0f607635)
    4. Нажать "Решение"![image](https://github.com/user-attachments/assets/adaca255-a506-40e1-963b-a9312f6965b2) (пробное выравнивание). Проверить значения невязки.
    5. Нажать "Применить преобразование".
- **Ожидаемый результат:** Сшивка выполнена успешно, облака корректно совмещены, минимальное расхождение между точками.
- **Фактический результат:** Сшивка выполнена успешно, облака корректно совмещены, минимальное расхождение между точками.
- **Статус:** Пройден.


## Тест-кейс 6.2: Успешная сшивка - пять пар точек, среднее расхождение.

- **Описание:** Проверка успешной попарной сшивки с умеренным расхождением между пятью парами точек.
- **Предусловия:** Облака точек `mgu_1.las` и `mgu_2.las` успешно импортированы. Команда `PC_REGISTRATION_MANUAL` выбрана.![image](https://github.com/user-attachments/assets/725628cf-b2e0-4252-b412-ae05b6710b96)
- **Шаги:**  Как в 6.1, но с пятью парами точек, имеющих умеренное расхождение.![image](https://github.com/user-attachments/assets/6da6546f-3ca1-42e4-b53f-f1f7196e4673)
- **Ожидаемый результат:** Сшивка выполнена успешно, облака корректно совмещены, умеренное расхождение между точками. 
- **Фактический результат:** Сшивка выполнена успешно, облака корректно совмещены, умеренное расхождение между точками. 
- **Статус:** Пройден.


## Тест-кейс 6.3: Нет возможности совмещения при двух точках совмещения.

* **Описание:** Проверка обработки ситуации с недостаточным количеством точек.
* **Предусловия:** Облака точек `mgu_1.las` и `mgu_2.las` успешно импортированы. Команда `PC_REGISTRATION_MANUAL` выбрана.
* **Шаги:** Как в 6.1, но с двумя парами точек.![image](https://github.com/user-attachments/assets/840b37d5-6029-43a5-b5c9-549b77372305)
* **Ожидаемый результат:** Функция "Применить совмещение" не активна.
* **Фактический результат:** Функция "Применить совмещение" не активна.
* **Статус:** Пройден.

## Тест-кейс 6.5: Удаление точек.

* **Описание:** Проверка функционала удаления точек после добавления.
* **Предусловия:** Облака точек `mgu_1.las` и `mgu_2.las` успешно импортированы. Команда `PC_REGISTRATION_MANUAL` выбрана.![image](https://github.com/user-attachments/assets/2976641a-5ee5-4a15-abb1-6f73dba4783d)
* **Шаги:**
    1. Выполнить шаги 6.1, добавив четыре пары точек.![image](https://github.com/user-attachments/assets/ad3a0958-97df-42e8-a797-0c3374b27407)
    2. Удалить одну пару точек.![image](https://github.com/user-attachments/assets/db5574eb-498e-4181-ba0c-14f8382ff4ef)
    3. Нажать "Решение"![image](https://github.com/user-attachments/assets/adaca255-a506-40e1-963b-a9312f6965b2) (пробное выравнивание). Проверить значения невязки.
    4. Нажать "Применить преобразование".
* **Ожидаемый результат:** Удаленная точка удалена из таблицы, сшивка выполнена корректно с учетом оставшихся точек.
* **Фактический результат:** Удаленная точка удалена из таблицы, сшивка выполнена корректно с учетом оставшихся точек.
* **Статус:** Пройден.


## Тест-кейс 6.6: Изменение положения маркера

- **Описание:** Проверка функционала изменения положения маркера.
- **Предусловия:** Облака точек `mgu_1.las` и `mgu_2.las` успешно импортированы. Команда `PC_REGISTRATION_MANUAL` выбрана.![image](https://github.com/user-attachments/assets/09ae08e0-e81c-4fb3-b630-b1df044d1d46)
- **Шаги:**
    1. Выполнить шаги 6.1, добавив две пары точек.
    2. Изменить положение одного маркера.![image](https://github.com/user-attachments/assets/25b21910-9d7e-4757-9ec7-8bdcc4535782)
    3. Нажать "Решение"![image](https://github.com/user-attachments/assets/adaca255-a506-40e1-963b-a9312f6965b2) (пробное выравнивание). Проверить значения невязки.
    4. Нажать "Применить преобразование".
- **Ожидаемый результат:** Положение маркера изменено, сшивка выполнена корректно с учетом нового положения маркера.
- **Фактический результат:** Положение маркера изменено, сшивка выполнена корректно с учетом нового положения маркера.
- **Статус:** Пройден.
