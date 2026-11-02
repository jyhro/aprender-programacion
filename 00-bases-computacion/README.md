# Módulo 0 - Bases de la Computación

> Para quien nunca ha programado. Sin palabras raras. Si algo suena técnico, lo explicamos con un ejemplo de la vida real.

## Cómo usar este módulo

Todo el módulo usa 3 técnicas probadas para aprender. Son medibles: siempre sabrás tu puntaje.

1. **Predice antes de ver.** Adivina el resultado por escrito antes de probar. Medida: predicción registrada (vale puntos aunque falle) más acierto.
2. **Recuerda sin mirar.** Cada sección cierra con "Mide tu avance": tapar y explicar en voz alta. Medida: puntos sobre total explícito (por ejemplo 3 de 3).
3. **Repite espaciado.** Vuelve en 1, 3 y 7 días solo a lo que fallaste. Medida: lista de pendientes que se acorta.

Anota todo en [NOTAS.md](./NOTAS.md), tu diario del módulo. Cada sección tiene un "Investiga" que termina ahí. Sin notas no hay puntos.

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

Todo lo que hace tu compu sigue el mismo ciclo: **entra algo, se procesa y sale algo**.

```text
ENTRADA -> PROCESO -> SALIDA
teclado, mouse -> CPU -> pantalla, bocinas
```

Ejemplo: presionas `A` (entrada), la CPU decide qué hacer (proceso) y la letra aparece en pantalla (salida). Programar es escribir las reglas del paso del medio.

Imagina la cocina:

- **CPU:** el chef que hace el trabajo paso a paso. Mientras más rápido el chef, más rápido todo.
- **RAM:** la mesa donde pones lo que usas ahora mismo. Se vacía al apagar.
- **Disco:** la alacena donde guardas todo para después. Lo guardado sobrevive al apagado.
- **Software:** las recetas que el chef sigue. Sin recetas, la cocina no produce nada.
- **Sistema operativo:** el jefe de cocina que decide quién usa qué. Ejemplos: Windows, macOS, Linux.

Diferencia clave para no confundirte: lo que está **abierto ahora** vive en la RAM, lo que está **guardado** vive en el disco.

### Investiga

Abre la información de tu compu (en macOS: menú manzana, Acerca de esta Mac; en Windows: Configuración, Sistema, Acerca de) y anota en `NOTAS.md`: modelo de CPU, GB de RAM, espacio libre en disco, sistema operativo y versión. Luego clasifica 3 programas que uses a diario: ¿cuáles son sistema operativo y cuáles son aplicaciones?

### Mide tu avance

Tapa la lista y di en voz alta qué es CPU, RAM y disco, más el ciclo entrada-proceso-salida con un ejemplo. Cada acierto vale 1 punto, total 4. Los specs anotados en `NOTAS.md` valen 1 punto extra. Lo que falles, apúntalo para el repaso del día 3.

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

### Investiga

Elige 3 archivos tuyos (un texto, una foto y un video o audio), mira su tamaño real y anota en `NOTAS.md` cada nombre con su tamaño en KB, MB o GB. Ordénalos de menor a mayor y escribe si el orden coincide con lo que esperabas.

### Mide tu avance

Primero predice por escrito qué pesa más, un mensaje de "hola" o una selfie. Luego tapa la tabla y ordena de menor a mayor Byte, KB, MB y GB. Predicción registrada vale 1 punto y orden perfecto vale 2. Total 3 puntos.

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

### Ruta absoluta y ruta relativa

- **Absoluta:** la dirección completa desde la raíz, funciona desde cualquier lugar. Ejemplo: `/Users/tu-nombre/Documentos/fotos/playa.jpg`.
- **Relativa:** la dirección corta desde donde estás parado. Si ya estás en `Documentos`, basta con `fotos/playa.jpg`.

La terminal siempre está parada en alguna carpeta. Por eso el mismo archivo se nombra distinto según desde dónde lo pidas.

### Permisos en una frase

Cada archivo dice quién puede **leerlo** (abrirlo), **escribirlo** (cambiarlo) y **ejecutarlo** (correrlo como programa). Si un día no te deja guardar algo, casi siempre es un permiso, no un archivo roto.

### Investiga

Anota en `NOTAS.md` 3 rutas reales de tu compu (usa el explorador o `pwd` más `ls`). Marca cuál es absoluta y escribe la versión relativa de al menos una. Para una de ellas, anota su extensión y qué programa la abre.

### Mide tu avance

Crea la carpeta `python` y dentro el archivo `hola.py`. Luego tapa esta sección y escribe de memoria la ruta absoluta de ese archivo. Carpeta más archivo creados vale 1 punto y ruta absoluta correcta vale 1 punto. Total 2 puntos.

## 0.4 La terminal no muerde

La terminal es pedirle cosas a la compu con texto en vez de clicks. Con estos comandos haces el 90 por ciento del módulo:

```bash
pwd              # dónde estoy parado
ls               # qué hay aquí
cd python        # entrar a la carpeta python
cd ..            # volver una carpeta atrás
mkdir pruebas    # crear una carpeta
python3 hola.py  # correr tu programa
clear            # limpiar la pantalla
```

Tres ayudas que te ahorran tiempo:

- **Tab** autocompleta nombres. Escribe `cd py` más Tab y la terminal completa `python`.
- **Flecha arriba** repite el comando anterior. Úsala en vez de reescribir.
- **Borrar con `rm`** no tiene papelera. Úsalo solo en carpetas de prueba que tú creaste.

Un flujo completo se ve así:

```bash
mkdir python
cd python
echo "print('hola')" > hola.py
python3 hola.py
```

### Investiga

Corre `ls ~` (el contenido de tu carpeta personal), anota en `NOTAS.md` 5 carpetas que veas y qué crees que guardan. Prueba Tab con `cd` y la flecha arriba, y anota qué hizo cada una con tus palabras.

### Mide tu avance

Antes de correr `pwd` y `ls`, escribe qué crees que mostrará cada uno. Cada predicción escrita vale 1 punto aunque falles, y cada acierto suma 1 más. Máximo 4 puntos con 2 comandos.

## 0.5 Internet en una frase

Tu compu le pide cosas a otra compu, como pedir comida a domicilio:

1. Tú pides: dame el video.
2. El servidor responde con datos, muchas veces en formato `JSON`.

No necesitas más por ahora, pero sí entender las 3 partes de una dirección web:

| Parte | Ejemplo en `https://github.com/jyhro/aprender-programacion` | Para qué sirve |
| --- | --- | --- |
| Protocolo | `https` | Cómo deben hablar las compus |
| Dominio | `github.com` | A qué compu le pides (la agenda que traduce nombres a números se llama DNS) |
| Ruta | `/jyhro/aprender-programacion` | Qué cosa exacta le pides |

Y así se ve el formato `JSON`, solo texto ordenado con nombres y valores:

```json
{
  "nombre": "Ana",
  "edad": 20,
  "estudia": true
}
```

Python entiende este formato sin esfuerzo, por eso lo verás mucho más adelante.

### Investiga

Descompón en `NOTAS.md` 2 direcciones reales (la de este repo en GitHub y una que uses a diario) en protocolo, dominio y ruta. Anota en una frase qué crees que le estás pidiendo al servidor en cada una.

### Mide tu avance

Tapa la tabla y explica quién pide y quién responde, más las 3 partes de una URL con un ejemplo inventado. Explicación del pedido vale 1 punto y URL descompuesta bien vale 1 punto. Total 2 puntos.

## 0.6 Cómo vamos a aprender

Ideas adaptadas de la [guía de Platzi para aprender a programar desde cero](https://platzi.com/blog/como-aprender-a-programar/):

1. Piérdele el miedo a escribir código. Copia, corre, rompe y arregla.
2. Piensa en recetas. Antes de programar, explica los pasos en español.
3. Practica en chiquito. Veinte minutos escribiendo valen más que dos horas mirando.
4. Los errores son normales. Lee el mensaje con calma, te dice dónde mirar.
5. Haz un mini-proyecto tuyo, como tu presupuesto o tu lista de juegos.

> [!TIP]
> Mide tu avance (3 min): escribe en 5 líneas los pasos para preparar un sándwich. Ese es tu primer algoritmo. Cinco pasos ordenados valen 1 punto. Guárdalo en `NOTAS.md`.

## 0.7 Palabras que verás mucho

- **Programa:** receta que la compu sigue. Ejemplo: `hola.py`.
- **Sintaxis:** reglas de escritura. Si te equivocas, la compu te avisa con un error.
- **Variable:** cajita con nombre donde guardas algo, como `ahorro = 200`.
- **Lista:** varias cajitas en fila, como `["pan", "queso", "jamón"]`.
- **Función:** máquina que hace algo cada vez que la llamas, para no repetir código.
- **Condicional:** si pasa esto, haz esto. Ejemplo: si tienes hambre, come.
- **Bucle:** repite hasta que termine. Ejemplo: mientras haya platos sucios, lava.

> [!TIP]
> Mide tu avance (4 min): tapa las definiciones y define los 7 términos en voz alta con un ejemplo cada uno. De 6 a 7 bien vale 4 puntos, de 4 a 5 vale 2 puntos, menos es 0. Anota tu puntaje en `NOTAS.md`, lo usarás en el repaso final.

## 0.8 Repaso final medible

Hazlo sin mirar el resto del módulo. Suma tus puntos al final. Todo queda anotado en `NOTAS.md`.

### Práctica 1 - Qué pesa más y dónde vive (2 puntos)

1. Observa: el mensaje `hola` y una selfie de tu compu o celular.
2. Pregunta: ¿cuál ocupa más bytes y dónde vive cada uno, en RAM o en disco?
3. Escribe tu hipótesis antes de medir (1 punto por dejarla escrita).
4. Mide: mira el tamaño de cada archivo con propiedades o `ls -l` y anota ambos tamaños más dónde vive cada uno (1 punto por anotación completa).
5. Conclusión en una frase: el texto son poquitos bytes en disco y la foto son millones.

### Práctica 2 - La extensión y la ruta mandan (2 puntos)

Trabaja sobre una copia, nunca sobre el original.

1. Observa: copia `hola.py` como `hola-copia.py` dentro de `python`.
2. Pregunta: ¿qué pasa si le cambio la extensión a `.txt` y la pido con ruta relativa?
3. Escribe tu hipótesis: qué cambiará al abrirla y cuál es su ruta absoluta (1 punto por dejarla escrita).
4. Experimento: entra a la carpeta con `cd`, renombra la copia a `hola-copia.txt` e intenta abrirla.
5. Anota qué cambió, qué siguió igual y la ruta absoluta (1 punto por anotación completa).

### Práctica 3 - Predice la terminal y la web (2 puntos)

1. Abre la terminal dentro de la carpeta del repo.
2. Escribe qué mostrarán `pwd` y `ls` antes de correrlos (1 punto por predicción escrita).
3. Corre ambos comandos y compara línea por línea con tu predicción.
4. Descompón la URL de este repo en GitHub en protocolo, dominio y ruta, sin mirar el punto 0.5 (1 punto por descomposición correcta).

### Auto-test de vocabulario (4 puntos)

Sin mirar el punto 0.7, define los 7 términos con un ejemplo cada uno. Usa la misma escala de ese punto: de 6 a 7 bien son 4 puntos, de 4 a 5 son 2 puntos, menos es 0.

### Tu puntaje y qué hacer

| Puntaje | Significa | Qué hacer |
| --- | --- | --- |
| 8 a 10 | Listo | Pasa al Módulo 1 |
| 5 a 7 | Casi | Repite mañana solo las prácticas falladas |
| 0 a 4 | Relee | Relee el módulo pasado mañana y repite el repaso |

### Plan de repaso espaciado

- [ ] Día 1: repaso final completo y puntaje anotado en `NOTAS.md`.
- [ ] Día 3: solo recuerdo sin mirar de lo que fallaste.
- [ ] Día 7: repite las 3 prácticas en 15 minutos.

## Siguiente paso

Pasa al Módulo 1 cuando tu puntaje sea de 8 o más, donde escribirás tu primera receta en forma de programa.
