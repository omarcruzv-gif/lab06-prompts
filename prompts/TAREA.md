# TAREA INDIVIDUAL: Diseño de un prompt profesional

## 1. Funcionalidad seleccionada

**Sistema de registro de préstamos de libros en una biblioteca escolar.**

La funcionalidad elegida consiste en desarrollar un programa de consola en Java que permita registrar y consultar información de los préstamos de libros realizados por los estudiantes.

El sistema almacenará el nombre del estudiante, el título del libro, la fecha del préstamo y la fecha de devolución.

Elegí esta funcionalidad porque permite aplicar conceptos básicos de programación orientada a objetos y desarrollar una solución sencilla mediante Java.

## 2. Evolución del prompt

### 2.1. Versión 1 (v1): Prompt básico

**Prompt utilizado:**

```text
Crea un programa en Java para registrar préstamos de libros.
```

**¿Qué cambié?**

En esta primera versión utilicé una instrucción sencilla y directa. Solamente indiqué que necesitaba un programa en Java para registrar préstamos de libros.

**¿Por qué lo cambié?**

Esta primera prueba me permitió observar cómo interpreta la inteligencia artificial una solicitud general, sin proporcionarle información adicional sobre el funcionamiento del sistema.

**¿Qué mejoró en la respuesta?**

Obtuve un programa funcional que permitía ingresar el nombre del libro, el estudiante y las fechas del préstamo y devolución. Sin embargo, el código era básico y no utilizaba programación orientada a objetos.

### 2.2. Versión 2 (v2): Rol y contexto

**Prompt utilizado:**

```text
Actúa como desarrollador Java. Necesito desarrollar un sistema de consola para gestionar préstamos de libros en una biblioteca escolar.

El programa debe permitir registrar los datos del estudiante, el nombre del libro, la fecha del préstamo y la fecha de devolución. También debe mostrar en pantalla la información del préstamo registrado.

Utiliza Java y Scanner para ingresar los datos. Mantén el código sencillo y comprensible para un estudiante que está aprendiendo programación.
```

**¿Qué cambié?**

Agregué el rol de desarrollador Java, el contexto de una biblioteca escolar y las instrucciones específicas sobre los datos que debía registrar el programa.

**¿Por qué lo cambié?**

La primera versión no explicaba dónde se utilizaría el sistema ni qué información debía manejar. Por eso, necesitaba proporcionar más contexto y definir mejor el objetivo.

**¿Qué mejoró en la respuesta?**

El código presentó una estructura más organizada, comentarios explicativos y una interfaz de consola más clara. Sin embargo, todavía utilizaba únicamente el método principal `main`, sin implementar una clase específica para representar los préstamos.

### 2.3. Versión 3 (v3): Rol, contexto, instrucciones, ejemplos y formato

**Prompt utilizado:**

```text
Actúa como desarrollador Java especializado en programación orientada a objetos.

Necesito desarrollar un sistema de consola para gestionar préstamos de libros en una biblioteca escolar. El sistema será utilizado por un bibliotecario para registrar y consultar los préstamos realizados por los estudiantes.

El programa debe utilizar una clase llamada Prestamo con los atributos estudiante, libro, fechaPrestamo y fechaDevolucion. Debe permitir ingresar los datos de un préstamo y mostrar la información registrada.

Ejemplo: si se registra un préstamo para el estudiante "Ana Pérez", del libro "El Principito", con fecha de préstamo "12/11/2026" y fecha de devolución "19/11/2026", el programa debe mostrar correctamente toda esa información.

Restricciones:
- Utiliza Java y programación orientada a objetos.
- No utilices librerías externas.
- Utiliza Scanner para ingresar los datos.
- Mantén el código sencillo y comprensible para un estudiante que está aprendiendo Java.

Formato de respuesta:
Presenta primero una breve explicación de la clase Prestamo, sus atributos y su función. Después muestra el código Java completo y finalmente un ejemplo de ejecución.
```

**¿Qué cambié?**

Incorporé una clase llamada `Prestamo`, definí sus cuatro atributos y especifiqué que debía utilizar programación orientada a objetos. También agregué un ejemplo concreto, restricciones y un formato para presentar la respuesta.

**¿Por qué lo cambié?**

Necesitaba que el programa tuviera una estructura más organizada y que la inteligencia artificial comprendiera exactamente cómo debía desarrollar la solución.

**¿Qué mejoró en la respuesta?**

La respuesta implementó una clase independiente llamada `Prestamo`, un constructor y el método `mostrarInformacion()`. De esta manera, el programa comenzó a aplicar los conceptos de programación orientada a objetos.

## 3. Prompt final profesional

Después de analizar las tres versiones anteriores, elaboré una última versión incorporando los cinco componentes de un prompt profesional.

**Prompt final:**

```text
ROL:
Actúa como desarrollador Java especializado en programación orientada a objetos y con experiencia enseñando programación a principiantes.

INSTRUCCIÓN:
Desarrolla un sistema de consola en Java para registrar y consultar préstamos de libros en una biblioteca escolar.

CONTEXTO:
El sistema será utilizado por un bibliotecario que necesita llevar un control organizado de los préstamos realizados por los estudiantes.

El programa debe utilizar una clase llamada Prestamo con los siguientes atributos:
- estudiante
- libro
- fechaPrestamo
- fechaDevolucion

Debe incluir un constructor, métodos getters y setters y un método mostrarInformacion() para visualizar los datos del préstamo.

El programa principal debe utilizar Scanner para ingresar la información y crear un objeto de tipo Prestamo.

EJEMPLO:
Si se registra un préstamo con los siguientes datos:

Estudiante: Ana Pérez
Libro: El Principito
Fecha de préstamo: 12/11/2026
Fecha de devolución: 19/11/2026

El programa debe mostrar toda la información correctamente.

RESTRICCIONES:
- Utiliza únicamente Java y sus librerías estándar.
- No utilices librerías externas.
- Mantén el código sencillo y comprensible para un estudiante principiante.
- Utiliza atributos privados para aplicar encapsulamiento.
- No agregues funcionalidades que no hayan sido solicitadas.

FORMATO DE RESPUESTA:
1. Explica brevemente la estructura de la clase Prestamo.
2. Describe la función de sus atributos y métodos.
3. Presenta el código Java completo.
4. Muestra un ejemplo de ejecución en consola.
5. Explica brevemente cómo funciona el programa.
```

## 4. Identificación de los cinco componentes

| Componente | Identificación dentro del prompt | Función |
|---|---|---|
| Rol | Desarrollador Java especializado en programación orientada a objetos. | Define el perfil que debe asumir la IA. |
| Instrucción | Desarrollar un sistema de consola para registrar préstamos. | Explica qué se necesita desarrollar. |
| Contexto | Sistema utilizado por un bibliotecario en una biblioteca escolar. | Proporciona información sobre el entorno y la necesidad. |
| Ejemplos | Registro de Ana Pérez y el libro El Principito. | Muestra un caso concreto de funcionamiento. |
| Formato | Explicación, estructura, código y ejemplo de ejecución. | Organiza la presentación de la respuesta. |

## 5. Restricciones del prompt final

Se establecieron las siguientes restricciones para orientar correctamente la solución:

- Utilizar Java y sus librerías estándar.
- No incorporar librerías externas.
- Mantener un nivel de programación adecuado para principiantes.
- Aplicar encapsulamiento mediante atributos privados.
- Evitar funcionalidades adicionales que no hayan sido solicitadas.

Estas restricciones permiten obtener una solución sencilla, comprensible y relacionada directamente con el objetivo del programa.

## 6. Evaluación del resultado final

| Criterio de evaluación | Resultado |
|---|---|
| ¿El prompt define un rol específico? | Sí |
| ¿La instrucción explica claramente qué se necesita desarrollar? | Sí |
| ¿Incluye un contexto de utilización? | Sí |
| ¿Presenta un ejemplo concreto? | Sí |
| ¿Establece restricciones? | Sí |
| ¿Indica el formato de respuesta? | Sí |
| ¿El código utiliza una clase Prestamo? | Sí |
| ¿Implementa constructor, getters y setters? | Sí |
| ¿Aplica encapsulamiento? | Sí |
| ¿Presenta explicación y ejemplo de ejecución junto con el código? | No, no aparecen en la respuesta compartida |

## 7. Errores frecuentes y cómo los evité

### Error 1: Ser demasiado general

En la primera versión solamente solicité un programa para registrar préstamos de libros. Esta instrucción no especificaba la estructura ni las características necesarias.

**¿Cómo lo evité?**

En las siguientes versiones agregué información sobre el funcionamiento del sistema, los datos que debía registrar y la utilización de una clase específica llamada `Prestamo`.

### Error 2: No indicar el formato

Inicialmente no indiqué cómo quería recibir la solución, por lo que la respuesta solamente presentaba el código sin una explicación de su estructura.

**¿Cómo lo evité?**

En la tercera versión y en el prompt final establecí un formato de respuesta que solicita explicar primero la clase, presentar después el código Java y finalmente mostrar un ejemplo de ejecución.

## 8. Conclusiones

1. La elaboración de un prompt profesional requiere proporcionar instrucciones claras y específicas para obtener mejores resultados.

2. La incorporación de un rol y un contexto permite orientar a la inteligencia artificial hacia una necesidad concreta.

3. Los ejemplos ayudan a explicar de manera práctica el resultado que se espera obtener.

4. Las restricciones permiten controlar la complejidad de las respuestas y evitar funcionalidades innecesarias.

5. La iteración de prompts permite identificar errores, mejorar las instrucciones y obtener soluciones más organizadas y precisas.

## 9. Evidencia de publicación

**Repositorio:** lab06-prompts.

**Archivo:** `prompts/TAREA.md`.

La publicación se realizará mediante Git y GitHub, incluyendo la actualización del README principal y los commits correspondientes.