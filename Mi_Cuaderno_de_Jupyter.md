# Mi primer cuaderno de Jupyter Notebook
Esta es una prueba de ejecución de código Python y Markdown dentro de Jupyter Notebook


```python
print("Hola mundo")
```

    Hola mundo
    

# Listas en Python
Las listas son utilizadas para almacenar datos simples 


```python
mi_lista = [0,4,7,3,9,2,8]
print(mi_lista)
mi_lista.sort()
print(mi_lista)
```

    [0, 4, 7, 3, 9, 2, 8]
    [0, 2, 3, 4, 7, 8, 9]
    

# Tuplas en Python
Las tuplas son utilizadas para almacenar datos simples que no se puedan cambiar


```python
mi_tupla = ("manzana","mango","naranja")
print(mi_tupla)
```

    ('manzana', 'mango', 'naranja')
    

# Sets en Python
Se utilizan para almacenar datos simples, desordenados y no indexados


```python
mi_set = {"manzana", "mango", "naranja"}
print(mi_set)
```

    {'naranja', 'manzana', 'mango'}
    

# Diccionarios en Python
Se usan para almacenar valores de datos en pares de clave:valor, no permite duplicados


```python
mi_diccionario = {
    "nombre": "Yesser",
    "cedula": "8163535363637",
    "correo": "nombre@mail.com"
}
print(mi_diccionario)
```

    {'nombre': 'Yesser', 'cedula': '8163535363637', 'correo': 'nombre@mail.com'}
    


```python
# accediendo a datos del diccionario 
print(mi_diccionario["correo"])
```

    nombre@mail.com
    

# Fechas en Python
Los objetos de fecha se manipulan usando el modulo **datetime**


```python
import datetime
```


```python
x = datetime.datetime.now()
print(x)
```

    2021-08-23 16:23:00.455676
    

# Aplicando Numpy
Importando numpy para el calculo de la media, mediana y moda


```python
import numpy
```


```python
# calculo de la media 
velocidades = [70,80,77,82,90,76,77,85,86,82,76,75,72]
resultado_normal = (70+80+77+82+90+76+77+85+86+82+76+75+72)/13
print(resultado_normal)
```

    79.07692307692308
    


```python
resultado_numpy = numpy.mean(velocidades)
print(resultado_numpy)
```

    79.07692307692308
    


```python
# calculo de la mediana
mediana = numpy.median(velocidades)
print("mediana: ", mediana)
```

    mediana:  77.0
    


```python
# calculo de la moda
from scipy import stats
moda = stats.mode(velocidades)
print("Mode: ", moda)
```

    Mode:  ModeResult(mode=array([76]), count=array([2]))
    
