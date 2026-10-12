# Situaciones de aprendizaje de Echidna Educación

Situaciones de aprendizaje (SdA) para el alumnado, hechas con [eXeLearning](https://exelearning.net/) para la placa EchidnaBlack2 y EchidnaML. Se publican con GitHub Pages en **<https://rea.echidna.es/>** y se enlazan desde [Materiales alumnado](https://echidna.es/alumnado/).

## Índice

- [Situaciones de aprendizaje](#situaciones-de-aprendizaje)
- [Cómo añadir o actualizar una](#cómo-añadir-o-actualizar-una)
- [Dominio y direcciones antiguas](#dominio-y-direcciones-antiguas)
- [Pendiente](#pendiente)

## Situaciones de aprendizaje

| SdA | Nivel | Autoría | Licencia | Dirección |
|---|---|---|---|---|
| ¿Hace calor aquí? | 3.er ciclo de Primaria | Jorge Lobo Martínez | CC BY-SA 4.0 | [hace-calor-aqui/](https://rea.echidna.es/hace-calor-aqui/) |
| Andalucía, del alba al anochecer | 5.º de Primaria | Jorge Lobo Martínez, con José Pujol Pérez | CC BY-SA 4.0 | [del-alba-al-anochecer/](https://rea.echidna.es/del-alba-al-anochecer/) |
| ¡La Tierra se mueve! | 4.º de Primaria | Jorge Lobo Martínez | CC BY-SA (ver [Pendiente](#pendiente)) | [la-tierra-se-mueve/](https://rea.echidna.es/la-tierra-se-mueve/) |

Cada carpeta contiene la exportación web de eXeLearning y su fichero fuente `.elp`, que se puede abrir con eXeLearning para modificarla.

## Cómo añadir o actualizar una

1. Exporta la SdA desde eXeLearning como «Sitio web» y copia el contenido en una carpeta con un nombre corto en minúsculas y con guiones (`mi-situacion/`).
2. Copia también el `.elp` en la misma carpeta.
3. Haz *push* a `main`: GitHub Pages la publica en `https://rea.echidna.es/<carpeta>/`.
4. Añade su tarjeta en `web/src/content/recursos.yaml` del repo de la web, [EchidnaEducacion.github.io](https://github.com/EchidnaEducacion/EchidnaEducacion.github.io).

El fichero `.nojekyll` es necesario: eXeLearning usa ficheros que empiezan por `_`, que GitHub Pages ignoraría sin él.

## Dominio y direcciones antiguas

El repo se publica con el dominio `rea.echidna.es` (fichero `CNAME`; en el DNS de OVH, `rea.echidna.es` es un `CNAME` a `echidnaeducacion.github.io`). Las direcciones de antes, `echidnaeducacion.github.io/situaciones-aprendizaje/…`, las redirige GitHub a ese dominio.

Antes, `rea.echidna.es` era un servidor propio con otros nombres de carpeta. Para que sus enlaces sigan funcionando:

| Dirección antigua | Lleva a |
|---|---|
| `rea.echidna.es/` | [Materiales alumnado](https://echidna.es/alumnado/) (`index.html`) |
| `rea.echidna.es/02_SensorTemperatura/` | `hace-calor-aqui/` |
| `rea.echidna.es/P4LaTierraSeMueve/` | `la-tierra-se-mueve/` |
| `rea.echidna.es/nocheydia/` | `del-alba-al-anochecer/` |

- Cada carpeta antigua tiene un `index.html` que redirige a la nueva (funciona sin JavaScript).
- Las páginas interiores (`/02_SensorTemperatura/3_el_reto.html`) las resuelve `404.html`: cambia la carpeta y conserva la página, la consulta y el ancla, porque las exportaciones de eXeLearning mantienen los nombres de página. Cualquier otra dirección que no exista lleva a Materiales alumnado.
- **No uses esos nombres de carpeta** para una situación nueva. Si cambia el nombre de una carpeta, añade la antigua en `404.html` y su carpeta de redirección.

## Pendiente

- **Licencia de ¡La Tierra se mueve!**: el texto de créditos dice CC BY-SA, pero el pie de las páginas enlaza a CC BY-NC-SA 4.0. Hay que aclararlo con el autor y corregirlo en el `.elp`.
- **¿Hace calor aquí?**: en «Créditos», la descarga «Ficha XY-Grid» apunta a `Alhambra2.sb3`, que no existe (tampoco en el original).
