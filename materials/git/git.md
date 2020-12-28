{% include header.md %}

{% include important-news.md %}

Системы контроля версий - Git
=====

Материалы для самоподготовки
---------------------
### Основные материалы - Git
1. [Видео: Learn - Version control with GIT](https://learn.epam.com/detailsPage?id=601f195a-d408-4439-a16d-0630ed2a412e){:target="_blank"}
1. [Книга: Pro Git](https://git-scm.com/book/ru/v2){:target="_blank"} (1, 2, 3, 5 главы обязательны для изучения)
1. [Habr: Удачная модель ветвления для Git](https://habr.com/ru/post/106912/){:target="_blank"}

### Дополнительные материалы - Git
1. [Приложение для тренировки навыков работы в GIT](https://learngitbranching.js.org/){:target="_blank"}

Практическая работа
---------------------
1. Создайте учетную запись на **[Github](https://github.com/){:target="_blank"}**.  
Все последующие практические работы нужно будет сохранять в этой учётной записи, в других репозиториях.

2. Установите и настройте **[git](https://git-scm.com/downloads)** и клиент для него.  
Варианты клиентов:
* [SourceTree](https://www.sourcetreeapp.com/){:target="_blank"}
* [Tortoise GIT](https://tortoisegit.org/){:target="_blank"}
* [Плагин в IntellijiIdea](https://plugins.jetbrains.com/plugin/3033-git-integration){:target="_blank"}
* [GitKraken](https://www.gitkraken.com/){:target="_blank"}
* [SmartGit](http://www.syntevo.com/smartgit/){:target="_blank"}

3. Создайте новый репозиторий в своем аккаунте на Github и склонируйте его себе на рабочую машину.

4. Выполните **все** следующие операции в любом удобном вам порядке:
* commit
* create new branch (создайте несколько дополнительных веток)
* merge (без конфликтов слияния)
* merge (с конфликтами слияния)
* push
* pull (можете внести изменения в файлы через сайт Github и затем спуллить изменения)
* pull с конфликтами слияния (для этого нужно изменить одну и ту же строчку в файле в локальном репозитории и в репозитории на Github, после чего сделать pull)
* rebase
* revert
* tags (создайте несколько тегов, проверьте что они будут запушены на Github)
* stash 
* cherry-pick
* reset

5. Удостоверьтесь, что вы действительно поняли смысл каждой команды и логику ее работы.
5. Запуште итоговый результат всех изменений в ваш центральный репозиторий на Github.  
6. Закройте цель и подцели, укажите в комментарий ссылку на репозиторий.

Вопросы для самоконтроля
---------------------
{% include questions/git_questions.md %}