# Attendence_server_project

Проект на языке C#

### 1. Название проекта: Attendence_server_project

### 2. Список студентов:
* Тютюльников Михаил Андреевич - 19144
* Носоерев Константин Алексеевич - 19144
### 3. Проблема, которую решает проект.
* В настоящий момент имеется приложение, работающее с сервером НГУ. В рамках расширения возможностей использования приложения вне НГУ необходимо дополнить проект приложения проектом сервера для него.
### 4. Основные компоненты системы:
* Хост (сервер для обработки запросов, хранения данных, взаимодействие с пользователем)
### 5. Описание точек расширения:
* Добавление личного кабинета преподавателя/студента
* Формирование отчетов по посещаемости
* Формирование электронной зачетки 

### Основные сценарии
* Сценарий 0
  - Пользователь приложения входит в свой аккаунт, после чего с сервера получаются данные пользователя.
 
Далее сценарии разбиты по группе к которой относится пользователь
* Сценарий "Студент"
  - Пользователь получает с сервера свой уникальный идентификатор, которые затем при помощи BLE раздается.

* Сценарий "Преподаватель"
  - Пользователь получает с сервера список своих дисциплин.
  - Выбрав дисциплину, пользователь получает список "студентов" в виде (ФИО - уникальный идентификатор)
  - После BLE сканирования окружающих пользователя идентификаторов формируется список присутствующих студентов.
  - После добавления (в случае необходимости) "студентов" вручную, список отправляется на сервер с указанием дополнительных параметров (например, время занятия)
