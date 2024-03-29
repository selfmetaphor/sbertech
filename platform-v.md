# Работа с Shell. Вычитка

---

## Стилистика

1. Длинные абзацы. Такую информацию сложно воспринимать, у читателя может сложиться впечатление, что материал длинный, сложный. Лучше разбить на несколько или сократить.

    **Пример:**

    Говоря о командной строке, на самом деле мы имеем в виду командную оболочку (shell). Командная оболочка — это программа, которая принимает команды, введенные с клавиатуры, и передает их операционной системе для выполнения. Практически все дистрибутивы Linux поставляются с командной оболочкой из проекта GNU, которая называется bash. Имя bash — это аббревиатура от названия Bourne Again Shell, отражающего тот факт, что bash является улучшенной заменой sh, первоначальной командной оболочки для Unix.

2. Длинные предложения. Также сложно читать и разбираться, что к чему относится. Большую часть можно просто разбить на несколько.

    **Примеры:** 

    Имя bash — это аббревиатура от названия Bourne Again Shell, отражающего тот факт, что bash является улучшенной заменой sh, первоначальной командной оболочки для Unix.

    Если последний символ в приглашении — знак решетки (#), а не знак доллара, это означает, что сеанс в терминале обладает привилегиями суперпользователя.

    <…> выводит каталог, в котором сейчас находитесь; в командной строке пользователь не может быть «просто так», он находится в каком-либо каталоге (текущем и рабочем каталоге).

3. Причастия, деепричастия и обороты с ними. Такие конструкции утяжеляют предложение, добавляют запятых, в предложении становится сложно разобраться с первого прочтения. Лучше разбить предложения или опустить.

    **Примеры**:

    Говоря о командной строке, введенные с клавиатуры, отражающего тот факт, улучшенной заменой.

4. Буквальные повторы в списке. Стоит переформулировать или выбрать другую форму представления информации.

    **Примеры:**

    выводит имя машины, выводит логин, выводит каталог.

## Стиль изложения

### Не стиль технической документации

Стиль изложения не похож на стиль изложения технической документации.
Автор дает очень много отступлений, например, в первом абзаце, делая акцент на описании каких-то сущностей и терминов.
Знание этих определений не помогает пользователю в решении своих задач, а только отвлекает внимание.

К тому же складывается ощущение, что автор не совсем понимает свою аудиторию и разжевывает довольно очевидные вещи для читателя документа подобной сложности.

Если определения сущностей и терминов важны в документе, их стоит вынести в отдельный раздел.

### Бесполезная информация

1. Бесполезные отступления: *в командной строке пользователь не может быть «просто так»*.
Можно просто оставить, что он всегда находится в каком-либо каталоге.

2. Очевидные вещи: *знак решетки (#)*. При это знак доллара автор далее не иллюстрирует наглядно.

### Неоднозначность формулировок

*Вероятно, текущий и рабочий каталог выводятся в приглашении (prompt).* — не очень понятно, как читатель должен интерпретировать такую фразу: автор сам не знает или текущий и рабочий каталог по-разному выводятся в зависимости от обстоятельств (каких?).


## Структура и форматирование

1. Несвязность примечания. Не хватает связки между вводным абзацем раздела и примечанием. Сейчас получается довольно резкий переход, не очень понятно, при чем тут приглашение сразу после вводного абзаца.

2. Оформление списка:

    - Инструкция из одного пошагового пункта — можно было не оформлять как инструкцию. Если нужно, в качестве вводного предложения можно вынести *Выполните следующие команды*.
    - Не понятна конечная цель пошаговой инструкции. Зачем именно выполнять следующие команды. Кажется, что пошаговая инструкция тут не нужна. Можно просто маркированным списком оставить описание команд.
    - Неконсистентная пунктуация в конце пунктов маркированного списка. Последний пункт заканчивается точкой с запятой, предпоследний точкой. Последний точно должен заканчиваться точкой. Некоторые пункты длинные (стоит разбить на несколько предложений) — в таком случае стоит везде поставить точку.
    - `ls /home` не выделено полужирным, как другие команды.
    - Неконсистентные формулировки в пунктах списка: где-то есть глагол (*выводит*), где-то сразу используется существительное.

3. Оформление заголовков. В документе не хватает нумерации или более явного оформления заголовков разного уровня. Не совсем по документу понятно *Получение информации о своем пользователе и своей группе* относится к разделу *Работа с Shell* или уже нет.

4. Место раздела. Довольно вводный раздел про работу с Shell поместили между довольно «конкретными» разделами:

    * *Завершение пользовательской сессии*;
    * *Получение информации о своем пользователе и своей группе*.

    Складывается ощущение, что этот раздел структурно не на своем месте. Или ему нужно дать другой заголовок.