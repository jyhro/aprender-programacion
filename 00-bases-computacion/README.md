# Módulo 0 - Bases de la Computación

> Para quien nunca ha programado. Sin palabras raras. Si algo suena técnico, lo explicamos con un ejemplo de la vida real.

## Cómo usar este módulo

Todo el módulo usa 3 técnicas probadas para aprender. Son medibles: siempre sabrás tu puntaje.

1. **Predice antes de ver.** Adivina el resultado por escrito antes de probar. Medida: acertaste o no.
2. **Recuerda sin mirar.** Tapa la sección y explícala en voz alta. Medida: puntos sobre el total (por ejemplo 3 de 3).
3. **Repite espaciado.** Vuelve en 1, 3 y 7 días solo a lo que fallaste. Medida: lista de pendientes que se acorta.

> [!TIP]
> Regla de avance: no pases al Módulo 1 hasta sacar 8 de 10 en el repaso final (punto 0.8). Si sacas menos, el mismo 0.8 te dice qué repetir y cuándo.

## Índice

- [Cómo usar este módulo](#cómo-usar-este-módulo)
- [0.1 La computadora es como una cocina](#01-la-computadora-es-como-una-cocina)
- [0.2 Todo son ceros y unos](#02-todo-son-ceros-y-unos)
- [0.3 Archivos y carpetas](#03-archivos-y-carpetas)
- [0.4 La terminal no muerde](#04-la-terminal-no-muerde)
- [0.5 Internet en una frase](#05-internet-en-una-frase)
- [0.6 Cómo vamos a aprender](#06-cómo-vamos-a-aprender)
- [0.7 Palabras que verás mucho](#07-palabras-que-verás-mucho)
- [0.8 Repaso final medible](#08-repaso-final-medible)

## 0.1 La computadora es como una cocina

Imagina una cocina:

- **CPU:** el chef que hace el trabajo paso a paso.
- **RAM:** la mesa donde pones lo que usas ahora mismo.
- **Disco:** la alacena donde guardas todo para después.
- **Software:** las recetas que el chef sigue.
- **Sistema operativo:** el jefe de cocina que decide quién usa qué.

```text
TU COMPU
CPU (chef) + RAM (mesa) -> trabajo de ahora
Disco (alacena) + Software (recetas) -> trabajo guardado
```

> [!TIP]
> Mide tu avance (2 min): tapa la lista y di en voz alta qué es CPU, RAM y disco. Cada acierto vale 1 punto. 3 de 3 es listo. Lo que falles, apúntalo para el repaso del día 3.

## 0.2 Todo son ceros y unos

La compu solo entiende prendido y apagado, como un foco:

- **Bit:** un foquito (`1` es prendido, `0` es apagado).
- **Byte:** 8 foquitos juntos. Guarda 1 letra.

```text
Bits: 1 0 1 0 0 0 0 1 = 1 byte = la letra "A"
```

Python traduce esto por ti. Tú escribes `A` y la compu guarda `01000001`.

### Tamaños KB, MB y GB

Es solo contar bytes juntos, como contar monedas:

| Unidad | Equivale a | Ejemplo |
| --- | --- | --- |
| Byte | 1 letra | `A` |
| KB | 1.000 bytes | Un párrafo |
| MB | 1.000 KB | Una foto |
| GB | 1.000 MB | Un video corto |

Quédate con una idea: mientras más grande el archivo, más bytes ocupa.

### El mismo truco para todo

- **Texto:** cada letra tiene su código. `A` es `01000001`, `B` es `01000010`.
- **Números:** también son foquitos. Por eso `"5"` como texto no es igual a `5` para sumar. Python te deja convertirlos.
- **Fotos:** millones de puntitos de colores. Más puntitos es foto más pesada.
- **Verdadero o falso:** 1 foquito. `1` es sí, `0` es no. Así nacen los booleanos.

> [!TIP]
> Mide tu avance (3 min): primero predice por escrito qué pesa más, un mensaje de "hola" o una selfie. Luego tapa la tabla y ordena de menor a mayor Byte, KB, MB y GB. Predicción registrada vale 1 punto y orden perfecto vale 2. Total 3 puntos.

## 0.3 Archivos y carpetas

Todo lo que guardas vive en archivos dentro de carpetas:

- **Ruta:** la dirección del archivo, como `Documentos/fotos/playa.jpg`.
- **Extensión:** lo que va después del punto (`.jpg`, `.py`, `.txt`). Le dice a la compu qué tipo de cosa es.
- **Regla de oro:** un archivo `.py` es solo texto con instrucciones para Python.

```text
Documentos/
  fotos/
    playa.jpg
  aprender-programacion/
    hola.py
```

> [!TIP]
> Mide tu avance (5 min): crea la carpeta `python` y dentro el archivo `hola.py`. Luego tapa esta sección y escribe de memoria una ruta con 2 carpetas y su extensión. Carpeta creada vale 1 punto y ruta correcta vale 1 punto. Total 2 puntos.

## 0.4 La terminal no muerde

La terminal es pedirle cosas a la compu con texto en vez de clicks. Solo necesitas 4 comandos:

```bash
pwd              # dónde estoy
ls               # qué hay aquí
cd python        # entrar a la carpeta python
python3 hola.py  # correr tu programa
```

- **Proceso:** un programa corriendo. Nace, hace su trabajo y termina.
- **VS Code:** tu cuaderno para escribir código, con colores y ayuda.

> [!TIP]
> Mide tu avance (3 min): antes de correr cada comando, escribe qué crees que mostrará. Cada predicción escrita vale 1 punto aunque falles, y cada acierto suma 1 más. Máximo 4 puntos si predices 2 comandos.

## 0.5 Internet en una frase

Tu compu le pide cosas a otra compu, como pedir comida a domicilio:

1. Tú pides: dame el video.
2. El servidor responde con datos, muchas veces en formato `JSON`.

No necesitas más por ahora.

> [!TIP]
> Mide tu avance (1 min): tapa la lista y explica con tus palabras quién pide y quién responde. Explicación completa vale 1 punto.

## 0.6 Cómo vamos a aprender

Ideas adaptadas de la [guía de Platzi para aprender a programar desde cero](https://platzi.com/blog/como-aprender-a-programar/):

1. Piérdele el miedo a escribir código. Copia, corre, rompe y arregla.
2. Piensa en recetas. Antes de programar, explica los pasos en español.
3. Practica en chiquito. Veinte minutos escribiendo valen más que dos horas mirando.
4. Los errores son normales. Lee el mensaje con calma, te dice dónde mirar.
5. Haz un mini-proyecto tuyo, como tu presupuesto o tu lista de juegos.

> [!TIP]
> Mide tu avance (3 min): escribe en 5 líneas los pasos para preparar un sándwich. Ese es tu primer algoritmo. Cinco pasos ordenados valen 1 punto.

## 0.7 Palabras que verás mucho

- **Programa:** receta que la compu sigue.
- **Sintaxis:** reglas de escritura. Si te equivocas, la compu te avisa.
- **Variable:** cajita con nombre donde guardas algo, como `ahorro = 200`.
- **Lista:** varias cajitas en fila.
- **Función:** máquina que hace algo cada vez que la llamas.
- **Condicional:** si pasa esto, haz esto.
- **Bucle:** repite hasta que termine.

> [!TIP]
> Mide tu avance (4 min): tapa las definiciones y define los 7 términos en voz alta. De 6 a 7 bien vale 4 puntos, de 4 a 5 vale 2 puntos, menos es 0. Anota tu puntaje, lo usarás en el repaso final.

## 0.8 Repaso final medible

Hazlo sin mirar el resto del módulo. Suma tus puntos al final.

### Práctica 1 - Qué pesa más (2 puntos)

1. Observa: un mensaje que diga `hola` y una selfie de tu compu o celular.
2. Pregunta: ¿cuál ocupa más bytes?
3. Escribe tu hipótesis antes de medir (1 punto por dejarla escrita).
4. Mide: mira el tamaño de cada archivo con propiedades o `ls -l` y anota los dos tamaños (1 punto por anotar ambos).
5. Conclusión en una frase: el texto son poquitos bytes y la foto son millones.

### Práctica 2 - La extensión manda (2 puntos)

Trabaja sobre una copia, nunca sobre el original.

1. Observa: copia `hola.py` como `hola-copia.py`.
2. Pregunta: ¿qué pasa si le cambio la extensión a `.txt`?
3. Escribe tu hipótesis: qué crees que cambiará (1 punto por dejarla escrita).
4. Experimento: renombra la copia a `hola-copia.txt` e intenta abrirla.
5. Anota qué cambió y qué siguió igual (1 punto por anotar ambas cosas).

### Práctica 3 - Predice la terminal (2 puntos)

1. Abre la terminal dentro de la carpeta del repo.
2. Escribe qué mostrarán `pwd` y `ls` antes de correrlos (1 punto por predicción escrita).
3. Corre ambos comandos y compara línea por línea (1 punto por comparación anotada).
4. Si algo no coincidió, escribe por qué en una frase.

### Auto-test de vocabulario (4 puntos)

Sin mirar el punto 0.7, define los 7 términos. Usa la misma escala de ese punto: de 6 a 7 bien son 4 puntos, de 4 a 5 son 2 puntos, menos es 0.

### Tu puntaje y qué hacer

| Puntaje | Significa | Qué hacer |
| --- | --- | --- |
| 8 a 10 | Listo | Pasa al Módulo 1 |
| 5 a 7 | Casi | Repite mañana solo las prácticas falladas |
| 0 a 4 | Relee | Relee el módulo pasado mañana y repite el repaso |

### Plan de repaso espaciado

- [ ] Día 1: repaso final completo y puntaje anotado.
- [ ] Día 3: solo recuerdo sin mirar de lo que fallaste.
- [ ] Día 7: repite las 3 prácticas en 15 minutos.

## Siguiente paso

Pasa al Módulo 1 cuando tu puntaje sea de 8 o más, donde escribirás tu primera receta en forma de programa.
