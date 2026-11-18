# Cómo contribuir

¡Gracias por interesarte en mejorar esta calculadora! Acá explicamos cómo sumar nuevas jurisdicciones o corregir datos.

## ¿Cómo sumar una provincia?

Cada provincia argentina tiene su propio Estatuto Docente. Para agregarla a la calculadora necesitamos una tabla clara con:

- Tipo de licencia (ej: Matrimonio, Maternidad, Enfermedad)
- Situación de revista (Titular, Provisional, Suplente, Todos)
- Artículo del estatuto
- Cantidad de días
- Tipo de día: H (hábil) o C (corrido)
- Goce de haberes: días con goce al 100%, 50% o sin goce
- Observaciones importantes

### Formato esperado

Los datos se cargan en el archivo `index.html` dentro del array `rawLicenciasXXXX` (donde `XXXX` es el código de la provincia).

Cada fila sigue este orden:

```js
["Tipo de licencia", "Situación", "Artículo", "Días", "H/C", "Goce100", "Cod100", "Goce50", "Cod50", "SinGoce", "CodSinGoce", "Observaciones"]
```

Ejemplo:

```js
["Matrimonio", "Todos", "69", "10", "H", "10", "m", "", "", "", "", "10 días hábiles con goce íntegro"]
```

## ¿Dónde conseguir los datos?

- Estatuto Docente oficial de la provincia.
- Resoluciones del ministerio de educación provincial.
- Informes de los sindicatos docentes de cada jurisdicción.

## Pasos para contribuir

1. Hacé un fork del repositorio.
2. Agregá los datos en el array correspondiente.
3. Probá localmente abriendo `index.html`.
4. Enviá un pull request explicando de dónde sacaste los datos.

## Datos que NO vamos a inventar

No agreguemos datos sin una fuente clara. La idea es que la calculadora sea confiable.

## ¿Preguntas?

Abrí un issue en el repositorio y lo vemos.
