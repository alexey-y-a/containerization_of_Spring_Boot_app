# 💥Контейнеризация Spring Boot-приложения

## Техническое задание
- Собрать JAR-файл локально (например, через Maven или Gradle).
- Базовый образ — openjdk:21-jdk
- Скопировать JAR-файл app.jar в контейнер (например, в директорию /app).
- EXPOSE 8080 — это стандартный порт Spring Boot, если вы не переопределяете его.
- CMD или ENTRYPOINT — запустить ваш JAR-файл командой java -jar /app/app.jar.
- Итог: При запуске контейнера с пробросом порта (например, -p 8080:8080),
 при переходе на http://localhost:8080 вы должны увидеть ответ сервиса 
 (например, Hello from Spring Boot!).

