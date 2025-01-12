﻿# Это репозиторий для обучения pull request

## Первые шаги

1. Делаем fork репозитория, в которой потом хотим сделать pull request. Ищем кнопку Fork на странице репозитория <https://git@github.com:gulden-geekbrains/version_control.git>
2. Выполняем команду клонирования из своей fork-копии
```sh
git clone git@github.com:*YOURE_GITHUB*/version_control.git
```
3. Создаем новую ветку и вносим необходимые изменения в файл
```sh
git checkout -b updatereadme
vim README.md
git add README.md
git commit -m "Добавили инструкцию как создать pull request"
```
4. Делаем push  
```sh
git push --set-upstream origin updatereadme
```
5. Переходим на свою страницу репозитория. Выбираем ветку **updatereadme** и жмем кнопку **Compare & pull request**

## Заметки

Что бы сделать push от другого пользователя необходимо выполнить команду
```sh
GIT_SSH_COMMAND='ssh -i ~/.ssh/user-private-key -o IdentitiesOnly=yes' git push git@github.com:gulden-geekbrains/version_control.git
```

вместо *user-private-key* подставьте свой ключ

Можно прописать настройки для подсоединения по ssh
```sh
git config remote.origin.url git@github.com:gitusername/reponame
git config core.sshCommand "ssh -i ~/.ssh/user-private-key -o IdentitiesOnly=yes"
```
# Как подружить git с github под Windows 10

Вот видео инструкция https://youtu.be/E8cIjbJMEpE

1. **Подготовьте репозиторий для работы**:
   - Создайте новый репозиторий на GitHub, в котором будет находиться файл с инструкцией по работе с Git.
   - Добавьте README.md файл в ваш репозиторий, в котором будет содержаться начальная инструкция по работе с Git.

2. **Напишите инструкцию по работе с Git**:
   - Откройте файл README.md и начните писать инструкцию по работе с Git. Напишите о команде git init, git add, git commit, git status и других основных командах.
   - Добавьте информацию о создании веток, слиянии веток, отмене изменений и другие полезные команды.

3. **Дополните инструкцию информацией о работе с удаленными репозиториями**:
   - Добавьте раздел в инструкцию, где будет описано клонирование удаленного репозитория, добавление удаленных репозиториев, отправка изменений на удаленный репозиторий и т.д.

4. **Создайте pull request**:
   - Перейдите на страницу [репозитория преподавателя](https://github.com/gulden-geekbrains/version_control) и нажмите кнопку "Pull request".
   - Укажите ваш репозиторий и ветку, в которой находится ваш файл с дополненной инструкцией.
   - Опишите в pull request, что вы добавили информацию о работе с удаленными репозиториями.

5. **Подгрузите скриншоты**:
   - Сделайте скриншот отправленного pull request.
   - Сделайте скриншот самой инструкции с добавленной информацией о работе с удаленными репозиториями.

6. **Отправьте скриншоты и ссылку на ваш репозиторий**:
   - После выполнения всех шагов отправьте скриншоты и ссылку на ваш репозиторий преподавателю.


