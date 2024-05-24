# MySQL Go
## Instruction
1. docker-compose up
2. go run create_note.go
3. docker exec -it docker-mysql-db-1 mysql -uexample_user -pexample_password example_db
4. select * from example_db;
5. show tables;
6. select * from notes;
## Description
This is a simple Go application that demonstrates using GORM with MySQL to manage notes in a database.

## Prerequisites
- Go installed on your system
- MySQL database running locally or in a remote server

## Installation
1. Clone the repository to your local machine.
2. Download the necessary dependencies by running:
    ```bash
    go mod tidy
    ```
3. Update the DSN (Data Source Name) in the `main.go` file with your MySQL connection details.

## Usage
1. Run the application by executing:
    ```bash
    go run main.go
    ```
2. The application will connect to the MySQL database using the provided DSN, create a table for `Note` objects if it doesn't exist, and insert a new note into the database.

## Project Structure
- `main.go` - Contains the main application logic.
- `README.md` - Information about the project setup.
- `go.mod`, `go.sum` - Go modules files.

## Contributing
Feel free to contribute by opening issues or pull requests.

## License
This project is licensed under the [MIT License](LICENSE).




# MySQL Go

## Описание
Это простое приложение на Go, которое демонстрирует использование GORM с MySQL для управления заметками в базе данных.

## Предварительные требования
- Установленный Go на вашей системе
- База данных MySQL, запущенная локально или на удаленном сервере

## Установка
1. Склонируйте репозиторий на свой локальный компьютер.
2. Загрузите необходимые зависимости, запустив:
    ```bash
    go mod tidy
    ```
3. Обновите DSN (Data Source Name) в файле `main.go` своими данными подключения к MySQL.

## Использование
1. Запустите приложение, выполнив:
    ```bash
    go run main.go
    ```
2. Приложение подключится к базе данных MySQL с использованием предоставленного DSN, создаст таблицу для объектов `Note`, если её не существует, и добавит новую запись в базу данных.

## Структура Проекта
- `main.go` - Содержит основную логику приложения.
- `README.md` - Информация о настройке проекта.
- `go.mod`, `go.sum` - Файлы Go модулей.

## Вклад
Не стесняйтесь вносить свой вклад, создавая задачи или запросы на слияние.

## Лицензия
Этот проект лицензируется по [лицензии MIT](LICENSE).