# Поиск файлов по подстроке

## Условие задания

В данном задании необходимо написать программу, которая позволяет быстро искать файлы по подстроке. Программе даётся каталог, ей необходимо его проиндексировать, подписаться на его модификацию и быстро уметь находить подстроку внутри текстовых файлов.

## Требования

- Программа должна иметь графический интерфейс на базе библиотеки Qt Widgets. Использование других тулкитов требует предварительного согласования. Познакомиться с возможностями библиотеки Qt, можно используя секцию Welcome/Examples в Qt Creator или использование программы qtdemo. По [ссылке](https://github.com/sorokin/dirdemo) расположен простой пример программы работающей с директориями и имеющей графический интерфейс.
- Для работы с файлами разрешается использовать: Qt, `std::filesystem`, `boost::filesystem` либо POSIX-функции `opendir`/`readdir`/`closedir`.
- Файлов в каталоге может быть много, много больших бинарных и текстовых файлов, считайте, что у вас могут быть гигабайты текста (быстрые индексы требуют много памяти, поэтому вы скорее всего проиграете с ними).

## Дополнительная информация

- В задании специально не специфицируется, как именно должен выглядеть интерфейс программы. Студентам предлагается самим подумать, какой интерфейс лучше всего подойдет для этой задачи.
- Подумайте над:
  - Выбором способа индексации директории
  - Многопоточной индексации
  - Многопоточным поиском
  - Возможностью отмены поиска
  - JIT search function