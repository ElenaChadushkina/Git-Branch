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
4. Запушить структуру багрепорта на внешний репозиторий  `git add . && git commit -m "bag report"` --> `git push --set-upstream origin Bag_Reports`
5. Вмержить ветку Bag Reports в Main `git checkout main` --> `git merge Bag_Reports`
6. Запушить main на внешний репозиторий. `git push`
7. В ветке CheckLists набросать структуру чек листа. `git checkout Checklists`--> `vim Checklists.txt`
8. Запушить структуру на внешний репозиторий ` git push --set-upstream origin Checklists`
9. На внешнем репозитории сделать Pull Request ветки CheckLists в main `Compare&pull request`
10. Синхронизировать Внешнюю и Локальную ветки Main `git checkout main`--> `git pull`
