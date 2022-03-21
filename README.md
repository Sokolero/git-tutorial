# git-tutorial

## Git В локальном репозитории

**1. git init**
  создает новый репозиторий в той директории, где запущена команда. С этого момента гит отслеживает все изменения файлов/ папок в этой директории. Короче в корне проекта
#
**2. git add { путь к файлу, папке, изменения которой нужно добавить в репозиторий, наприме _src/index.js_ }**
**Используй вместо пути * - добавить изменения по ВСЕМ файлам проекта** (использую, когда не заморачиваюсь). Изменения добавляются в ИНДЕКС, что-то вроде промежуточной стадии перед тем, как окончательно утвердить изменения, типа буфера такого, изменения кода в нем еще не попали в репозиторий.
#
**3. git status** - посмотреть текущее состояние индекса и изменений - варианты: нет изменений для коммита/ есть изменения и они еще не индексе (красным шрифтом) / есть изменения в индексе (зеленым шрифтом)
# 
**4. git commit -m "Исправлен баг в файле app.js"**
  делаем коммит (то бишь окончательную запись этой версии кода в репозиторий), флаг -m означает "добавить описание коммита сразу", а дальше собственно строка с описанием коммита. Если делать без флага, гит откроет типа редактора для текста описания, обычно не пользуюсь.
  
  После этого локальный репозиторий хранит твой код.
  
## GitHub как удаленный репозиторий
Сервис GitHub позволяет публиковать свои/ скачивать чужие репозитории, а также совместно вносить изменения в код проекта.
1. Регишься на **Гитхаб**
2. Создаешь новый пустой репозиторий, там в панели плюсик, разберешься кароч, но! **ЛУЧШЕ не добавляй файлы README или что-то еще, пусть будет пустой прям.**
3. **Сделай в в корне проекта файл c названием .gitignore** (внутри напиши строку "node_modules/", или можешь в моих репозиториях его копирнуть), это, чтобы в в репозиторий не записывались тыщи всех библиотек, а только исходный код
4. Из корня проекта запускаешь 
  **git add remote origin https://github.com/YourProfile/YourRepository**
  так ты объявляешь удаленный репозиторий, под локальным именем origin и адрес своего репозитория (копирнешь ссылку на свой удаленный репо из Гитхаба)
  
  Все, теперь ты готов делиться с миром своим высоким искусством))
**5. git push origin main - кидаем наш локальный репо на удаленную репу в ветку MAIN, она у нас главная, он там попросит почту/ пароль**
  #
  И усе! Теперь твой код в репе на гитхаб и кидай ссылку кому угодно)


  
  
  
