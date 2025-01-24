# Practica_5.1_Entornos

![Diagrama](https://github.com/Lmrocio/Practica_5.1_Entornos/blob/main/Untitled%20Diagram.png?raw=true)


## 1.Interpreta el significado del diagrama de clases.

a) Relación entre las clases. Significado, tipo, multiplicidad. 

  Las clases que se relacionan son 'Curso' y 'Estudiante', cuya relación es que un curso contiene de uno a varios estudiantes 
  (en este caso, no se especifíca el número mínimo, pero interpreto que es más coherente que deba existir mínimo un alumno en
  el curso), y un estudiante está contenido en un sólo curso. El tipo de la relación es de agregación, lo cual podemos saberlo
  por el rombo vacío que une ambas tablas, y quiere decir que una de las clases, en este caso 'Curso', representa un todo del
  cual la otra clase, en este caso 'Estudiante', representa una parte.
  

b) Elementos de las clases. Tipos y propósito. 

En cada clase podemos encontrar sus atributos, ubicados en la primera parte de la tabla, y sus métodos, en la segunda parte.

- Curso:
  - Atributos:
    - Nombre es un atributo privado de tipo 'String' o palabra que contiene el nombre del objeto de tipo Curso, es decir, de una instancia determinada.
    - Código es un atributo privado de tipo 'String' que contiene el código del objeto de tipo Curso.
    - Estudiantes es un atributo privado de tipo 'MutableList' que contiene una lista con los estudiantes que conforman un curso.
      
  - Métodos:
    - agregarEstudiante(Estudiante estudiante): es una función pública de la clase que añade una instancia de la clase Estudiante a la lista de estudiantes que pertenecen a un curso.
    - mostrarEstudiante(): es una función pública de la clase que muestra por pantalla los datos de un determinado estudiante de un curso concreto.

- Estudiante:
  - Atributos:
    - Nombre es un atributo público de tipo 'String' que contiene el nombre del objeto de tipo Estudiante.
    - Dni es un atributo público de tipo 'String' que contiene el dni de un estudiante.
      
  - Métodos:
    - inscribirseCurso(Curso curso): es una función pública de la clase que inscribe a un estudiante en un determinado curso.


c)Significado del método agregarAlumno(). Funcionamiento. 

  El método agregarEstudiante(estudiante: Estudiante) recibe un objeto de la clase 'Estudiante' y lo añade en la lista 'estudiantes' que es uno de los
  atributos de la clase Curso.


d) Significado del método inscribirse()

En este caso, el método pertenece a la clase 'Estudiante' y llama al método 'agregarEstudiante' de la clase 'Estudiante' para agregar dicha instancia a la lista de estudiantes, la
cual es un atributo de la clase Curso.


## 2. Generación de código a partir del diagrama. 

a) Crear clases

b) Crear relaciones

c) Crear main (para probar el sistema).

Solución: https://github.com/Lmrocio/Practica_5.1_Entornos/blob/main/parte2.kt
