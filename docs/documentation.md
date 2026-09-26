# Общее описание решения

В файлах сожержаться функции для вычисления <ins>площадей</ins> и <ins>периметров</ins> геометрических фигур.

- [Круг](https://github.com/Dramatae/lw2_isrpo/blob/main/circle.py) - S = πr<sup>2</sup>, P = 2πr
- [Квадрат](https://github.com/Dramatae/lw2_isrpo/blob/main/square.py) - S = a<sup>2</sup>, P = 4a
- [Треугольник](https://github.com/Dramatae/lw2_isrpo/blob/main/triangle.py) - S = ah/2, P = a+b+c

# Описание каждой функции с примерами вызова

## Circle.py
```
import math

def area(r):
   
    Возвращает площадь окружности по её радиусу.

    	Параметры:
        	r (int/float): радиус окружности
        Возвращаемое значение:
        	area (float): площадь окружности (π * r²)
    	Пример вызова:
        	area(12) = 452.3893421169302
    
    return math.pi * r * r

def perimeter(r):

    Возвращает длину окружности по её радиусу.
        
        Параметры:
        	r (int/float): радиус окружности
    	Возвращаемое значение:
        	perimeter (float): длина окружности (2 * π * r)
    	Пример вызова:
        	perimeter(12) = 75.39822368615503
    
    return 2 * math.pi * r
```

## Square.py
```
def area(a):
    
    Возвращает площадь квадрата по его стороне.

        Параметры:
            a (int/float): сторона квадрата
        Возвращаемое значение:
            area (int/float): площадь квадрата (a²)
        Пример вызова:
            area(2) = 4
    
    return a * a


def perimeter(a):
    
    Возвращает периметр квадрата по его стороне.

        Параметры:
            a (int/float): сторона квадрата
        Возвращаемое значение:
            perimeter (int/float): периметр квадрата (4 * a)
        Пример вызова:
            perimeter(2) = 8

    return 4 * a
```

## Triangle.py
```
def area(a, h):
    
    Возвращает площадь треугольника по стороне и высоте.

        Параметры:
            a (int/float): сторона треугольника
            h (int/float): высота, проведённая к этой стороне
        Возвращаемое значение:
            area (int/float): площадь треугольника (a * h / 2)
        Пример вызова:
            area(6, 12) = 36

    return a * h / 2


def perimeter(a, b, c):
    
    Возвращает периметр треугольника по трём сторонам.
        Параметры:
            a (int/float): первая сторона треугольника
            b (int/float): вторая сторона треугольника
            c (int/float): третья сторона треугольника
        Возвращаемое значение:
            perimeter (int/float): периметр треугольника (a + b + c)
        Пример вызова:
            perimeter(12, 11, 7) = 30
    
    return a + b + c
```

# История изменения проекта с хешами коммитов

| Хеш | Название коммита |
|---|---|
|fbbeaf5 | add funcs description|
|cc03a08 | add comments triangle.py|
|11a2166 | add comments square.py|
|1d4f78e | add comments circle.py|
|aaf8583 | add general description in documentation|
|fb4a90d | add files|