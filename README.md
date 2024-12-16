# Лабораторная работа: Использование команды grep

Для решения понадобится установить Docker. Можно это делать как в виртуальной машине с установленным Linux, так и через WSL (главное на линукс подобной системе).
## Цель работы
Изучить команду grep, ее основные функции и возможности, а также применить ее для поиска текстовой информации в файлах.
## Пример (не надо его включать в отчет!)
### Шаг 1: Ознакомление с командой grep
Команда grep (Global Regular Expression Print) используется для поиска строк, соответствующих заданному шаблону. Она позволяет находить текст в файлах и выводить строки, которые содержат искомую подстроку.
### Шаг 2: Пример использования команды
1. Создание тестового файла:
```
echo -e "Hello World\nThis is a test file.\nGrep is powerful.\nGoodbye World" > testfile.txt
```
2. Поиск строки "Grep":
```
   grep "Grep" testfile.txt
```
**Ожидаемый вывод:**
```
     Grep is powerful.
```
### Шаг 3: Примеры некоторых параметров команды grep
• -i: Игнорировать регистр (поиск без учета регистра).

• -v: Вывести строки, не содержащие шаблон.

• -r: Рекурсивный поиск в директориях.

• -n: Вывести номера строк, где найден шаблон.

**Пример с параметрами:**
```
   grep -i "hello" testfile.txt

```
**Ожидаемый вывод:**
```
     Hello World
```
## Задание 2: Задача на выполнение
### Условие задачи
Создайте текстовый файл, содержащий следующий список студентов и их оценки:

* Alice: 85
* Bob: 90
* Eve: 88
* Grace: 95
* Sara: 91
* Mark: 74
* Sasha: 86
* Tim: 99

Используя команду grep, выполните следующие действия:

1. Найдите всех студентов с оценкой выше 80.
2. Найдите всех студентов с оценкой ниже 80.
3. Найдите студентов, чьи имена начинаются на букву "A".
4. Найдите любого студента из списка, не учитывая регистр
5. Подсчитайте общее количество студентов, у которых оценка выше 90
6. Сделайте вывод только имен студентов с оценками выше 85

Приложите скриншоты к каждому пункту.

### Как успешно сдать работу?

Создать свой репозиторий из шаблона этого. Как это делается - "Use this template" -> "Create a new repository" и сделайте его public. 

Находясь уже в своем репозитории - создайте новый файл формата .md и там оформляйте отчет. В отчете опишите все шаги которые вы делали, чтобы получить финальный результат работы.
 

## Источники

[Источник где можно найти все](https://google.com)

[Документация по команде grep](https://man7.org/linux/man-pages/man1/grep.1.html)

[Регулярные выражения](https://www.regular-expressions.info/)


