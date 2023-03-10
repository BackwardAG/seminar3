# Instruction on Git

Git это программа для ...

Точка в начале имени в системах (посикс) = скрытая папка

(init commit

)

## Создание репозитория

для того, чтобы создать (**инициальзировать**) новый репозиторий в текущей папке используется команда:

    git init

## Проверка состояниярепозитория

Для того, чтобы проверить в каком состоянии репозиторий, нужно выполнить команду:

    git status

## Добавление изменений к отслеживанию

Для того, чтобы добавить изменения к отследиванию (в "индекс") нужно выполнить команду:

    git add <filename>
  

## Фиксирование добавленных изменений

Для того, чтобы зафиксировать изменения добавленные ранее, нужно выполнить команду: 

    git commit

## Фиксирование изменений с коментарием о них

Для того, чтобы зафиксировать изменения добавленные ранее и добавить комментарий, нужно выполнить команду: 

    git commit -m

## Добавление и фиксирование всех изменений 

Для того, чтобы добавить и зафиксировать все изменения, используем команду:

    git commit -a

## Добавление и фиксирование всех изменений с комментарием 

Для того, чтобы добавить и зафиксировать все изменения и оставить комментарий, используем команду:

    git commit -am

## Посметреть последние зафиксированные изменения хронологически с их полными хеш-суммами

Для того, чтобы посмотреть последние фиксации изменений в текущем состоянии репозитория, необходимо ввести команду:

    git log

Внимание: для выхода из состояния просмотра терминала, нажмите клавишу "q"

## Посмотреть список зафиксированных изменений в упрошенном формате

Для того, чтобы посмотреть список зафиксированных изменений в текущем состоянии репозитория, в упрошенном виде необходимо ввести команду:    

    git log --oneline

## Отображение всех фиксаций в любом случае

Для того, чтобы посмотреть все фиксации на даннй момент безотносительно состояния репозитория в котором вы находитесь, необходимо ввести команду:

    git log --oneline --all

## Возвращение в последнее зафиксированное состояние

Чтобы переместиться в последнее зафиксированное состояние, введите команду:

    git checkout main

внимание - вместо main у вас может быть master, в таком случае команда будет выглядеть так:

    git checkout master

## Просмотр еще не зафиксированный изменений

Чтобы посмотреть последние не зафиксированные изменения, необходимо воспользоваться командой 

    git diff

Внимание:
1. Добавленные данные будут со знаком "+" и в зеленом цвете
2. Удаленные данные будут со знаком "-" и в красном цвете

## Просмотр разницы между состояниями репозитория

Чтобы посмотреть отличие состояний репозитория друг от друга, необходимо воспользоваться командой 

    diff <hash>

где hash состоит из двух хеш-сумм сравниваемых состояний, записанных через "пробел"

[Git emblem](git.JPG)

## Ветвлении в Git нужны для того, чтобы ...

    git branch 

test newbranch 1

test newbranch 2

### создание новой ветки

чтобы создать новую ветку, необходимо воспользоваться командой:
    git branch <branchname>

    
## Зачем нужно ветвления в git

Ветвление в git позволяет создавать ветки от основной - чтобы вносить, например новый функционал. 

Более подробный пример: У вас есть ветка мастер - в которой ваш проект находится на стадии Х, и вы создали ветку тест. Дальнейшие изменения в ветке Х не будут менять ветку тест, как и наоборот, изменения в ветке тест не будут влиять на работу в ветке Х. 

Далее вы можете в ветке тест сделать то, что от вас требуется, или доработать какой-то функционал и предложить его "владельцу" проекта.

В общей сложности, можно сказать, что ветвление нужно, чтобы любое количество пользователей могло работать на проекте не изменяя его вообще, но при этом иметь возможность тестировать свою работу "локально".

## Создание новой ветки в git

Чтобы создать новую ветку, необходимо воспользоваться командой:

    git branch <branchname>

### Как переключаться между ветками

Чтобы переключиться с одной ветки на другую необходимо воспользоваться командой:

    git checkout <branchname>

## Как сливать ветки

Чтобы слить ветки, необходимо воспользоваться командой 

    git merge <branchname>


## Слиение веток - подробнее

При слиении веток может произойти конфликт
Visual code предлагает 4 вариатна продолжения слияния 
1. принятие тукущих изменений - это означает, что изменения ветки в которой вы находитесь будут приняты
2. принятие входящих изменений - данное действие приведет в принятию текущей веткой изменений, зафиксированных в ветке слияемой с данной 
3. принятие изменеий обеих веток - изменения зафиксированные в обеих ветках войдут в текущую 
4. Сравнение изменений - что делает понятно, нажимать не стоит до получения новых знаний :)


## Удаленные репозитории

Удаленные репозитории нужны чтобы... 



