# Git-Branch

1. На локальном репозитории сделать ветки для:
- Postman `git checkout -b Postman`
- Jmeter `git checkout -b Jmeter`
- CheckLists `git checkout -b Checklists `
- Bag Reports `git checkout -b Bag_Reports`
- SQL `git checkout -b SQL `
- Charles `git checkout -b Charles `
- Mobile testing `git checkout -b Mobile_testing`

2. Запушить все ветки на внешний репозиторий `git push origin --all`
3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта ` git checkout Bag_Reports`-->  `vim Bag_Reports`--> `i`
<pre>
Bug-ID: Номер
Title: Заголовок, отвечает на вопросы «Что?», «Где?», «При каких обстоятельствах?»
Project: Название проекта
STR: Точная последовательность действий, которая приводит к тому, чтобы воспроизвести баг   
Actual result: К чему приводит воспроизведение шагов, как сейчас работает программа
Expected result: ак должна работать программа на самом деле и к чему должны приводить действия,описанные в пункте «Шаги к воспроизведению»
Environment: Точная версия ПО, содержащая баг
Browser 
Severity: Параметр, который определяет влияние бага на работу программы по шкале от S0 до S4
Priority: Параметр, который определяет срочность исправления бага по шкале от P1 до PЗ
Status
Author
</pre>
<pre>Esc--> :wq </pre>
5. Запушить структуру багрепорта на внешний репозиторий  `git add . && git commit -m "bag report"` --> `git push --set-upstream origin Bag_Reports`
6. Вмержить ветку Bag Reports в Main `git checkout main` --> `git merge Bag_Reports`
7. Запушить main на внешний репозиторий. `git push`
8. В ветке CheckLists набросать структуру чек листа. `git checkout Checklists`--> `vim Checklists.txt`--> `i`
<pre>
Номер
Название:В названии отражается раздел или область в ПО, для которого сделаны проверке, например «Регистрация пользователя»
Наименование проверки: Краткое описание сути проверки
Ожидаемый результат: Сама проверка: что мы ожидаем получить. В некоторых видах чек-листов он не используется.
Результат: Прошла проверка или нет (passed/failed)
  </pre>
 <pre>Esc--> :wq </pre> 
9. Запушить структуру на внешний репозиторий ` git push --set-upstream origin Checklists`
10. На внешнем репозитории сделать Pull Request ветки CheckLists в main `Compare&pull request`
11. Синхронизировать Внешнюю и Локальную ветки Main `git checkout main`--> `git pull`
