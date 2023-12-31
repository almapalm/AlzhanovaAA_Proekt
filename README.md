# Преобразование табличных данных в удобный для пользователя формат

### Описание 

Эта программа представляет собой утилиту для конвертации статистических данных из CSV файла, полученного, например, из сервиса статистики Telegram, в более удобный формат Excel (XLSX). Для работы она использует несколько важных библиотек.


В начале программы импортируются четыре модуля: datetime для работы с датой и временем, sys для взаимодействия с интерпретатором Python, pandas (импортированный как pd) для обработки и анализа данных, и argparse для обработки аргументов командной строки.


Основной функционал программы построен вокруг библиотеки argparse, которая используется для создания интерфейса командной строки. Программа принимает три аргумента: путь к входному файлу CSV (-i или --input), имя выходного файла Excel (-o или --output), и опциональный флаг --parce для обработки дат в CSV файле.


Далее, с помощью модуля pandas, программа читает данные из указанного CSV файла. В этом файле данные разделены табуляцией. Если был указан флаг --parce, программа дополнительно обрабатывает столбец с датами, преобразуя строки в формат даты и времени. При этом учитывается особый формат даты, указанный в CSV файле.


В итоге обработанные данные сохраняются в файл Excel. Имя выходного файла определяется пользователем через аргумент командной строки, к которому автоматически добавляется расширение .xlsx. Эта функциональность обеспечивается методом to_excel() из библиотеки pandas.

Таким образом, программа представляет собой удобный инструмент для обработки, анализа и перевода табличных данных в бюолее универсальный и удобный для анализа формат, уменьшая тем самым вероятность тшибок и экономя время.

## Google Colab
[ссылка на коллаб](https://colab.research.google.com/drive/1WqhPc3CIED0qWT0lQFzeyalKdg9VRlhc?usp=sharing)

## Результат

[Ссылка на итоговую таблицу](https://docs.google.com/spreadsheets/d/1OLgr_uLgfdLdYE-TJhzB9mYeY43x7MJc/edit?usp=sharing&ouid=101600728093234542078&rtpof=true&sd=true)

## Видеопрезентация 
[видео презентация](https://drive.google.com/file/d/18rrkDvYfyGAUINl5UHYNxBXjF4sBqWGj/view?usp=sharing)
