# Personalizacion-LangChain
Este proyecto utiliza LangChain para realizar consultas sobre los datos del Titanic, que están disponibles tanto en un archivo XLSX como en una base de datos SQL. El agente LangChain selecciona automáticamente la fuente de datos más adecuada (SQL o XLSX) para responder a las consultas del usuario.

## Cargar el archivo XLSX y la base de datos SQL:

Si aún no tienes la base de datos SQL, puedes convertir el archivo XLSX a SQL utilizando pandas:
![](https://github.com/ANTHONYCCOLQUE/t44/blob/main/p1.png)

## Consultas básicas y más complejas:

Puedes realizar consultas como:

- ¿Cuántos sobrevivientes había en el Titanic?

- ¿Qué edades tenían los pasajeros que sobrevivieron y viajaban en la primera clase?

- ¿Cuáles son los nombres de los pasajeros que sobrevivieron y tenían más de 30 años?

Aquí hay un ejemplo de cómo realizar consultas a través del agente LangChain:
![](https://github.com/ANTHONYCCOLQUE/t44/blob/main/d2.png)

![](https://github.com/ANTHONYCCOLQUE/t44/blob/main/d3.png)


## Ejemplos de consultas:
Algunos ejemplos de preguntas que puedes hacer y cómo el sistema las maneja:

**¿Cuántos pasajeros sobrevivieron?**

SQL es elegido para esta consulta, y el agente ejecuta la consulta SELECT COUNT(*) FROM passengers WHERE Survived = 1.

**¿Qué edades tenían los pasajeros que sobrevivieron y viajaban en la primera clase?**

XLSX es elegido ya que la consulta involucra múltiples columnas y filtros más complejos.

**¿Quiénes fueron los pasajeros que viajaban en la tercera clase?**

La consulta utiliza SQL y devuelve el número de pasajeros que viajaban en clase 3.

![](https://github.com/ANTHONYCCOLQUE/t44/upload)
