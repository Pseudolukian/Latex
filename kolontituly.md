# Колонтитулы

Для управлением колонтитулами следует подключить пакет `\usepackage`. Нижний и верхний колонтитул состоит из трех секций: левой \(L\), центральной \(C\) и правой \(R\). Каждую секцию можно настроить. За управление верхним колонтитулом отвечает команда `\fancyhead`, а за нижний - `\fancyfoot`.

В \[\] указывается позиция, а в {} указывается текст. Так настройка колонтикулов может выглядить вот так: `\fancyhead[R]{Это простой пример верхнего колонтитула}`  
`\fancyhead[L]{}`  
`\fancyhead[C]{}`

`\fancyfoot[R]{ \copyright Конник М.В., перевод}`  
`\fancyfoot[L]{Страница \thepage \; из \pageref{LastPage}}`  
`\fancyfoot[C]{}`

Отступ колонтитула от верхнего края листа задаётся командой `\topmargin=0pt`. В таком виде колонтитул отступит на 2,5 см от верхнего края. Меняя значения на отрицательные вы будете уменьшать отступ. Для меня идеальное значения оказалось -50pt.

Часто бывает, что нумерация страниц должна начинаться не с первой. В этом случае можно поместить на первыую страницу отсчёта команду: `\setcounter{page}{стартовый номер страницы}`.

