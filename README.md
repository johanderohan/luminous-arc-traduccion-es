# Luminous Arc — Traducción al español

[![Invítame a un café en Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/johanderohan)

Traducción al **español de España** de *Luminous Arc* (Nintendo DS, 2007),
el RPG táctico de imageepoch publicado por Marvelous y Atlus USA, que nunca salió
en español.

La traducción se reparte como **parche**: no incluye el juego. Necesitas tu propia
copia para aplicarlo.

## Estado

Última versión: **[v1.1 — Menús e imágenes en español](../../releases/tag/v1.1)**.

Esta versión incorpora **227 rótulos traducidos dentro de imágenes**: menú
principal, opciones, guardar/cargar, equipo, estadísticas, títulos de capítulos
y nombres de lugares, entre otros. Se conservan las paletas del juego y se han
ajustado la alineación y la altura de las letras.

También corrige letras que desaparecían en ayudas y nombres de objetos,
como la **ú** de «Ajusta el volumen de la música». Incluye los caracteres
**á é í ó ú ü ñ Á É Í Ó Ú Ü Ñ ¡ ¿**, recupera tildes omitidas en algunas
intervenciones en mayúsculas y completa ocho descripciones que usaban «&».

La cobertura de referencia del guion sigue siendo la publicada en v1.0.1:
aproximadamente **94 %** (16.862 de 17.859 líneas). Los rótulos gráficos se
cuentan aparte; esta versión no recalcula el porcentaje global del guion.

| Parte | Estado |
|---|---|
| Historia principal y escenas | **99 %** |
| Objetos y habilidades | **98 %** |
| Conversaciones secundarias | 96 % |
| Menús y sistema | 88 % |
| Texto dentro de imágenes | **227 rótulos traducidos**; revisión visual parcial |

### Lo que queda pendiente

Quedan textos sin traducir y la revisión completa durante una partida. La
corrección de «música» se ha comprobado en el emulador; no equivale a una
prueba de todo el juego de principio a fin.

**Las imágenes traducidas sí están incluidas en el parche.** Aún quedan algunos
avisos de combate, botones y textos de pantallas secundarias por traducir, además
de revisar todos los gráficos durante una partida. No se presenta como una
traducción de imágenes completa ni como una revisión visual de todo el juego.

## Cómo aplicar el parche

1. Descarga el parche `.xdelta` de la sección **[Releases](../../releases)**.
2. Consigue tu copia del juego en versión **USA**. El parche solo funciona con
   esa versión exacta.
3. **Comprueba que tu copia es la correcta** antes de nada:

   | | |
   |---|---|
   | Archivo | `Luminous Arc (USA).nds` |
   | Tamaño | 134.217.728 bytes (128 MB) |
   | MD5 | `cc5aa096e73df3a2fffc23a779a6052f` |

   ```bash
   md5sum "Luminous Arc (USA).nds"     # Linux
   md5 "Luminous Arc (USA).nds"        # macOS
   CertUtil -hashfile "Luminous Arc (USA).nds" MD5   # Windows
   ```

   Si no coincide, el parche fallará o dará un resultado corrupto.
4. Aplica el parche con una de estas herramientas:
   - **Windows**: [Delta Patcher](https://github.com/marco-calautti/DeltaPatcher/releases)
   - **Linux / macOS**: `xdelta3 -d -s "juego original.nds" parche.xdelta "juego traducido.nds"`
5. Para **v1.1**, comprueba que la ROM resultante tiene MD5
   **`985588c9cba4bae92b86b94de2482986`**.
6. Carga la ROM resultante en tu emulador o flashcard preferidos.

Aplica cada versión sobre la **ROM USA original**, no sobre una ROM ya
traducida ni sobre el parche anterior.

Cada release indica además el md5 de la ROM ya traducida, por si quieres
confirmar que el parcheado ha ido bien.

## Aviso

Este proyecto es una traducción hecha por afición, sin ánimo de lucro y sin
relación alguna con imageepoch, Marvelous ni Atlus. Aquí no se distribuye el
juego ni ninguna parte de él: solo un parche que modifica una copia que ya
tengas.

Si eres el titular de los derechos y quieres que retire esto, abre una incidencia
y lo hago.
