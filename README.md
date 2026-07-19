# Clasificador de Objetos Celestes

Repositorio que contiene el proyecto de machine learning para el ramo de Introduccion a los Repositorios de Codigo Distribuido, el proyecto trata sobre clasificacion de objetos astronomicos (estrellas, galaxias y quaseres) basandose en las caracteristicas y en las emisiones de luz de los cuerpos.

Para la clasficacion de los objetos se entrenaron y evaluaron dos modelos distintos, el primero es un modelo Random Forest, este ademas es el modelo principal, ya que alcanzo una precision del 98%. Como segundo modelo se entreno un KNN en donde la precision fue de tan solo 95%.

Instrucciones de ejecucion:
1) Clonar este repositorio
2) Verificar que las librerias 'pandas', 'scikit-learn', 'matplotlib' y 'seaborn' esten instaladas en el entorno donde se ejecutara el codigo.
3) abrir el archivo 'clasificador.ipynb' y ejecutar celda por celda de manera secuencial.

### Nueva Feat: Clasificación de un objeto nuevo
Se incluye la función `clasificar_objeto(u, g, r, i, z, redshift)`, que permite usar el modelo ya entrenado para predecir la clase de un objeto astronómico nuevo a partir de sus magnitudes y su redshift. La función valida que todas las entradas sean numéricas y retorna la clase predicha junto con la probabilidad de cada clase.

Ejemplo de uso:
```python
clasificar_objeto(u=22.79, g=21.65, r=20.05, i=19.18, z=18.74, redshift=0.52)
```

```
# Resultado
{'clase_predicha': 'GALAXY', 'probabilidades': {'GALAXY': 0.99, 'QSO': 0.01, 'STAR': 0.0}}
```

### Declaración de uso de Inteligencia Artificial
De acuerdo con las exigencias de la evaluación, se declara el uso de herramientas de Inteligencia Artificial (IA) como apoyo durante la elaboración de este informe. Su utilización se limitó estrictamente a la corrección ortográfica y gramatical, la adecuación del estilo de redacción y la estructuración de las ideas para el análisis del historial de Git. Todo el código fuente, el entrenamiento de los modelos predictivos y las decisiones técnicas sobre la integración y resolución de conflictos en el repositorio fueron desarrollados e interpretados de manera completamente personal.