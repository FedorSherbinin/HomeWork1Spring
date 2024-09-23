# MavenWeb

Это простое веб-приложение, созданное с использованием Maven и Jetty. 

## Структура проекта

Проект содержит базовую настройку для веб-приложения с использованием Maven и Jetty. 

Структура проекта:
mavenweb/
├── src/
│   ├── main/
│   │   ├── resources/
│   │   └── webapp/
│   │       ├── WEB-INF/
│   │       │   ├── web.xml
│   │       │   └── classes/
│   │       └── index.jsp
├── .gitignore
├── pom.xml
└── README.md

markdown
Копировать код

## Установка

1. Убедитесь, что у вас установлены [Java](https://www.oracle.com/java/technologies/javase-downloads.html) и [Maven](https://maven.apache.org/install.html).

2. Клонируйте репозиторий:

   ```bash
   git clone https://github.com/FedorSherbinin/HomeWork1Spring.git

3. Перейдите в нужную директорию:
   
   ```bash
   cd mavenweb
   
4. Выполните команду для загрузки зависимостей и сборки проекта:

   ```bash
   mvn clean install

5. Для запуска веб-приложения с использованием Jetty выполните следующую команду:
   ```bash
   mvn jetty:run

6. Приложение будет доступно по адресу: http://localhost:8080.

#Сравнение Maven и Gradle


| Характеристика              | Maven                                          | Gradle                                        |
|-----------------------------|------------------------------------------------|-----------------------------------------------|
| **Конфигурация**            | XML, громоздко, но предсказуемо               | Groovy/Kotlin, более выразительно и гибко    |
| **Производительность**      | Каждый билд с нуля, медленно                  | Инкрементальная сборка, кэширование          |
| **Управление зависимостями**| Простой и четкий подход                       | Гибкость с конфигурациями (например, `implementation`, `compileOnly`) |
| **Расширяемость**           | Большая экосистема плагинов, сложно писать свои | Легко создавать собственные плагины, много встроенных |
| **Сообщество и поддержка**  | Зрелое сообщество, часто используется в корпорациях | Активное сообщество, привлекает внимание разработчиков |

Заключение
Gradle обладает более гибкой и мощной системой управления зависимостями и процессом сборки, чем Maven. Однако Maven может быть предпочтительным в проектах с устоявшейся структурой, где важна строгость и предсказуемость конфигурации. Gradle особенно полезен в динамичных и больших проектах, где важна скорость и удобство работы с конфигурацией.
