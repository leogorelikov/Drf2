
создать новую ветку 

git branch <название_ветки>
#или
git checkout -b <название_ветки>


Отправить изменения для ветки
git checkout <название_ветки>
git push origin <название_ветки>


create a new repository on the command line

echo "# Drf2" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/leogorelikov/Drf2.git
git push -u origin main

or push an existing repository from the command line

git remote add origin https://github.com/leogorelikov/Drf2.git
git branch -M main
git push -u origin main

---------------------------------------------------------------------------
# Посмотреть
git status

git branch          ;  ветки локально 
git branch -r       ;  ветки remotes ( удаленно ) 
---------------------------------------------------------------------------
# Внесение изменений в проект
git status

# Переключаемся в main и Обновляем локальную ветку main с сервера
git checkout main
git pull origin main

# Создаем новую ветку fix1 и переключаемся на нее
git checkout -b fix1

# Добавляем сделанные изменения в ветку fix1
git add .
git commit -m "изменения из fix1"

# Вливаем в main изменения из fix1 
git checkout main
git pull origin main
git merge fix1

# Отправляем наши изменения в GitHub
git status
git push origin main
---------------------------------------------------------------------------
# Откат наших изменений до локального состояния ветки main
git checkout -f  main
---------------------------------------------------------------------------






