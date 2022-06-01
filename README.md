# GitHub Homework 2

#создаём и kлонируем внешний репозиторий git clone <copy repository HTTPS>, не забыть перейти в главную ветку

1. На локальном репозитории сделать ветки для:
#создаём и kлонируем внешний репозиторий git clone <copy repository HTTPS>, не забыть перейти в главную ветку

-Postman
```bash
git branch Postman

#or создать и сразу в неё перейти
git checkout -b Postman

#вернуться обратно на главную ветку
git checkout main
```

-Jmeter
    
```bash
git branch Jmeter
```

-CheckLists 
```bash
git branch CheckLists
```

-Bug_Reports
```bash
git branch Bug_Reports
``` 

-SQL
```bash
git branch SQL
```

-Charles
```bash
git branch Charles
``` 

-Mobile_testing
```bash
git branch Mobile_testing
```
#проверить все ли ветки создались
```
git branch
```

2. Запушить все ветки на внешний репозиторий

```bash
git push origin --all
```

3. В ветке Bug Reports сделать текстовый документ со структурой баг репорта

```bash
  git checkout Bug_Reports  --> 
  vim Bug_Reports.txt
  .
  .
  Esc
:wq

 or
 
  git checkout Bug_Reports -->
  cat > Bug_Reports.txt
  ^C
    
|ID|Version|Environment|Summary|STR|Expected Result|Actual Result|Severity|Priority|Attachments|
  
  or 
Environment:
ID:
Summary:
Steps to reproduce:
Actual Result:
Expected Result:
Attachments:
```
```
#проверить создание файла
git status
```

4. Запушить структуру багрепорта на внешний репозиторий

```bash
git add Bug_Reports.txt  -->
git commit -m "add file bug_reports"  -->
git push --set-upstream origin Bag_reports
```

5. Вмержить ветку Bug Reports в Main 

```bash
git checkout main  -->
git merge Bug_Reports
```

6. Запушить main на внешний репозиторий.

```bash
 git push
```
 
7. В ветке CheckLists набросать структуру чек листа.

```bash
git checkout CheckLists  -->
vim CheckLists.txt
.
.
Esc
:wq

or
git checkout CheckLists  -->
cat > CheckLists.txt
^C    
    
|ID|Check|Result|Comment|

 
or 

ID:
Check:
Result:
Comment:
 
```
 
8. Запушить структуру на внешний репозиторий

```bash
git add .  -->
git commit -m "add file checklis"  -->
git push origin CheckLists
```

9. На внешнем репозитории сделать Pull Request ветки CheckLists в main

#in web `Compare & pull request` :arrow_forward: `Create pull request`  :arrow_forward: `Merge pull request`  :arrow_forward: `Confirm merge` 


10. Синхронизировать Внешнюю и Локальную ветки Main

```bash
git checkout main
    
#посмотреть были ли изменения
git fetch
--> 
git pull
```
 
