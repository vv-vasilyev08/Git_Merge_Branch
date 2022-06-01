# Git_Merge_Branch

## GitHub. HW_2
0. Создать репозитрою на GitHub и выгрузить на локальный Git
>git_Merge_Branch
>git clone git@github.com:vv-vasilyev08/Git_Merge_Branch.git
1. На локальном репозитории сделать ветки для:
- Postman  
- Jmeter  
- CheckLists  
- Bag Reports  
- SQL  
- Charles  
- Mobile testing
>git branch  
>git branch postman  
>git branch jmeter  
>git branch checklist  
>git branch bagreports  
>git branch sql  
>git branch charles  
>git branch mobile
2. Запушить все ветки на внешний репозиторий
>git push origin postman jmeter checklist bagreports sql charles mobile
3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта
>git checkout bagreports  
>cat >> bugreport.txt  
>ID: VKS-2525  
>Author: Fintiflushka  
>Assignment: Dev007  
>Priority: Very High  
>Title: [Ошибка] Preprod. Кнопка регистрации не активна на странице регистрации  
>Environment: Preprod. Google Chrome version 110  
>Preconditions: Открыть страницу https://xyz.com , перейти в раздел регистрации  
>STR: Заполнить валидными данными поля регистрации и нажать кнопку зарегистрироваться  
>ER: Регистрация успешно выполнена и на почту пришло письмо об успешной регистрации  
>AR: Кнопка регистрации не активна после заполнения всех необходимых полей регистрации  
>Attachments: Screenshot-001.png , Screencast-001.mp4  
>CTRL+D  
>git add . && git commit -m "add bugreport"
4. Запушить структуру багрепорта на внешний репозиторий
>git push --set-upstream origin bagreports
5. Вмержить ветку Bag Reports в Main
>git checkout main  
>git merge bagreports -m "merge bugreports"
6. Запушить main на внешний репозиторий.
>git push
7. В ветке CheckLists набросать структуру чек листа.
>git checkout checklist  
>cat >> checklist.txt  
>1. Проверить запуск приложения на Preprod  
>2. Установить приложение из тестового репозитория  
>3. Удалить приложение  
>4. Установить из внутреннего-тестового маркет плейса  
>5. Удалить приложение из маркет плейса  
>CTRL+D  
>git add . && git commit -m "add checklist"
8. Запушить структуру на внешний репозиторий
>git push --set-upstream origin checklist
9. На внешнем репозитории сделать Pull Request ветки CheckLists в main
>Нажать на Pull Request в GitHub и выбрать ветки checklist в main
10. Синхронизировать Внешнюю и Локальную ветки Main
>git fetch  
>git pull
