
������� ����� ����� 

git branch <��������_�����>
#���
git checkout -b <��������_�����>


��������� ��������� ��� �����
git checkout <��������_�����>
git push origin <��������_�����>


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
# ����������
git status

git branch          ;  ����� �������� 
git branch -r       ;  ����� remotes ( �������� ) 
---------------------------------------------------------------------------
# �������� ��������� � ������
git status

# ������������� � main � ��������� ��������� ����� main � �������
git checkout main
git pull origin main

# ������� ����� ����� fix1 � ������������� �� ���
git checkout -b fix1

# ��������� ��������� ��������� � ����� fix1
git add .
git commit -m "��������� �� fix1"

# ������� � main ��������� �� fix1 
git checkout main
git pull origin main
git merge fix1

# ���������� ���� ��������� � GitHub
git status
git push origin main
---------------------------------------------------------------------------
# ����� ����� ��������� �� ���������� ��������� ����� main
git checkout -f  main
---------------------------------------------------------------------------






