# remote-test-1

Создайте удалённый репозиторий remote-test-1 с файлом README.md
Склонируйте его на свой рабочий стол командой git clone
Посмотрите связи с удалённым репозиторием командой git remote -v
Создайте новый пустой удалённый репозиторий remote-test-2
Удалите связь с текущим репозиторием: git remote remove origin
Подключите свой локальный репозиторий к новому удалённому:
git remote add origin path
Отправьте изменения в новый удалённый репозиторий:
git push -u origin master

Создаём связь с исходным репозиторием: git remote add source path
Просматриваем связи и убеждаемся, что все установились: git remote -v
Вносим изменения в локальный код и отправляем в оба репозитория:
git push -u origin master
git push -u source master
Просматриваем изменения в удалённых репозиториях
Вносим в удалённых репозиториях изменения в разные файлы
Затягиваем изменения: git fetch --all
Просматриваем их:
git log origin/master ^master
git log source/master ^master
Вливаем их:
git merge origin/master
git merge source/master