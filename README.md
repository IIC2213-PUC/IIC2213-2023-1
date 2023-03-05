# IIC2213 - Lógica para ciencia de la computación

## 2023-1

Bienvenidos al sitio web del curso de Lógica para ciencia de la computación. En esta página podrás encontrar la información administrativa del curso. En el repositorio podrás encontrar las diapositivas de clase, guías de ejercicios, enunciados y soluciones de ayudantías y evaluaciones.

## Tabla de contenidos

- [IIC2133 - Estructuras de Datos y Algoritmos](#iic2213---logica-para-ciencia-de-la-computacion)
  - [2023-1](#2023-1)
  - [Tabla de contenidos](#tabla-de-contenidos)
  - [Tareas](#tareas)
  - [Clases](#clases)
  - [Ayudantías](#ayudantías)
  - [Equipo](#equipo)
  - [Evaluación](#evaluación)
    - [Evaluaciones Escritas](#evaluaciones-escritas)
    - [Tareas](#tareas)
  - [Política de Atrasos](#política-de-atrasos)
  - [Política de integridad académica](#política-de-integridad-académica)


## Tareas

- T1
  - Contenidos: 
  - Enunciado
  - Recursos adicionales
  - Pauta

## Clases

|   Tipo    | Número | Tema | Fecha | Sección 1  |
| :-------: | :----: | :------------------------------------------: | :---: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | 
| Cátedra | 0 | Introducción | 2023-03-07 | aquí va el link |

  ## Ayudantías

|   Tipo    | Número | Tema | Encargade | Material   |
| :--- | :--- | :--- | :--- | :--- |
| Ayudantía | 0 | Sintaxis y semántica en lógica proposicional | Quién la hace | aquí va el link |


## Equipo

| Nombre  | Cargo | Email | Github |
| :-------------- | :------ | :---------------- | : ----------- |
| Sebastián Bugedo | Profe  | bugedo@uc.cl | [@seba-bug](https://github.com/seba-bug) |
| Sofía Errázuriz | Ayudante coordinadora  | sofiaerrazurizm@uc.cl | |
| Sebastián Hagedorn | Ayudante   | shagedorn@uc.cl | |
| Julián García | Ayudante   | jgarcg@uc.cl | |
| Matías Fernandez | Ayudante   | matias.fernandez@uc.cl | |

## Evaluación


### Evaluaciones Escritas

Habrá un único examen escrito que busca evaluar los contenidos esenciales del curso: _Lo que no puede faltar en un estudiante que aprueba el curso._

| Evaluación | Fecha |
| :-------------- | :--------- |
| Examen | 3 de julio (9:00) |

### Tareas

Habrá 7 tareas que buscan evaluar el avance de los contenidos del curso. Estas pueden incluir demostraciones teóricas, pseudocódigo, código python, código prolog, entre otras.



| Evaluación | Fecha Publicacion  | Fecha Entrega      | Plazo (días completos) |
| :--------- | :----------------- | :----------------- | : -- |
| Tarea 1    | Martes 14 de marzo | Lunes 27 de marzo | 13 |
| Tarea 2    | Martes 28 de marzo    | Miércoles 5 de abril    | 8 |
| Tarea 3    | Martes 11 de abril  | Martes 25 de abril  | 14 |
| Tarea 4    | Martes 9 de mayo  | Lunes 22 de mayo  | 13 |
| Tarea 5    | Martes 23 de mayo  | Lunes 5 de junio  | 13 |
| Tarea 6    | Martes 6 de junio  | Lunes 19 de junio  | 13 |
| Tarea 7    | Martes 20 de junio  | Viernes 30 de junio  | 10 |

La publicación será el día indicado, luego de la cátedra. La entrega será a las 23:59 del día indicado. Además se especifica la cantidad de días enteros (de 24 horas) de los que disponen para resolver cada tarea. ¡Planifiquen bien su tiempo!

La nota 

La nota final del curso se calcula de la siguiente manera:

```c++
double nota_final() {
  /* La nota de cada tarea */
  double T0, T1, T2, T3;
  /* La nota de cada interrogación*/
  double I1, I2, I3;

  /* Promedio de tareas */
  double NT = 0.20 * T0 + 0.30 * T1 + 0.25 * T2 + 0.25 * T3;
  /* Promedio de interrogaciones */
  double NI = 0.25 * I1 + 0.30 * I2 + 0.45 * I3;

  /* Nota final */
  double NF = (NT + NI) / 2;

  /* Es necesario tener sobre 3.7 en las evaluaciones escritas y las tareas por separado para aprobar el curso */
  if (NI < 3.7 || NT < 3.7) {
    return min(3.9, NF);
  } else {
    return min(NF, 7);
  }
}
```

## Política de Atrasos

La formula de atrasos es la siguiente:

```c++
  double nota_con_atraso(double nota, int dias_de_atraso){
    return max(1.0, nota - 0.7 * dias_de_atraso**1.3);
  }
```

## Política de integridad académica

Este curso se adscribe a la política de integridad académica de la Escuela de Ingeniería y el Departamento de Computación.

---

Los alumnos de la Escuela de Ingeniería de la Pontificia Universidad Católica de Chile deben mantener un comportamiento acorde a la Declaración de Principios de la Universidad. En particular, se espera que **mantengan altos estándares de honestidad académica**. Cualquier acto deshonesto o fraude académico está prohibido; los alumnos que incurran en este tipo de acciones se exponen a un Procedimiento Sumario. Es responsabilidad de cada alumno conocer y respetar el documento sobre Integridad Académica publicado por la Dirección de Docencia de la Escuela de Ingeniería (disponible en SIDING).

Específicamente, para los cursos del Departamento de Ciencia de la Computación, rige obligatoriamente la siguiente política de integridad académica. Todo trabajo presentado por un alumno para los efectos de la evaluación de un curso debe ser hecho individualmente por el alumno, sin apoyo en material de terceros. Por “trabajo” se entiende en general las interrogaciones escritas, las tareas de programación u otras, los trabajos de laboratorio, los proyectos, el examen, entre otros.

**En particular, si un alumno copia un trabajo, o si a un alumno se le prueba que compró o intentó comprar un trabajo, obtendrá nota final 1.1 en el curso y se solicitará a la Dirección de Docencia de la Escuela de Ingeniería que no le permita retirar el curso de la carga académica semestral.**

Por “copia” se entiende incluir en el trabajo presentado como propio, partes hechas por otra persona. **En caso que corresponda a “copia” a otros alumnos, la sanción anterior se aplicará a todos los involucrados**. En todos los casos, se informará a la Dirección de Docencia de la Escuela de Ingeniería para que tome sanciones adicionales si lo estima conveniente. Obviamente, está permitido usar material disponible públicamente, por ejemplo, libros o contenidos tomados de Internet, siempre y cuando se incluya la referencia correspondiente y sea autorizado por los ayudantes.

Lo anterior se entiende como complemento al Reglamento del Alumno de la Pontificia Universidad Católica de
Chile<sup><a name="pucCLBack">[1](#pucCL)</a></sup>. Por ello, es posible pedir a la Universidad la aplicación de sanciones adicionales especificadas en dicho reglamento.

<sub>**<a name="pucCL">[1](#pucCL)</a>**: Reglamento del Alumno de la Pontificia Universidad Católica de Chile disponible en: http://admisionyregistros.uc.cl/alumnos/informacion-academica/reglamentos-estudiantiles [&#8593;](#pucCLBack)</sub>
