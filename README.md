# Curvas de tasa de cheques de pago diferido

Informe de las subastas de cheques de pago diferido del Mercado Argentino de
Valores. Muestra la tasa promedio ponderada por monto y la máxima del día por
tramo de plazo, con ajuste logarítmico de la curva, abierto por avalista en el
segmento garantizado y por empresa en el no garantizado.

**[Ver el informe](https://TU-USUARIO.github.io/cpd-curvas/)**

## Qué hay adentro

- **Curvas por plazo.** Cada punto es un tramo; su posición en el eje x es el
  plazo promedio ponderado del tramo y su área, el monto negociado. La línea es
  el ajuste TNA = a + b·ln(plazo), estimado por mínimos cuadrados ponderados por
  monto sobre las subastas individuales.
- **Comparador de fechas.** La misma entidad en dos días, con el delta por tramo
  en puntos básicos.
- **Evolución.** La tasa de una o varias entidades día a día, contra el promedio
  ponderado del mercado y la banda que va del mínimo al máximo de ese día.

## Criterios

Solo entran las subastas con estado **Negociada**. Los tramos son 0-30, 31-60,
61-90, 91-120, 121-150, 151-180, 181-270, 271-360 y 361 o más días; en el
segmento no garantizado el primero se abre en 0-15 y 16-30, donde se concentra
el volumen. Las curvas nunca mezclan monedas: pesos, dólar billete y dólar
linked se miran por separado. El segmento "Garantizado MAV" agrupa las subastas
garantizadas sin avalista identificado en el listado.

Fuente: listado de subastas del MAV. Los datos van embebidos en el HTML, así que
el informe refleja la última publicación y no se actualiza solo.

## Aviso

Uso informativo. No constituye recomendación de inversión ni oferta de compra o
venta de ningún instrumento. Las cifras pueden contener errores de procesamiento
y no reemplazan a la información oficial del mercado.
