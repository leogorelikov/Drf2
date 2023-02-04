
создать новую ветку 

git branch <название_ветки>
#или
git checkout -b <название_ветки>


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