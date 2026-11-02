# Aprender Programación

Repo de aprendizaje desde cero: primero bases de computación, luego fundamentos (lógica, algoritmos, estructuras), luego Python aplicado con ejercicios.

## Ruta

### 0. Bases de la Computación
Cómo funciona una computadora y el entorno donde correrán tus programas.
1. La computadora: hardware (CPU, memoria RAM, almacenamiento) y software (SO, apps) → conecta con 1.1 (qué es programar) y Python 1 (instalación/entorno).
2. Datos y binario: bits/bytes, cómo se representa texto, números e imágenes → conecta con 2.2 (tipos de datos) y Python 2/6 (casting, archivos).
3. Sistema operativo y archivos: carpetas, rutas, extensiones, permisos básicos → conecta con Python 1/6 (ejecutar `.py`, leer/escribir archivos).
4. Terminal y herramientas: comandos básicos, VS Code, qué es un programa en ejecución (proceso) → conecta con Python 1 (terminal, primer script) y 6.1 (errores).
5. Redes e internet (visión general): qué es una red, cliente/servidor, nube → conecta con Python 6.2 (JSON como intercambio de datos).
6. Seguridad e higiene digital: contraseñas, backups, qué no romper → conecta con 6.1 (código robusto que no colapsa).

### 1. Introducción a la Programación
1. Fundamentos de la Computación y la Lógica: qué es programar, hardware/software, pensamiento algorítmico, diagramas de flujo, pseudocódigo (PSeInt), lenguajes y compiladores/intérpretes.
2. Elementos Básicos: variables/constantes, tipos primitivos, operadores, entrada/salida.
3. Control de Flujo: condicionales (if/else/elif/switch), bucles (while/do-while/for, break/continue).
4. Estructuras de Datos: arreglos/listas, matrices, cadenas como arreglos.
5. Modularidad: funciones/procedimientos, parámetros, scope local vs global.
6. Paradigmas (visión general): estructurada y POO (clase, objeto, atributos, métodos, encapsulamiento/herencia/polimorfismo).

### 2. Programación con Python
1. Setup: ecosistema Python, instalación, terminal, VS Code, primer script (`print`, comentarios).
2. Datos y Variables: tipado dinámico, `snake_case`, `int/float/str/bool`, casting, operadores, `input()`.
3. Control de Flujo: `if/elif/else` + indentación, `while`, `for`, `range()`, `break/continue`.
4. Colecciones: `list` (append/insert/remove/pop, slicing), `tuple`, `dict`, `set`.
5. Funciones: `def/return`, args posicionales y por keyword, scope, docstrings.
6. Errores y Archivos: `try/except`, lectura/escritura `.txt`, intro a JSON.
7. POO práctica: `class`, instancias, `__init__`/`self`, atributos y métodos.
8. Proyecto Final Aplicado.

## Ejercicios

- 2.1 Calculadora de Presupuesto Mensual: ingreso bruto → 20% ahorro, 50% fijos, 30% libres.
- 2.2 Conversor de Divisas: constante de tipo de cambio, `input` + casting.
- 3.1 Validador de Acceso: edad + ID (`and/or/not`).
- 3.2 Impuestos Progresivos: <20k 0%, 20k–50k 15%, >50k 25% (sobre excedente) con `elif`.
- 3.3 Inventario con `while`: stock inicial 50, retiros, control de insuficiente, fin en 0.
- 3.4 Reporte de Ventas con `for/range()`: N días, suma total.

## Seguimiento

Ver [CHECKLIST.md](./CHECKLIST.md).

## Convención

Un script por ejercicio en `python/`, p. ej. `python/ejercicio_2_1.py`.
