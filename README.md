### Без названия
В данном репозитории представлено общение двух микросервисов через кафку. Producer парсит и отправляет файл.xml либо отправляет заданный параметр в определенный ключ из файла.xml, Consumer принимает сообщение и, если пришел файл.xml, то распарсивает его и записывает в БД, если пришел параметр, то просто записывает его, если пришел формат JSON, то распрасивает JSON и записывает данные пары ключ-значение в отдельную связанную таблицу.
<br />
Использовалась локальная БД H2.
<br />
Для работы скачивайте проект -> ```mvn clean install -DskipTests``` -> ```mvn spring-boot:run```.
<br /> Чтобы пользоваться заполнить файлы application.properties своими данными.
