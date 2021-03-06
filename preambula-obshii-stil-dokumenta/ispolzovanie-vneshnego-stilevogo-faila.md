# Использование внешнего стилевого файла

Когда вы работаете над большим проектом преамбула файла сборки раздувается до больших размеров и с ней становится сложно работать. К тому же такой подход не позволяет работать над несколькими проектами, используя один стиль. Поэтому хорошим решением является создание стилевого файла и помещения в него преамбулы.

**Алгоритм такой**:

* Создаётся файл с расширением .sty;
* Первая команда в нём: `\ProvidesPackage{название файла без расширения}`далее следует преамбула;
* В сборочном файле указываются две команды: `\documentclass[a4paper,14pt]{нужный формат документа}` `\usepackage{название стилевого файла без расширения}`.

**Важны несколько основных моментов!**

Во-первых, название стилевого файла, подключаемого пакета в преамбуле компилируемого файла и название декларации в стилевой файле должны совпадать.  
Во-вторых, вначале компилируемого файла должна идти команда `\documentclass[a4paper,14pt]{нужный формат документа}` и только потом подключение стилевого файла.

