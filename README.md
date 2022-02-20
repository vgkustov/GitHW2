1. На локальном репозитории сделать ветки для:
- Postman
- Jmeter
- CheckLists
- Bug Reports
- SQL
- Charles
- Mobile testing  

> Локально:  
>> mkdir GitHW2 && cd GitHW2   
>> git init - определяем GitHW2 как локальный репозторий  
>> git branch Postman - создаем ветку Postman. Остальные – аналогично. 

2. Запушить все ветки на внешний репозиторий  

> На GitHub:
>> New repository -> Name: GitHW2 -> Create repository 

> Локально:  
>> git remote add origin https://github.com/vgkustov/GitHW2.git - связываем локальный репозиторий с внешним  
>> git push -u origin main - пушим ветку main  
>> git push --all - пушим все остальные ветки  

3. В ветке Bug Reports сделать текстовый документ со структурой баг репорта  

> git switch Bug_Reports - Переключаемся в ветку switch работает как checkout  
> vim bugreport.txt - составляем багрепорт

4. Запушить структуру багрепорта на внешний репозиторий  

> git add bugreport.txt - добавляем в отслеживание для гита
> git commit -m "add bugreport.txt" - коммитим
> git push - отправляем на внешний репозиторий

5. Вмержить ветку Bug Reports в Main

> git switch main  
> git merge Bug_preports - мержим ветку.  

7. Запушить main на внешний репозиторий.

> git push

9. В ветке CheckLists набросать структуру чек листа.

> git switch Checklists  
> vim checklist.txt - заполняем чеклист.  
> git add . && git commit -m "message"  

11. Запушить структуру на внешний репозиторий

> git push

12. На внешнем репозитории сделать Pull Request ветки CheckLists в main

> "new pull request" -> add description -> "Create pull request"  
>  Merge pull request

13. Синхронизировать Внешнюю и Локальную ветки Main

> git pull
