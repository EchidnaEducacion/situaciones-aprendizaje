# Situaciones de aprendizaje de Echidna Educación

Situaciones de aprendizaje (SdA) para el alumnado, hechas con [eXeLearning](https://exelearning.net/) para la placa EchidnaBlack2 y EchidnaML. Se publican con GitHub Pages y se enlazan desde [Materiales alumnado](https://echidna.es/alumnado/).

## Índice

- [Situaciones de aprendizaje](#situaciones-de-aprendizaje)
- [Cómo añadir o actualizar una](#cómo-añadir-o-actualizar-una)
- [Pendiente](#pendiente)

## Situaciones de aprendizaje

| SdA | Nivel | Autoría | Licencia | Dirección |
|---|---|---|---|---|
| ¿Hace calor aquí? | 3.er ciclo de Primaria | Jorge Lobo Martínez | CC BY-SA 4.0 | [hace-calor-aqui/](https://echidnaeducacion.github.io/situaciones-aprendizaje/hace-calor-aqui/) |
| Andalucía, del alba al anochecer | 5.º de Primaria | Jorge Lobo Martínez, con José Pujol Pérez | CC BY-SA 4.0 | [del-alba-al-anochecer/](https://echidnaeducacion.github.io/situaciones-aprendizaje/del-alba-al-anochecer/) |
| ¡La Tierra se mueve! | 4.º de Primaria | Jorge Lobo Martínez | CC BY-SA (ver [Pendiente](#pendiente)) | [la-tierra-se-mueve/](https://echidnaeducacion.github.io/situaciones-aprendizaje/la-tierra-se-mueve/) |

Cada carpeta contiene la exportación web de eXeLearning y su fichero fuente `.elp`, que se puede abrir con eXeLearning para modificarla.

## Cómo añadir o actualizar una

1. Exporta la SdA desde eXeLearning como «Sitio web» y copia el contenido en una carpeta con un nombre corto en minúsculas y con guiones (`mi-situacion/`).
2. Copia también el `.elp` en la misma carpeta.
3. Haz *push* a `main`: GitHub Pages la publica en `https://echidnaeducacion.github.io/situaciones-aprendizaje/<carpeta>/`.
4. Añade su tarjeta en `web/src/content/recursos.yaml` del repo de la web, [EchidnaEducacion.github.io](https://github.com/EchidnaEducacion/EchidnaEducacion.github.io).

El fichero `.nojekyll` es necesario: eXeLearning usa ficheros que empiezan por `_`, que GitHub Pages ignoraría sin él.

## Pendiente

- **Licencia de ¡La Tierra se mueve!**: el texto de créditos dice CC BY-SA, pero el pie de las páginas enlaza a CC BY-NC-SA 4.0. Hay que aclararlo con el autor y corregirlo en el `.elp`.
- **¿Hace calor aquí?**: en «Créditos», la descarga «Ficha XY-Grid» apunta a `Alhambra2.sb3`, que no existe (tampoco en el original).
