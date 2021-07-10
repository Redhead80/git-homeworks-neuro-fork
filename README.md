#  Домашнее задание к лекции «Командная работа»

## Задача №1 - Конфликт при push'е

### Легенда

Вы с коллегой вдвоём работаете над функцией определения геолокации посетителя лендинга NeuroStartUp. Вы сделали ряд изменений и пытатесь запушить их в репозиторий. Но в этот момент выясняется, что ваш коллега тоже не сидел без дела и успел запушить свои изменения раньше вас. Вам необходимо разрешить кофликт и залить свои изменения на GitHub. 

### Задача

1. Сделайте форк репозитория [по ссылке](https://github.com/netology-code/git-homeworks-neuro-fork);
2. Скачайте [архив изменений](https://github.com/netology-code/git-homeworks/blob/master/remote/src/neuro-push.zip);
3. Свяжите локальный репозиторий из архива с форком репозитория из п.1;
4. Выполните команду `push -u origin master`, удостоверьтесь, что конфликт произошёл;
5. Заберите актуальную версию данных из удалённого репозитория при помощи команды `git pull origin master`;
6. Разрешите появившийся конфликт и отправьте сделанные вами изменения на GitHub.

### Решение

1. Сделал форк репозитория [по ссылке](https://github.com/netology-code/git-homeworks-neuro-fork) на github'е; 
2. Скачал [архив изменений](https://github.com/netology-code/git-homeworks/blob/master/remote/src/neuro-push.zip) по умолчанию в папку загрузки;
3. Распаковал архив, переименовал в  Repo_for_Push_3.1 чтобы небыло пробелов а то gitbash ругается;
4. Запустил gitbash, командой 'cd Repo_for_Push_3.1' перешёл в данный репозиторий;
5. Связал локальный репозиторий Repo_for_Push_3.1 с форком репозитория git-homeworks-neuro-fork на github'е командой 'git remote add git-homeworks-neuro-fork https://github.com/Redhead80/git-homeworks-neuro-fork.git' (git запрашивал Логин и Пароль);
6. Выполнил команду git push --set-upstream git-homeworks-neuro-fork master, соответственно произошёл конфликт);
7. Выполнил команду git pull  git-homeworks-neuro-fork master, gitbash указал на конфликт: CONFLICT (add/add): Merge conflict in js/app.js;
8. Открыл файл app.js программой VS Code, подредактировал этот файл (VS Code решает эту проблему автоматически, что очень удобно.) Сохранил файл;
9. Отправил сделанные изменения в удалённый репозиторий на github командой git push  git-homeworks-neuro-fork master.
10. Отправил ссылку на этот репозитрий в дз

