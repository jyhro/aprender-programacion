# Módulo 1 - Lógica y algoritmos

> Aquí no se programa todavía. Se aprende a pensar como programa: pasos claros, sin adivinanzas. Todo se escribe primero a mano en español estructurado y al final se comprueba en PSeInt.

## Cómo usar este módulo

Todo el módulo usa 3 técnicas probadas para aprender. Son medibles: siempre sabrás tu puntaje.

1. **Predice antes de ver.** Adivina el resultado por escrito antes de probar. Medida: predicción registrada (vale puntos aunque falle) más acierto.
2. **Recuerda sin mirar.** Cada sección cierra con "Mide tu avance": tapar y explicar en voz alta. Medida: puntos sobre total explícito (por ejemplo 4 de 4).
3. **Repite espaciado.** Vuelve en 1, 3 y 7 días solo a lo que fallaste. Medida: lista de pendientes que se acorta.

Anota todo en [NOTAS.md](./NOTAS.md), tu diario del módulo. Cada sección tiene un "Investiga" que termina ahí. Sin notas no hay puntos.

> [!TIP]
> Regla de avance: no pases al Módulo 2 hasta sacar 8 de 10 en el repaso final (punto 1.6). PSeInt es solo la calculadora que comprueba tus pasos: pensar ocurre a mano.

## Índice

- [Cómo usar este módulo](#cómo-usar-este-módulo)
- [1.1 Qué es un algoritmo](#11-qué-es-un-algoritmo)
- [1.2 Español estructurado a mano](#12-español-estructurado-a-mano)
- [1.3 Diagramas de flujo](#13-diagramas-de-flujo)
- [1.4 Pseudocódigo y PSeInt](#14-pseudocódigo-y-pseint)
- [1.5 Palabras que verás mucho](#15-palabras-que-verás-mucho)
- [1.6 Repaso final medible](#16-repaso-final-medible)

## 1.1 Qué es un algoritmo

Un algoritmo es una lista ordenada de pasos que resuelve algo. Cocinar, cruzar la calle y sumar un mercado son algoritmos que ya usas sin darte cuenta.

Un buen algoritmo cumple 3 cualidades:

- **Tiene fin:** termina, no sigue para siempre.
- **Es preciso:** cada paso se entiende sin adivinar. "Echa un poco de sal" no sirve; "echa una cucharada" sí.
- **Da lo mismo con los mismos datos:** si repites los pasos con la misma entrada, sale el mismo resultado.

Ejemplo malo contra bueno:

- Malo: "haz café".
- Bueno: "hierve 500 ml de agua, echa 2 cucharadas de café en el filtro, vierte el agua, espera 4 minutos, sirve".

### Investiga

Elige una tarea de tu día (tender la cama, calentar comida, pagar un pasaje), cuenta sus pasos y anota en `NOTAS.md` cuáles son ambiguos. Reescribe esos pasos hasta que otra persona pueda seguirlos sin preguntar.

### Mide tu avance

Tapa la lista y di en voz alta qué es un algoritmo más sus 3 cualidades con un ejemplo. Definición vale 1 punto y cada cualidad 1 punto. Total 4 puntos.

## 1.2 Español estructurado a mano

Antes de cualquier herramienta, el algoritmo se escribe a mano con esta plantilla:

```text
ENTRADA: qué datos necesito
PROCESO: pasos en orden
SALIDA: qué resultado entrego
```

Solo necesitas 4 piezas para todo el módulo:

- **Hacer:** una acción. Ejemplo: hervir el agua.
- **Guardar:** meter un dato en una cajita. Ejemplo: total vale 0.
- **Decidir:** elegir un camino. Ejemplo: si llueve, lleva paraguas; si no, no lo lleves.
- **Repetir:** hacer algo varias veces. Ejemplo: mientras queden platos sucios, lava uno.

Ejemplo completo, promedio de 3 notas:

```text
ENTRADA: nota1, nota2, nota3
PROCESO:
  1. Sumar las 3 notas y guardar en suma
  2. Dividir suma entre 3 y guardar en promedio
  3. Si promedio es 60 o más, decir "aprobado"; si no, decir "reprobado"
SALIDA: promedio y el mensaje
```

### Tus 3 algoritmos (a mano, sin compu)

1. Preparar café para 2 personas con medidas exactas.
2. Decidir si sales con paraguas según el cielo y el pronóstico.
3. Sumar precios del mercado uno por uno hasta pasar de 1.000, y avisar con cuánto te pasaste.

Para cada uno llena la plantilla ENTRADA/PROCESO/SALIDA y haz una prueba de escritorio: una tablita donde sigues tus pasos con un ejemplo real y anotas qué vale cada dato en cada paso.

### Investiga

Escribe los 3 algoritmos en `NOTAS.md` y corre la prueba de escritorio de al menos uno con números de verdad. Si te trabas siguiendo tus propios pasos, el hueco está en el algoritmo: corrígelo ahí, no en tu cabeza.

### Mide tu avance

Cada algoritmo completo con su plantilla vale 1 punto, total 3. La prueba de escritorio anotada vale 1 punto extra. Total 4 puntos.

## 1.3 Diagramas de flujo

Un diagrama es el mismo algoritmo dibujado. Solo usa 5 figuras:

| Figura | Significa | Ejemplo |
| --- | --- | --- |
| Óvalo | Inicio o fin | Inicio |
| Paralelogramo | Leer o mostrar | Leer edad |
| Rectángulo | Hacer algo | Total vale total más precio |
| Rombo | Decidir | ¿Edad es 18 o más? |
| Flecha | Orden de los pasos | Va del paso 1 al 2 |

Ejemplo dibujado con texto, permiso para entrar:

```text
( Inicio ) -> [ Leer edad ] -> < ¿Edad es 18 o más? >
  -- sí --> [ Mostrar "pasa" ] -> ( Fin )
  -- no --> [ Mostrar "no pasa" ] -> ( Fin )
```

### Tus 2 diagramas

1. Con decisión: permiso para entrar según edad y si trae identificación.
2. Con repetición: contar del 1 al 5 mostrando cada número, o sumar precios hasta pasar de 1.000.

Recorre cada diagrama con 2 casos distintos (uno que tome el sí y otro el no, o dos vueltas distintas) y anota qué sale en cada caso.

### Investiga

Dibuja los 2 diagramas en `NOTAS.md` (a mano o con texto como el ejemplo) y anota el recorrido de cada caso. Si un caso no tiene flecha de salida, te falta un camino: dibújalo.

### Mide tu avance

Cada diagrama completo vale 1 punto, total 2. Los recorridos anotados de los 4 casos valen 2 puntos. Total 4 puntos.

## 1.4 Pseudocódigo y PSeInt

El pseudocódigo es el algoritmo en español casi de programador. PSeInt solo lo ejecuta para comprobarte. Estas son todas las reglas que necesitas:

```text
Escribir "texto"     // mostrar en pantalla
Leer dato            // pedir un dato
total <- 0           // guardar un valor
Si condicion Entonces
  pasos
SiNo
  pasos
FinSi
Mientras condicion Hacer
  pasos
FinMientras
Para i <- 1 Hasta 5 Hacer
  pasos
FinPara
```

El ejemplo del promedio, ahora en pseudocódigo:

```text
Escribir "Dime las 3 notas"
Leer nota1, nota2, nota3
suma <- nota1 + nota2 + nota3
promedio <- suma / 3
Si promedio >= 60 Entonces
  Escribir "Aprobado con ", promedio
SiNo
  Escribir "Reprobado con ", promedio
FinSi
```

Cómo comprobar en PSeInt: escríbelo, ejecútalo paso a paso y compara con tu prueba de escritorio a mano. Si difieren, primero sospecha del algoritmo, no de la herramienta.

La validación final: dale tu pseudocódigo a otra persona (o léelo en voz alta actuando como la compu) sin explicar nada extra. Si se traba, el hueco está en el algoritmo.

### Investiga

Pasa uno de tus 3 algoritmos a pseudocódigo en `NOTAS.md`, ejecútalo en PSeInt con 2 datos distintos y anota ambas salidas. Luego valida el otro con la lectura en voz alta y anota dónde te trabaste, si pasó.

### Mide tu avance

Pseudocódigo que corre en PSeInt con 2 casos anotados vale 2 puntos. Validación en voz alta o con otra persona, con trabas anotadas, vale 1 punto. Total 3 puntos.

## 1.5 Palabras que verás mucho

- **Algoritmo:** pasos ordenados que resuelven algo. Ejemplo: la receta del café.
- **Entrada:** datos que recibe. Ejemplo: las 3 notas.
- **Salida:** resultado que entrega. Ejemplo: el promedio.
- **Variable:** cajita con nombre para un dato que cambia. Ejemplo: `total`.
- **Condición:** pregunta que se responde sí o no. Ejemplo: ¿edad es 18 o más?
- **Bucle:** repetición hasta que algo se cumpla. Ejemplo: mientras queden platos, lava.
- **Pseudocódigo:** algoritmo en español casi de programador. Ejemplo: la sección 1.4.

> [!TIP]
> Mide tu avance (4 min): tapa las definiciones y define los 7 términos en voz alta con un ejemplo cada uno. De 6 a 7 bien vale 4 puntos, de 4 a 5 vale 2 puntos, menos es 0. Anota tu puntaje en `NOTAS.md`, lo usarás en el repaso final.

## 1.6 Repaso final medible

Hazlo sin mirar el resto del módulo. Suma tus puntos al final. Todo queda anotado en `NOTAS.md`.

### Práctica 1 - Los 3 algoritmos a mano (2 puntos)

Entrega los 3 algoritmos de la sección 1.2 con plantilla ENTRADA/PROCESO/SALIDA (1 punto) más la prueba de escritorio de uno con ejemplo real anotado (1 punto).

### Práctica 2 - Los 2 diagramas recorridos (2 puntos)

Entrega los 2 diagramas de la sección 1.3 (1 punto) más los recorridos de los 4 casos anotados (1 punto).

### Práctica 3 - Pseudocódigo que corre y se entiende (2 puntos)

Pseudocódigo ejecutado en PSeInt con 2 casos anotados (1 punto) más validación en voz alta o con otra persona sin trabas, o con trabas corregidas y anotadas (1 punto).

### Auto-test de vocabulario (4 puntos)

Sin mirar el punto 1.5, define los 7 términos con un ejemplo cada uno. Usa la misma escala de ese punto: de 6 a 7 bien son 4 puntos, de 4 a 5 son 2 puntos, menos es 0.

### Tu puntaje y qué hacer

| Puntaje | Significa | Qué hacer |
| --- | --- | --- |
| 8 a 10 | Listo | Pasa al Módulo 2 |
| 5 a 7 | Casi | Repite mañana solo las prácticas falladas |
| 0 a 4 | Relee | Relee el módulo pasado mañana y repite el repaso |

### Plan de repaso espaciado

- [ ] Día 1: repaso final completo y puntaje anotado en `NOTAS.md`.
- [ ] Día 3: solo recuerdo sin mirar de lo que fallaste.
- [ ] Día 7: repite las 3 prácticas en 30 minutos.

## Siguiente paso

Pasa al Módulo 2 cuando tu puntaje sea de 8 o más, donde estos mismos pasos se escribirán en Python.
