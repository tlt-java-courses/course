{% include header.md %}

{% include important-news.md %}

Введение в платформу Java
=====

Материалы для самоподготовки
---------------------

### Основные материалы - Java Fundamentals
1. [Видео: Learn - Java Fundamentals](https://learn.epam.com/detailsPage?id=2dc581e5-a788-4737-9730-183dfef41e5f){:target="_blank"} (только раздел GETTING STARTED)
1. [Habr: Инструменты для запуска и разработки Java приложений, компиляция, выполнение на JVM](https://habr.com/ru/post/471772/){:target="_blank"}
1. [Видео: Введение в Java](https://www.youtube.com/watch?v=iK97P8DQeOU){:target="_blank"}

### Дополнительные материалы - Java Fundamentals
1. [W3S: Как поставить Java локально](https://www.w3schools.com/java/java_getstarted.asp){:target="_blank"}
1. [Горячие клавиши в Intelliji Idea](./Intelliji_idea_shortcuts.pdf){:target="_blank"}
1. [Java Google Codestyle](https://google.github.io/styleguide/javaguide.html){:target="_blank"}

Практическая работа
---------------------
1. Установите **[JDK 1.8+](https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html){:target="_blank"}** себе 
на рабочую машину (крайне рекомендуется вначале использовать версию **1.8**, позже можно будет перейти на более новую версию).
2. Убедитесь, что переменная окружения `JAVA_HOME` прописана верно, путь до `bin` добавлен в переменную окружения `path` и вы можете из консоли вызывать команды JDK, например `java -version`. 
3. Установите IDE (редактор кода). Рекомендуем использовать **[Intelliji Idea](https://www.jetbrains.com/idea/)** (бесплатной версии "Community Edition" вполне достаточно).
4. Создайте свое первое приложение "Hello World". Используйте следующий пример **[Создание первого приложения]({{site.materialsurl}}java_intro/hello-world-tutorial)**, выполните все пункты.
5. Запустите, убедитесь, что программа выполняется корректно, пройдитесь по всем шагам из примера.
6. Обязательно попрактикуйтесь работать с приложением в режиме Debug.
7. Запуште получивщуюся программу в специально созданный удаленный репозиторий.
8. Закройте цель и подцели, укажите в комментарий ссылку на репозиторий.

Вопросы для самоконтроля
---------------------
{% include questions/java_intro_questions.md %}