# Luminous Arc — Traducción al español

[![Invítame a un café en Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/johanderohan)

Traducción completa al **español de España** de *Luminous Arc* (Nintendo DS, 2007),
el RPG táctico de imageepoch publicado por Marvelous y Atlus USA, que nunca salió
en español.

La traducción se reparte como **parche**: no incluye el juego. Necesitas tu propia
copia para aplicarlo.

## Estado

Traducido el **87 %** del texto (15.487 de 17.859 líneas).

| Parte | Progreso |
|---|---|
| Historia principal y escenas | **99 %** |
| Conversaciones secundarias | 96 % |
| Menús y sistema | 88 % |
| Nombres y descripciones de objetos y habilidades | 18 % |
| Texto dentro de imágenes | 0 % |

**La historia está terminada**: se puede jugar de principio a fin en español.

### Lo que sigue en inglés

**Objetos y habilidades.** Sus nombres y descripciones están casi sin tocar. Es
donde el espacio aprieta más, porque hay que caber en el hueco del original.

**El texto dentro de las imágenes.** Parte del texto del juego no está guardado
como texto, sino **dibujado dentro de los gráficos**: el menú principal
(`New Game`, `Options`, `Extras`), los rótulos del menú de sistema y de equipo, y
las pantallas de guardar y cargar. Traducirlos no es escribir, es redibujar cada
rótulo píxel a píxel respetando su marco, así que van para más adelante.

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
5. Carga la ROM resultante en tu emulador o flashcard preferidos.

Cada release indica además el md5 de la ROM ya traducida, por si quieres
confirmar que el parcheado ha ido bien.

## Aviso

Este proyecto es una traducción hecha por afición, sin ánimo de lucro y sin
relación alguna con imageepoch, Marvelous ni Atlus. Aquí no se distribuye el
juego ni ninguna parte de él: solo un parche que modifica una copia que ya
tengas.

Si eres el titular de los derechos y quieres que retire esto, abre una incidencia
y lo hago.
