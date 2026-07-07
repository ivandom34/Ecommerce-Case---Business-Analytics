<<<<<<< HEAD
IVAN DOMINGO MORAZA - PEC 4

1. Estructura del proyecto:

Las carpetas se han estructurado de la siguiente forma:

- src/
   - main.py: Fichero principal que ejecuta los todos los ejercicios de la PEC
   de manera secuencial.
   - exercises/: Contiene las funciones de los diferentes ejercicios.
     - ex1.py
     - ex2.py
     - ex3.py
     - ex4.py
     - ex5.py
     - ex6.py
     - ex7.py

   - data/: LaLigaMatches.csv
   - img/: Imágenes generadas al ejecutar el main
- tests/:
   - tests_ex6.py
- doc/: La documentación de cada ejercicio
- screenshots/: Contiene capturas que acreditan el trabajo realizado
- requirements.txt: Tenemos las librerías del proyecto junto con su versión
- README.md: Contiene toda la información del proyecto.
- LICENSE: La licencia del proyecto

2. Instalación

Para ejecutar el proyecto se necesita instalar previamente un entorno con las librerías
necesarias para su ejecución. Para ello, es necesario que en el terminal se ejecuten los
siguientes comandos:

- python -m venv entorno_pec4
- entorno_pec4\Scripts\activate
- pip install -r requirements.txt

De esta manera nos aseguramos crear un entorno seguro para el proyecto donde no haya
problemas entre las diferentes versiones de las librerías.

3. Ejecución del proyecto

Una vez hemos preparado todo para ejecutar, desde el terminal nos colocamos en la carpeta
donde se encuentra el main y lo ejecutamos:
- cd Carpeta_pec...
- python main.py

También tenemos la opción de ejecutar ejercicios sueltos, por ejemplo, ex4. Además, en un
notebook / python podemos importar funciones determinadas de algún ejercicio.

4. Comprobación de análisis estático (linting) 

Gracias a Pylint se se han podido corregir problemas de estilo y calidad del código. Al principio,
partíamos de una nota de 0.36, pues se habían cometido errores sobre todo de indetación, demasiados
caracteres en una línea, espacios, no teníamos puesto docstrings, etc.

Poco a poco se fueron corrigiendo todos esos errores menos uno, que consideramos correcto por el enunciado
del ejercicio. En el fichero de config.py, las constantes van en mayúsculas, pero nosortros lo hemos puesto
en minúsculas: nom_alumne. Esto es así porque en el enunciado pone extresamente que debía ser con ese nombre.

La puntuación final fue de 9.90.

Para la revisión del código se usó: python -m pylint src

5. Generaciónd de la documentación con pydoc.

El hecho de corregir problemas de calidad de código con Pylint, nos dejó la documentación más limpia a la hora
de usar pydoc. Esto lo pudimos ver en los comentarios y docstrings que se añadieron previamente y era necesario
poner para generar la documentación con pydoc. 

La documentación se subió en la carpeta "doc/", situada en la carpeta raíz, que contiene los archivos html que se
generaron automaticamente.

Para generar la documentación se utilizó:

- Push-Location .\doc
- python -m pydoc -w config main exercises exercises.ex1 exercises.ex2 exercises.ex3 exercises.ex4 exercises.ex5
exercises.ex6 exercises.ex7
- Pop-Location

La salida de esta ejecución fue la obtención de 7 documentos html con la explicación que habíamos puesto en los 
docstrings de las funciones.

6. Test del ejercicio 6.

Para comprobar que el ejercicio 6 funciona correctamente usamos: python -m pytest tests/test_ejercicio_6.py
El código de test simplemente comprueba a partir de un dataframe ficticio que se ejecuta correctamente la
suma de los valores de dos columnas (goles del local y visitante), la suma de los goles a favor + visistante
y que la salida es una tupla con 3 valores correspondientes a la suma de las 3 columnas mencionadas.

7. Fichero requirements.txt

Las librerías utilizadas en el proyecto que aparecen en el fichero de requirements.txt son:

matplotlib==3.10.9
networkx==3.6.1
pandas==3.0.3
seaborn==0.13.2

8. Subir el proyecto a GitHub
git init
git add .
git commit -m "IVAN_DOMINGO_MORAZA_PEC4"
git branch -M main
git remote add origin https://github.com/ivandom34/IVAN_DOMINGO_MORAZA_PEC4.git
git push -u origin main


9. Licencia

Este proyecto cuenta con licencia conforme a los términos de la licencia MIT
=======
# Ecommerce-Case---Business-Analytics
This project analyzes an e-commerce dataset to identify insights that could drive revenue growth for the company. The project covers different analytical techniques such as RFM, LTV or a recommendation system.  
>>>>>>> 58a8f9e2296df34818e6ba3af7d8627c05cc09a8
