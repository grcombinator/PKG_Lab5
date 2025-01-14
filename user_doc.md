# Документация пользователя для программы Segment Clipper

## Введение

**Segment Clipper** — это приложение для отсечения отрезков и многоугольников от заданного прямоугольного окна с использованием алгоритма Сазерленда-Коэна. Программа также предоставляет возможность визуализировать результаты отсечения.

## Установка
- Убедитесь, что у вас установлен Python версии 3.6 или выше.
- Установите библиотеку Matplotlib, если она еще не установлена:

```bash
pip install matplotlib
```

## Запуск программы
- Сохраните код программы в файл, например, segment_clipper.py.
- Запустите программу из командной строки:

```bash
python segment_clipper.py
```

## Использование
- Ввод количества отрезков: Программа запросит у вас ввести количество отрезков, которые вы хотите отсечь. Введите целое число.
- Ввод координат отрезков:
- Для каждого отрезка вам будет предложено ввести его координаты в формате X1 Y1 X2 Y2.

**Пример ввода**: 1 2 3 4 (где (X1, Y1) и (X2, Y2) — это координаты концов отрезка).
- Ввод координат отсечающего окна:
- После ввода всех отрезков вам нужно будет ввести координаты отсечающего окна в формате Xmin Ymin Xmax Ymax.

**Пример ввода**: 0 0 5 5.
- Выбор метода отсечения:
- Программа предложит выбрать метод отсечения:
- Введите 1 для использования алгоритма Сазерленда-Коэна.
- Введите 2 для использования алгоритма отсечения многоугольников.

### Просмотр результатов: После ввода всех данных программа визуализирует отрезки и отсеченное окно. Исходные отрезки будут отображены зеленым цветом, а отсеченные — красным.

## Примечания
- Если один или оба конца отрезка находятся за пределами отсечающего окна, программа автоматически отсечет видимые части отрезка и отобразит их.
- В случае некорректного ввода (например, нечисловые данные) программа может завершиться с ошибкой. Убедитесь, что вводимые данные соответствуют заданному формату.

## Заключение

Программа Segment Clipper предоставляет удобный интерфейс для отсечения отрезков от заданного окна и визуализации этого процесса. Используя данный инструмент, вы можете лучше понять, как работают алгоритмы геометрической обработки.
