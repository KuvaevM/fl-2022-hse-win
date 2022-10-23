## Симуляция работы магазинного автомата

### Репозиторий
[Репозиторий проекта.](https://github.com/KuvaevM/pda_project)

### Моя подзадача
Bмея магазинный автомат и входную строку, необходимо пошагово продемонстрировать процесс принятия этой строки. Один шаг связывает две конфигурации в отношении |-. Пользователь должен иметь возможность просмотреть каждый шаг принятия строки, а также "промотать" несколько шагов, Как только найдена некоторая последовательность шагов, принимающая строку, сообщить об этом пользователю. Если строка не принимается автоматом, надо продемонстрировать все рассмотренные последовательности шагов.

### Выполненые задачи
* Была реализована симуляция работы магазинного автомата. Есть 2 режима: интерактивный (пользователь вводит команды в терминал, компьютер отвечает) и тестовый (пользователь передает название файла с уже заполненными командами).
* Моя подзадача 3 в проекте, так что мной было реализована коммуникация с выводом 2 подзадачи
* Возможны 2 вида комманд: next и next с числом. При вводе next компьютер показывает все цепочки магазинного автомата длины предыдущая плюс 1. При вводе next с числом, показываются цепочки длиной next + это число. Все цепочки между ними обрабатываются компьютером, но не выводятся.
* В случае, если обнаружилось, что строка не принимается автоматом, выводим все конечные (которые нельзя продолжить) строчки, которые у нас были. В случае, если мы смогли как-то принять строчку, немедленно выводим соответствующую цепочку шагов, завершаем программу.

### Запуск программы.
* Запускаем файл pushdown_automation.py командой python3 pushdown_automation.py <test>. Название тестового файла - как у одного из папки tests.
* Далее отрабатывает 2 часть алгоритма, строится магазинный автомат. Нам предлагают выбрать режим, в котором будем работать
* Если пишем test, то нас просят ввести название файла. Следует вводить название файла из директории automative_tests (файлы .in). Далее смотрим на вывод в соответствующем файле .out
* В интерактивном режиме просят ввести строку. Вводим, далее начинаем эмулировать работу магазинного автомата. Либо команда next - следующий шаг, либо next number - промотка на несколько шагов вперед.
