# **Traballando con MapReduce**

Este repositorio contiene ejercicios prácticos diseñados para comprender y aplicar el procesamiento de datos distribuidos utilizando **Hadoop** y la técnica de **MapReduce**. A través de ejemplos simples, se demuestra cómo analizar y extraer información útil de grandes conjuntos de datos almacenados en un sistema de archivos distribuido (HDFS).

---

## **Objetivos**
- Comprender cómo funciona el procesamiento distribuido basado en **MapReduce**.
- Diseñar y modificar mappers y reducers para resolver diferentes problemas y obtener resultados específicos.
- Experimentar con el análisis de datos a gran escala utilizando Hadoop.

---

## **Descripción de los Ejercicios**
En este proyecto se trabajan diversos ejercicios que cubren desde la validación de datos hasta el cálculo de estadísticas avanzadas sobre un archivo de datos de ventas (`purchases.txt`).  

A lo largo de los ejercicios, se realizan tareas como:
- Limpieza y validación de datos.
- Cálculo de totales y máximos por categorías o criterios específicos.
- Análisis de patrones y resultados globales.  

Cada ejercicio se plantea como un paso progresivo para explorar el poder de Hadoop en el manejo de datos distribuidos.

---

## **Requisitos**
Para ejecutar los ejercicios, es necesario contar con:
1. Un sistema de **Hadoop** configurado.
2. Un archivo de datos llamado `purchases.txt` cargado en HDFS.
3. Conocimientos básicos sobre:
   - Programación de mappers y reducers.
   - Comandos de Hadoop para ejecutar trabajos y consultar resultados.

---

## **Ejecución**
1. Escribir los scripts de mappers y reducers según las indicaciones de los ejercicios.
2. Ejecutar los trabajos en Hadoop mediante comandos de consola.
3. Analizar los resultados generados y almacenados en el sistema distribuido.

**Ejemplo de ejecución de un trabajo:**
```bash
$ mapred streaming 
    -files mapper.py,reducer.py
    -input myInputDirs \
    -output myOutputDir \
    -mapper script_mapper
    -reducer script_reducer
