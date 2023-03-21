План:

1. Создаем базу для fine-tuningа нейронки LLAMA
2. Файнтюним
3. Выкладываем и делаем доступные endpointы аналогичные openai
4. Подключаем к нашему VedaVany боту

Сейчас делаем только пункт 1. Пункты 2,3,4 - только собираем информацию, но реализуем позже

Для пункта 1:

* есть репозиторий - как на основе 175 инструкций РУЧНОГО ввода - сделать больше инструкций АВТОМАТИЧЕСКИ СГЕНЕРИРОВННЫХ https://github.com/yizhongw/self-instruct
* есть файл alpaka_data.json с 56К инструкциями, оригинал тут: https://raw.githubusercontent.com/tatsu-lab/stanford_alpaca/main/alpaca_data.json

Конкретные задачи (можно решать в параллель):
1.2. изучить alpaka_data.json
1.2.1. составить alpaka_data_delete.json - инструкции, которые неправильные и нужно удалить (можно просто скопировать неправильные элементы массива json c аттрибутами "instruction","input","output")
1.2.2. составить alpaka_data_update.json - инструкции, которые нужно скорректировать "instruction","input"


Позже (Для пункта 2 - реализации файнтюнинга)
https://github.com/tatsu-lab/stanford_alpaca


Статья на тему
https://newatlas.com/technology/stanford-alpaca-cheap-gpt/