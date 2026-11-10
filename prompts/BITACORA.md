# Bitacora de prompts

Laboratorio 06: Fundamentos de Ingenieria de Prompts.

Herramienta de IA usada: ChatGPT

## Ejercicio 2: Tokens y ventana de contexto

| Texto | Caracteres | Tokens |
|---|---:|---:|
| Los estudiantes programan en Java. | 34 | 7 |
| The students program in Java. | 29 | 6 |
| desafortunadamente | 18 | 4 |


## Ejercicio 3: Temperatura


| Temperatura | % de BiblioTec | Nombres en los 5 intentos |
|---|---|---|
| 0 | 100.0% | BiblioTec, LibroYa, PrestaLibro, LectoGo, PaginaLibre, NubeDeTinta |
| 0.5 | 65.3% | BiblioTec, LibroYa, PrestaLibro, LectoGo, PaginaLibre, NubeDeTinta |
| 1 | 44.5% | BiblioTec, LibroYa, PrestaLibro, LectoGo, PaginaLibre, NubeDeTinta  |
| 1.8 | 32.2% | BiblioTec, LibroYa, PrestaLibro, LectoGo, PaginaLibre, NubeDeTinta |

## Ejercicio 4: Prompt vago vs estructurado

| Criterio | Prompt vago | Prompt estructurado |
|	|	|	|
| Menciona el objetivo del sistema | No | Si |
| Menciona a los usuarios principales | No | Si |
| Tiene exactamente 3 funcionalidades | No | Si |
| Esta en 3 parrafos | No | Si |
| Lo usaria en un informe real | No | Si |

## Ejercicio 5: Anatomia de un prompt

| Componente | Texto de mi prompt |
|------------|--------------------|
| Rol | Java Sennior Developer |
| Instruccion | Create a Java program |
| Contexto | Managing products on a virtual store |
| Ejemplo | Using a Product class with the attributes Code, Name, Price, Stock |
| Formato | Methods:  getPrice(), setPrice(double price) |