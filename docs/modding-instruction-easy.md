# Если удалять нужно мало
### Скачиваем исходный код модификации
В списке дополнений нажимаем на [И], после чего нажимаем на Source или Issues. Переходим во вкладку "code" и затем, убедившись, что выбранная ветка (branch) соответствует версии сервера, нажимаем на зеленую кнопочку "Code" и выбраем "download zip".
Распаковыем архив в любом удобном месте.

Готово! Перед вами исходный код дополнения + файлы для обратной сборки. Сам код дополнения находится в директории src/main.

### Вносим изменения в код
Теперь нам нужно определить системные названия блоков, подлежащих удалению. Как правило, рабочих вариантов 2:
- копаться в названии папок и файлов (например, в resources\\assets\\(название_дополнения)\\(тип_объекта)
- открываем с помощью Notepad++ любой текстовый документ, нажимаем ctrl+f -> найти в файлах и, ограничив зону поиска директорией main, испытываем удачу и ваши знания английского

Определив системное название объекта, с помощью того же Notepad++ начинаем искать все совпадения. 
- если совпадение в названии файла, то удаляем файл
- если совпадении в строчках кода, аккуратно вырезаем их, стараясь не нарушить оставшуюся логику. Если сомневаетесь - спрашивайте в дискорде.

Попутно КРАЙНЕ желательно помечать связанные с удаляемым объектом переменные - это могут быть рецепты, блоки или другие особенности.
>Пример: у Ostrich может быть блок Ostrich_nest, а также выпадаемые предметы Ostrich_egg и Ostrich_meat. Ничего из этого нам не нужно.

Повторяем процедуру для всех удаляемых объектов :)
