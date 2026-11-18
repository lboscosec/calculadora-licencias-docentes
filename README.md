# Calculadora de Licencias Docentes

Calculadora orientativa de licencias y antigüedad docente para docentes argentinos.

Actualmente incluye:
- **PBA** (Provincia de Buenos Aires): Estatuto Docente Capítulo XX + Decreto 140/2022.
- **CABA** (Ciudad Autónoma de Buenos Aires): Estatuto del Docente de CABA.

El objetivo es sumar progresivamente otras provincias. Si querés aportar los datos de tu jurisdicción, mirá [`CONTRIBUTING.md`](CONTRIBUTING.md).

Funciona 100% en el navegador, sin necesidad de servidor ni base de datos. Los datos se guardan en `localStorage` del dispositivo del usuario.

## Funciones

- **Cálculo de licencias**: fecha de inicio, último día de licencia y fecha de retorno al trabajo.
- **Jurisdicciones**: PBA (Estatuto Docente Capítulo XX + Decreto 140/2022) y CABA (Estatuto del Docente de CABA).
- **Licencias especiales**: matrimonio, maternidad, paternidad/no gestante, adopción, fallecimiento, enfermedad, vacaciones, entre otras.
- **Cadena de licencias**: sumá licencias consecutivas (maternidad + cuidado del recién nacido + excedencia + vacaciones) y obtené la fecha final de retorno.
- **Licencias fraccionables**: excedencia, causas particulares y otras licencias corridas se pueden partir ingresando la cantidad de días deseada.
- **Feriados**: fijos de Argentina, variables automáticos (Carnaval, Semana Santa) y feriados adicionales personalizados.
- **Vacaciones y recesos**: verano e invierno configurables.
- **Antigüedad**: cálculo con cargos superpuestos, períodos que no suman y descuentos.
- **Historial**: guarda los últimos cálculos en el navegador.
- **Exportar / importar**: backup completo en JSON y exportación a CSV.
- **Imprimir / PDF**: versión limpia del resultado para presentar.

## Cómo usar localmente

1. Descargá o cloná este repositorio.
2. Abrí el archivo `calculadora-licencias-docentes.html` en tu navegador.
3. Opcional: si querés levantar un servidor local, ejecutá:

```bash
python -m http.server 8765
```

Y abrí `http://localhost:8765/calculadora-licencias-docentes.html`.

## Publicar online con GitHub Pages

1. Creá un repositorio en GitHub.
2. Subí el archivo `calculadora-licencias-docentes.html`.
3. Renombralo a `index.html` (o dejalo como está y accedé directamente al nombre del archivo).
4. Andá a **Settings → Pages → Source** y seleccioná **Deploy from a branch → main / root**.
5. En minutos tendrás un link tipo:

```
https://tusuario.github.io/calculadora-licencias-docentes
```

## Publicar online con Vercel (recomendado si ya tenés cuenta)

1. Creá un repositorio en GitHub y subí estos archivos.
2. Entrá a [vercel.com](https://vercel.com), iniciá sesión con GitHub.
3. Hacé clic en **Add New Project** e importá el repositorio.
4. Dejá la configuración por defecto (Vercel detecta automáticamente un sitio estático).
5. Hacé clic en **Deploy**. En minutos tendrás un link tipo:

```
https://calculadora-licencias-docentes.vercel.app
```

Cada vez que hagas un `git push` se actualizará automáticamente.

## Publicar online con GitHub Pages

1. Creá un repositorio en GitHub.
2. Subí el archivo `index.html` (y el resto de los archivos) a la raíz.
3. Andá a **Settings → Pages → Source** y seleccioná **Deploy from a branch → main / root**.
4. En minutos tendrás un link tipo:

```
https://tusuario.github.io/calculadora-licencias-docentes
```

## Publicar online con Netlify Drop

1. Entrá a [Netlify Drop](https://app.netlify.com/drop).
2. Arrastrá la carpeta que contiene el archivo HTML.
3. Netlify te dará un link público al instante.

## Aviso legal

Esta calculadora es una herramienta orientativa. Los cálculos se basan en la normativa vigente al momento de su desarrollo. Para casos particulares, interpretaciones o trámites formales, consultá con SADOP, UDAI, tu sindicato o la institución educativa de referencia.

## Licencia

Uso libre. Podés modificarla y compartirla.
