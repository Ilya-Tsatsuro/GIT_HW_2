# GIT_HW_2
![](https://ruleoftech.com/files/2019/05/simplified-git-flow.png)
## Предусловия: 
* Создаем репозиторий на вебе.
* Переходим в локальную папаку, куда будем клонировать репозиторий.
```bash
Command: cd Users/tsatsuro/Desktop/Тестирование/gitrepo/       
```
* Клонируем репозиторий, созданный на вебе.
```bash
Command: git clone git@github.com:Ilya-Tsatsuro/GIT_HW_2.git 
```
* Переходим в созданный и скопированный репозиторий.
```bash
Command: cd GIT_HW_2/ 
```
Просмотреть существующие ветки в репозитории.
```bash
Command: git branch 
```
----
## Задание
1. На локальном репозитории сделать ветки для:
- Postman
- Jmeter
- CheckLists
- Bag Reports
- SQL
- Charles
- Mobile testing

```bash
Command: git branch Postman; git branch Jmeter; git branch CheckLists; git branch Bag_Reports; git branch SQL; git branch Charles; git branch Mobile_testing 
```
```bash
Command: git branch
Result:
  Bag_Reports
  Charles
  CheckLists
  Jmeter
  Mobile_testing
  Postman
  SQL
* main
```



2.1. Запушить все ветки на внешний репозиторий.

```bash
Command: git push -u origin Postman; git push -u origin Jmeter; git push -u origin CheckLists; git push -u origin Bag_Reports; git push -u origin SQL; git push -u origin Charles; git push -u origin Mobile_testing      
```

2.2. Или
```bash
Command: git push -u origin Postman;
Command: git push -u origin Jmeter
Command: git push -u origin CheckLists
Command: git push -u origin Bag_Reports
Command: git push -u origin SQL
Command: git push -u origin Charles
Command: git push -u origin Mobile_testing
```

2.3. Результат:

![](https://github.com/Ilya-Tsatsuro/Screenshot/blob/main/HW_2_Git/8_branches.png?raw=true)

3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта.
```bash
Command: git checkout Bag_Reports
Command: cat >> BG_1.txt
    id: 
    Title:
    Precondition: 
    AR:
    ER:
    Status:
    Severity:
    Attachment:
    ^C⏎ 
```
4. Запушить структуру багрепорта на внешний репозиторий.
```bash
Command: git add BG_1.txt 
Command: git commit -m "add BG.txt  with the structure of the bug report" 
Command: git push 
```
![](https://github.com/Ilya-Tsatsuro/Screenshot/blob/main/HW_2_Git/add_BG%20in%20Bag_reports.png?raw=true)

5. Вмержить ветку Bag Reports в Main.
```bash
Command: git checkout main  
Command: git merge Bag_Reports
```
6. Запушить main на внешний репозиторий.
```bash
Command: git push 
```
![](https://github.com/Ilya-Tsatsuro/Screenshot/blob/main/HW_2_Git/push%20main%20repo.png?raw=true)

7. В ветке CheckLists набросать структуру чек листа.
```bash
Command: touch Checklist.txt
Command: vim Checklist.txt
```
8. Запушить структуру на внешний репозиторий.
```bash
Command: git add Checklist.txt
Command: git commit -m "add file Checklist.txt to Checklists branch"
Command: git push
```
9. На внешнем репозитории сделать Pull Request ветки CheckLists в main.

![](https://github.com/Ilya-Tsatsuro/Screenshot/blob/main/HW_2_Git/Compare&pull_request.png?raw=true)

----

![](https://github.com/Ilya-Tsatsuro/Screenshot/blob/main/HW_2_Git/Create_pull_request.png?raw=true)

----

![](https://github.com/Ilya-Tsatsuro/Screenshot/blob/main/HW_2_Git/Result_pull_request.png?raw=true)

----

![](https://github.com/Ilya-Tsatsuro/Screenshot/blob/main/HW_2_Git/Merge_pull_request.png?raw=true)

----

![](https://github.com/Ilya-Tsatsuro/Screenshot/blob/main/HW_2_Git/Result_merge.png?raw=true)

----

![](https://github.com/Ilya-Tsatsuro/Screenshot/blob/main/HW_2_Git/Pull%20Request%20ветки%20CheckLists%20в%20main.png?raw=true)

----

10. Синхронизировать Внешнюю и Локальную ветки Main.

```bash
Command: git checkout main    
Command: git pull 
```

Результат:
![](https://github.com/Ilya-Tsatsuro/Screenshot/blob/main/HW_2_Git/synchronizing%20repositories.png?raw=true)

-----