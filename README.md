# GitHelp
<h2>Начало работы</h2>
Создание нового репозитория, первый коммит, привязка удалённого репозитория с gthub.com, отправка изменений в удалённый репозиторий.
```
git init
touch readme.md
git add readme.md
git commit -m "Первый коммит"
git remote add origin https://github.com/NikitaIT/project.git
git push origin master
```

<h2>Внесение изменений в коммит</h2>
```
mkdir inc
touch inc/index.html
git add inc/index.html
git commit -m "Отжал семки у админа"
```
Если комит неинформативен делаем рекомит
```
git add inc/index.html
git commit --amend -m "Сверстал панель админа"
```

<h2>Новая ветка</h2>
```
git checkout -b название_ветки_то_что_мы_изменяем
```
Вносим изменения в файл
```
touch inc/header.html
git commit -a -m "то_что_мы_изменяем"
```
Назад в ветку мастер
```
git checkout master
```
Сливаем ветки и удаляем слитую
```
git merge название_ветки_то_что_мы_изменяем
git branch -d название_ветки_то_что_мы_изменяем
```
<h2>Merge failed</h2>
Коммитим содержимое первой ветки из под мастера, 
затем выбераем как совместить её с мастер-веткой и коммитим.
