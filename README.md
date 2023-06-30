# GitHub

GitHub HW2

1. На локальном репозитории сделать ветки для:	

	-Postman
	-Jmeter
	-CheckList
	-Bug Report
	-SQL
	-Charles
	-Mobile testing
		
		* На веб интерфейсе сайта github.com (под своим аккаунтом) создаём репозиторий GitHub
		* Копируем HTTPS ссылку на репозиторий
		* На локальной машине создаем папку в которую будем клонировать репозиторий и переходим в нее	
		* Запускаем Git Bash в папке и выполняем следующие команды:
			- git branch Postman
			- git branch Jmeter
			- git branch CheckList
			- git branch Bug_Report
			- git branch SQL
			- git branch Charles
			- git branch Mobile_Testing

2. Запушить все ветки на внешний репозиторий 

	- git push -u origin Postman
	- git push -u origin Jmeter
	- git push -u origin CheckList
	- git push -u origin Bug_Report
	- git push -u origin SQL
	- git push -u origin Charles
	- git push -u origin Mobile_Testing

3. В ветке Bug Reports сделать текстовый документ со структурой баг репорта

	- git checkout Bug_Report
	- cat > bugreport.txt
	- Заполняем файл и сохраняем
 
4. Запушить структуру багрепорта на внешний репозиторий

	- git add bugreport.txt
	- git commit -m "Add file bugreport.txt to Bug_Report branch"
	- git push
	- На удаленном репозитории в веб интерфейсе появится уведомление о недавних пушах. Нажимаем "Compare & pull request"
	- Веб форма предложит оставить коментарий, нажимаем "Create pull request", проходит проверка на конфликты с основной 	веткой. Если конфликтов нет - нажимаем "Merge pull request" и "Confirm merge" 

5. Вмержить ветку Bug Report в Main

	- git checkout main
	- git merge Bug_Report

6. Запушить Main на внешний репозиторий 
	
	- git fetch
	- git pull
	- git push -u origin main

7. В ветке CheckList набросать структуру чек листа

	- git checkout CheckList
	- cat > checklist.txt
	- Заполняем файл и сохраняем
	
8. Запушить структуру на внешний репозиторий

	- git add checklist.txt
	- git status (опционально, перепровериться)
	- git commit -m "Add checklist.txt file"
	- git push  
9. На внешнем репозитории сделать Pull Request ветки CheckList в Main

	- На удаленном репозитории в веб интерфейсе появится уведомление о недавних пушах. Нажимаем "Compare & pull request"
	- Веб форма предложит оставить коментарий, нажимаем "Create pull request", проходит проверка на конфликты с основной 	веткой. Если конфликтов нет - нажимаем "Merge pull request" и "Confirm merge"

10. Синхронизировать Внешнюю и Локальную ветки Main

	- git status
	- git fetch
	- git pull
