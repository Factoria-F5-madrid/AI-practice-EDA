# EDA con el catálogo CVE

## Para qué sirve

Hacer un análisis exploratorio de datos de principio a fin con datos reales: casi 90.000 vulnerabilidades de software del catálogo público CVE.

Al acabar sabrás responder tres preguntas con datos:

1. ¿Cuántas vulnerabilidades son graves de verdad?
2. ¿Hay tipos de fallo peores que otros? Por ejemplo, ¿SQL Injection o XSS?
3. ¿Qué tipos de fallo habría que revisar primero?

Y te quedas con un esquema que vale para cualquier tabla: mirar qué hay, limpiar, medir una variable, cruzar dos, sacar conclusiones.

## Cómo ejecutarlo

Necesitas Python 3.10 o superior.

```bash
pip install pandas matplotlib seaborn kagglehub
```

Abre `cve_eda_clase.ipynb` en VS Code o en Jupyter y ejecuta las celdas en orden. La primera celda descarga los datos (9 MB, sin cuenta de Kaggle). Tarda unos segundos.

## Cómo está montado

- Empieza con el caso, con qué datos se trabaja, qué es un EDA y sus 10 fases.
- Los bloques 0, 1 y 2 vienen hechos: cargar, mirar la tabla y contar los huecos.
- Desde el bloque 3 el código tiene huecos marcados con `____`. Encima de cada celda están las preguntas que llevan a cada hueco y dos opciones posibles. Decide, rellena y ejecuta.
- Debajo de cada bloque hay una celda con lo que se decidió y lo que tiene que salir. Úsala para comparar.
- La celda "Prueba" de cada bloque es para probar otra opción y ver si cambia el resultado.
- Al final hay un bloque "Ahora tú" con una pregunta sin huecos ni opciones, para que la resuelvas desde cero y compares con una forma de hacerlo.

Si dejas un hueco sin rellenar, sale `NameError: name '____' is not defined`. Es eso, no otra cosa.



## Datos

[CVE, Common Vulnerabilities and Exposures](https://www.kaggle.com/datasets/andrewkronser/cve-common-vulnerabilities-and-exposures), versión 3, publicada en Kaggle con licencia libre. Son los datos de la base NVD del NIST entre 1999 y noviembre de 2019.
