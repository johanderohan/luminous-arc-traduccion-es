# Luminous Arc — Traducción al español

[![Invítame a un café en Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/johanderohan)

Traducción al **español de España** de *Luminous Arc* (Nintendo DS, 2007),
el RPG táctico de imageepoch publicado por Marvelous y Atlus USA, que nunca salió
en español.

La traducción se reparte como **parche**: no incluye el juego. Necesitas tu propia
copia para aplicarlo.

## Estado

Última versión: **[v1.2 — Revisión de textos, menús y combate](../../releases/tag/v1.2)**.

Incluye **637 rótulos traducidos dentro de imágenes**, 410 más que v1.1.
Se han completado los menús de ciudades («Acción», «Volver al mapamundi»,
«Avanzar la historia» y «Hablar con…»), los botones del prólogo y los avisos,
recompensas y etiquetas de combate. También se ha revisado la alineación
del menú principal y de los objetivos.

Esta versión corrige **1.267 registros de texto** con duplicados sin traducir,
tramos en inglés y descripciones pendientes. Traduce **1.227 etiquetas de
hablante** que son cargos o descripciones, como «Monk» → «Monje», conservando
los nombres propios.

| Parte | Estado |
|---|---|
| Guion y menús | 1.267 registros completados o corregidos respecto a v1.1 |
| Nombres de hablantes | 1.227 etiquetas genéricas traducidas |
| Texto dentro de imágenes | **637 rótulos traducidos**, incluidos en el parche |
| Caracteres españoles | **á é í ó ú ü ñ Á É Í Ó Ú Ü Ñ ¡ ¿** |
| Revisión durante una partida | Parcial |

Se mantienen las correcciones de tildes y letras que desaparecían en ayudas
y objetos, incluida la **ú** de «música».

El porcentaje global del guion no se ha recalculado para esta versión.
Como referencia histórica, v1.0.1 publicó aproximadamente **94 %**
(16.862 de 17.859 líneas); esa cifra no representa el avance actual.

### Comprobaciones y trabajo pendiente

Se han comprobado en emulador el menú principal, los menús de ciudades,
el nombre «Monje» en una conversación, el despliegue y el objetivo del primer
combate. También se han revisado las imágenes recompuestas y sus colores.
El parche se ha aplicado sobre la ROM USA original y el resultado se ha
comparado byte a byte con la ROM preparada.

**Las imágenes traducidas sí están incluidas en el parche.** Queda la revisión
completa durante una partida y la comprobación de las pantallas secundarias.
No se presenta como una traducción de todos los gráficos ni como una prueba
del juego de principio a fin.

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
5. Para **v1.2**, comprueba que la ROM resultante tiene MD5
   **`a09df2543a8768e2f2ce1fd72f75b6ea`**.
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
