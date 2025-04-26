# <div align="center">Puzzle Deslizante 3x3</div>

**Curso:** Inteligencia Artificial  

## Archivos

En este repositorio encontrarás cuatro archivos:  
    - `Ejemplo_laberinto.ipynb`  
    - `laberinto.txt`  
    - `Puzzle_Deslizante.ipynb`  
    - `README.md`  

## Ejemplo_laberinto.ipynb

`Ejemplo_laberinto.ipynb` es un cuaderno de ejemplo proporcionado por el profesor. Contiene un código para resolver laberintos mediante los algoritmos BFS y DFS. Los laberintos deben escribirse en el archivo `laberinto.txt`.

## Puzzle_Deslizante.ipynb

Este cuaderno es el componente principal del repositorio. Contiene cuatro bloques de código, cada uno con una funcionalidad específica:

### Generador de puzzles

Este bloque genera aleatoriamente puzzles de 3x3 y define un estado objetivo. También permite ingresar manualmente un puzzle descomentando las líneas correspondientes.

### Solución del puzzle usando Cola (BFS/FIFO)

En este bloque se resuelve el puzzle utilizando el método de búsqueda en anchura (Breadth-First Search, BFS), también conocido como First In, First Out (FIFO).

### Solución del puzzle usando Pila (DFS/LIFO)

Este bloque resuelve el puzzle utilizando el método de búsqueda en profundidad (Depth-First Search, DFS), también conocido como Last In, First Out (LIFO).

### Solución del puzzle usando A*

En este bloque se utiliza el algoritmo A* (A-star) para resolver el puzzle, empleando como heurística la distancia de Manhattan.

## Comparación entre búsqueda informada y no informada

Se utilizó el siguiente puzzle como ejemplo para todas las pruebas:

<a align="center">

     (1, 8, 0)  
     (5, 6, 7)  
     (2, 4, 3)  

</a>

Los resultados obtenidos fueron los siguientes:

- El método con cola (BFS) exploró 136,235 estados, tardó 5 minutos con 57 segundos y encontró una solución de 24 movimientos.  
- El método con pila (DFS) exploró 133,633 estados, tardó 31 minutos con 47 segundos y encontró una solución que requiere 51,052 movimientos.  
- El algoritmo A* exploró 1,497 estados, tardó 0.1 segundos y encontró una solución de 24 movimientos.

Estos resultados muestran la eficiencia del algoritmo A* frente a los métodos de búsqueda no informada.
