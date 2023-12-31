# Simple_Bash_Utils

Этот проект был разработан мной как дополнение к моему резюме. В этом проекте я реализовал собственные версии утилит Bash по работе с текстом: `cat` и `grep` на языке программирования C. В реализации утилиты `cat` были включены следующие флаги:

## Флаги утилиты `cat`

- `-b` (GNU: `--number-nonblank`): Нумерует только непустые строки.
- `-e` предполагает и `-v` (GNU only: `-E` то же самое, но без применения `-v`): Также отображает символы конца строки как `$`.
- `-n` (GNU: `--number`): Нумерует все выходные строки.
- `-s` (GNU: `--squeeze-blank`): Сжимает несколько смежных пустых строк.
- `-t` предполагает и `-v` (GNU: `-T` то же самое, но без применения `-v`): Также отображает табы как `^I`.

## Флаги утилиты `grep`

- `-e`: Шаблон.
- `-i`: Игнорирует различия регистра.
- `-v`: Инвертирует смысл поиска соответствий.
- `-c`: Выводит только количество совпадающих строк.
- `-l`: Выводит только совпадающие файлы.
- `-n`: Предваряет каждую строку вывода номером строки из файла ввода.
- `-h`: Выводит совпадающие строки, не предваряя их именами файлов.
- `-s`: Подавляет сообщения об ошибках о несуществующих или нечитаемых файлах.

## Тестирование

Для проверки корректности реализации каждой функции, были написаны юнит-тесты.

## Комбинация флагов

Реализована возможность комбинировать флаги для достижения максимальной гибкости в использовании утилит.

## Использование

Для использования этого проекта, клонируйте репозиторий и выполните `make` в соответствующей директории. Это сгенерирует исполняемые файлы для `cat` и `grep`.

```bash
git clone https://github.com/fatkheev/Simple_Bash_Utils.git
cd Simple_Bash_Utils/src/cat
make
cd ../grep
make
```

После этого, вы можете использовать ./s21_cat и ./s21_grep как вы бы использовали их стандартные аналоги.

## Контакты

Если у вас есть какие-либо вопросы или предложения по улучшению, не стесняйтесь связаться со мной.