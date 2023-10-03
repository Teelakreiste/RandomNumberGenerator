# Método de Cuadrados y Productos Centrales

Este es un script que implementa el Método de Cuadrados y Productos Centrales para la generación de números aleatorios. El método permite generar secuencias de números pseudoaleatorios utilizando operaciones matemáticas simples a partir de semillas iniciales.

## Librerías

Se importa la librería `display` de IPython para mostrar resultados y Markdown.

## Funciones Principales

### `getNumberByMethod(x, y, option)`

Esta función obtiene un número calculado según el método seleccionado.

- `x`: Semilla uno.
- `y`: Semilla dos (ignorada si se utiliza el método de cuadrados centrales).
- `option`: Indicador del método (True para cuadrados centrales, False para productos centrales).

### `constraint(n, k)`

Esta función verifica las restricciones para agregar o no un cero.

- `n`: Número a verificar.
- `k`: Longitud deseada.

### `addZero(n, k, position)`

Esta función agrega un cero a la izquierda o derecha de un número según las restricciones.

- `n`: Número a modificar.
- `k`: Longitud deseada.
- `position`: Indicador de posición (True para agregar a la izquierda, False para agregar a la derecha).

### `getCentralNumbers(n, k)`

Esta función obtiene los dígitos centrales de un número.

- `n`: Número del cual se extraerán los dígitos centrales.
- `k`: Cantidad de dígitos centrales a extraer.

### `random(xOne, xTwo, k, m, method, position)`

Esta función genera un número pseudoaleatorio.

- `xOne`: Semilla uno.
- `xTwo`: Semilla dos.
- `k`: Longitud de las semillas.
- `m`: Valor de módulo.
- `method`: Método seleccionado (True para cuadrados centrales, False para productos centrales).
- `position`: Indicador de posición del cero (True para izquierda, False para derecha).

### `checkDuplicity(list, n)`

Esta función verifica la duplicidad de números generados.

- `list`: Lista de números generados.
- `n`: Número a verificar.

### `showInitParameters(seed_one, seed_two, k, m, zero_left, method)`

Esta función muestra los parámetros iniciales.

- `seed_one`: Semilla uno.
- `seed_two`: Semilla dos (ignorada si se utiliza el método de cuadrados centrales).
- `k`: Longitud de las semillas.
- `m`: Valor de módulo.
- `zero_left`: Indicador de ceros a la izquierda.
- `method`: Método seleccionado (cuadrados centrales o productos centrales).

### `runMethods(seed_one, seed_two, zero_left, method, iter)`

Esta función ejecuta los métodos de generación de números aleatorios.

- `seed_one`: Semilla uno.
- `seed_two`: Semilla dos (ignorada si se utiliza el método de cuadrados centrales).
- `zero_left`: Indicador de ceros a la izquierda.
- `method`: Método seleccionado (True para cuadrados centrales, False para productos centrales).
- `iter`: Número de iteraciones (0 para cálculo en pausa).
