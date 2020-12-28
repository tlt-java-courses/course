{% include header.md %}

{% include important-news.md %}

Введение в сборщик проектов Maven
===

Материалы для самоподготовки
---------------------
### Основные материалы
1. [Курс на Learn](https://learn.epam.com/detailsPage?id=2d408aa1-18c7-4da9-bed0-9ee229431c80){:target="_blank"}

### Дополнительные материалы
1. [Видео: Ant и Maven](https://www.youtube.com/watch?v=ouUuT2uEuiU){:target="_blank"}
1. [Jenkov: Maven](http://tutorials.jenkov.com/maven/maven-tutorial.html){:target="_blank"}
1. [Документация Мавена](https://www.apache-maven.ru/){:target="_blank"}
1. [Туториалы по Мавену](https://proselyte.net/tutorials/maven/){:target="_blank"}

Практическая работа
---------------------
1. Скачайте и поставьте Maven себе на рабочую машину. Добавьте директорию в переменную PATH. Выполните в конслои команду
`mvn -version`, чтобы удостовериться, что вы все сделали правильно.
1. Создайте новый мавен проект. В качестве groupId используйте связку `ru.фамилия.имя`, artifactId задайт как `maven-practice`.
Убедитесь, что структура проекта сответствует предыдущим практическим работам.  
1. Добавьте плагин для компиляции java и установите уровень языка `1.8`. 
1. В секции зависимостей добавьте `commons-lang`, из группы зависимостей `apache`. На сайте `mvn central` подберите 
наибольшую версию для этой зависимости. В Main попробуйте вызвать какую-нибудь функцию из этой библиотеки, например 
`org.apache.commons.text.WordUtils.capitalize(text)`.
1. Выполните фазу мавена под названием `package`. Проверьте наличие и содержание папки `target` в директории проекта.
1. Добавьте плагин в `pom.xml`
    ```xml
        <plugin>
            <artifactId>maven-assembly-plugin</artifactId>
            <configuration>
                <archive>
                    <manifest>
                        <mainClass>...</mainClass> <!-- Объявляем наш Main Class -->
                    </manifest>
                </archive>
                <descriptorRefs>
                    <descriptorRef>jar-with-dependencies</descriptorRef>  <!-- Объявляем имя для jar -->
                </descriptorRefs>
            </configuration>
            <executions>
                <execution>
                    <id>make-assembly</id>
                    <phase>package</phase> <!-- Привязываем выполнение к конкретной фазе мавена -->
                    <goals>
                        <goal>single</goal>
                    </goals>
                </execution>
            </executions>
        </plugin>
    ```
1. Выполните команду `mvn clean package`
1. Откройте получившийся архив `...-1.0-SNAPSHOT-jar-with-dependencies.jar` Проверьте наличие там пакетов из группы 
`org.apache.commons`.
1. Выполните команду `mvn clean install`. В чем её отличие от предыдущей?
1. Добавьте в ваш pom.xml `Maven Javadoc Plugin`. Добавьте джавадок к методу Main и выполните `javadoc:javadoc`. Проверьте
успешность выполнения плагина

Вопросы для самоконтроля
---------------------
{% include questions/maven_questions.md %}
