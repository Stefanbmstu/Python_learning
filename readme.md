Особенности языка Python
# 1. Высокоуровневый  
Python является интерпретируемым языком - все вычисления осуществляет интерпретатор, который автоматически управляет памятью и обладает встроенными высокоуровнеыми типами данных, такими как списки, словари и множетсва.  
# 2. Динамическая типизация  
Тип переменной определяется во время выполнения, а не до него.
# 3. Язык - конструктор  
Сам базовый Python со своим встроенным набором библиотек может безгранично расширяться доп библиотеками. Это, в свою очередь, накладывает особенности, как конфликты версий (если обновили какую-то одну библиотеку). Для этого используется виртуальное окружение, об этом чуть ниже.  
  
# По типам данных:  

Делятся на 2 основных типа:
1. Незменяемые (immutable)  

1.1 Целочисленные типы данных (int)  
- Под капотом: Python использует целые числа фиксированной точности, что означает, что они могут представлять целые числа с произвольной длиной.  

1.2 Вещественные числа (float)  
- Под капотом: Python использует стандарт IEEE 754 для представления вещественных чисел, что обеспечивает точность и представление чисел с плавающей запятой.  

1.3 Строки (str)  
- Под капотом: Строки в Python представляются как последовательности символов Unicode. Это позволяет работать с текстом на различных языках и символах.  

1.4 Кортежи (tuple)  
- Под капотом: Кортежи похожи на списки, но они не могут быть изменены после создания. Это делает их более эффективными с точки зрения использования памяти.  

1.5 Логический тип (bool)  
- Под капотом: Логический тип использует один байт памяти для хранения True или False.  

1.6 None (NoneType)  
- Под капотом: Внутри Python None представлен как единственный экземпляр объекта NoneType.  

1.7 Хэш - множества (frozenset)  
- Под капотом: Внутри Python множества реализованы как хэш-таблицы (set) или неизменяемые хэш-множества (frozenset).

2. Изменяемые (mutable)  

2.1 Списки (list)  
- Под капотом: Внутри Python списки реализованы как динамические массивы, что позволяет эффективное добавление и удаление элементов.  

2.2 Словари (dict)  
- Под капотом: Внутри Python словари реализованы как хэш-таблицы, что обеспечивает быстрый доступ к значениям по ключу.  

2.3 Множества (set)  
- Под капотом: Внутри Python множества реализованы как хэш-таблицы (set).  

# Установка виртуального окружения  
Вирутальное коружение используется дла работы изолированного интерпретатора Python (любой версии, не обязательно совпадающей с глобальной, и всеми необходимыми для конкретного проекта библиотеками)
Поставить можно в VS Code двумя способами:  
1. CLI  
Открываем командную строку `Ctrl + ~`, создаем каталог проекта, переходим в директорию, выполняем команду `python -m venv myenv` (myenv - название окружения) и активируем его `myenv\Scripts\activate`.  
2. Горячими клавишами  
`Ctrl + Shift + P` --> `Python: Create Environment` --> `Select Interpreter` --> `venv`.  
Создается и активируется автоматически.  
При создании окржуения станет доступен установщик пакетов pip. `pip install/uninstall package`
# Зависимости  
Зависимости от всех библиотек проекта хранятся в файлу `reqirements.txt`.  
Установка `pip install -r requrements.txt`  
Создание `pip freeze > reqirements.txt`
 


