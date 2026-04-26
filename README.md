# aircraft-assignment-greedy
Optimización de la asignación de aeronaves en el transporte aéreo comercial regular mediante un algoritmo Greedy de partición de intervalos

---

## Descripción

Este repositorio contiene la implementación computacional desarrollada en Python/Jupyter Notebook como parte de mi tesis de Ingeniería Aeronáutica, donde el problema de asignación de aeronaves se modela como una instancia del problema clásico de **partición de intervalos (Interval Partitioning)**.

Cada vuelo se representa como un intervalo temporal y se busca asignar aeronaves sin conflictos de traslape, minimizando el número de aeronaves requeridas.

La solución se obtiene mediante un algoritmo voraz **Earliest-Start-Time-First** implementado con una **cola de prioridad (min-heap)**.

---

## Aportaciones del proyecto

Este trabajo incluye:

- Formulación matemática del problema de asignación de aeronaves como problema de partición de intervalos.
- Implementación del algoritmo greedy óptimo.
- Cálculo de la profundidad (*Depth*) como número mínimo de aeronaves necesarias.
- Generación de instancias sintéticas de vuelos.
- Validación computacional de resultados teóricos.

Resultado central verificado:

**Número mínimo de aeronaves = Profundidad del conjunto de intervalos**

---

## Fundamento algorítmico

El algoritmo implementado sigue el esquema:

1. Ordenar vuelos por tiempo de salida.
2. Reutilizar la aeronave que se libera más temprano cuando sea factible.
3. Crear una nueva aeronave únicamente cuando sea necesario.

Complejidad temporal:

```text
O(n log n)
```

---

## Contenido del notebook

El cuaderno incluye:

- generación de instancias sintéticas  
- cálculo de profundidad  
- algoritmo greedy de asignación  
- experimentos computacionales  
- tablas de resultados  



## Ejecución

Abrir el notebook:

```bash
jupyter notebook greedy_aircraft_assignment.ipynb
```

Ejecutar todas las celdas para reproducir los experimentos.

---

## Aplicaciones

Posibles aplicaciones en:

- Planeación de flota  
- Programación de aeronaves  
- Asignación de recursos  
- Investigación de operaciones  
- Optimización en transporte aéreo

---

## Tesis asociada

Repositorio asociado al trabajo de tesis:

**Optimización de la asignación de aeronaves en transporte aéreo comercial mediante un algoritmo greedy de partición de intervalos**

Instituto Politécnico Nacional  
ESIME Unidad Ticomán

---

## Referencias

Basado en:

- Kleinberg & Tardos — Algorithm Design  
- Wayne — Algorithms, Part II

---

## Autor

Juan Antonio Vargas Juárez.

---

## Licencia

MIT License
