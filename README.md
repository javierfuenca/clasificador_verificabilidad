# Clasificador de frases verificables/no verificables
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1aO3gU4U7ESpYsPqFu8ZPg2N1xR-gZZ2O?usp=sharing)

El siguiente proyecto se trata de un clasificador que categoriza las frases como verificables o no verificables basado en BERT y válido para múltiples lenguas. El entorno utilizado ha sido Google Colab con GPU, donde solo se ha añadido la instalación de ktrain y se ha mantenido por defecto el resto de versiones de librerías utilizadas.

### Pruebas realizadas
El procedimiento que se ha utilizado a lo largo de las pruebas viene descrito en mayor detalle en las celdas de texto.

En un inicio y a modo de análisis, se restringió únicamente al inglés para unas primeras observaciones. Al obtener una precisión cercana al 90% se procedió a utilizar más idiomas, cambiando del modelo BERT en inglés al multilengua.

Más adelante, tras desdoblar en 3 idiomas (español, inglés y francés), se realizó un entrenamiento sobre una separación aleatoria entre train y test.
Sería recomendable una futura prueba que separe frases en todos los idiomas ya que al tokenizarlas es probable que, aunque estén en distinto idioma, existan frases semejantes en varios idiomas que estén en ambos sets de train y test, contaminando así los resultados de predicción.
Como el resultado que se hizo sobre un solo idioma no dista mucho del final, no parece que haya afectado en gran medida, aunque para datasets de mayor tamaño sería recomendable realizarlo de esta forma.

License
----

MIT
