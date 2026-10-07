# Magical Vacation — Traducción al castellano

[![Invítame a un café en Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/johanderohan)

Ficha del proyecto, capturas y más traducciones al castellano en **[Parches en Castellano](https://parchesencastellano.com/traducciones/game-boy-advance/magical-vacation)**.

Traducción del japonés al **español de España** de *Magical Vacation* para Game Boy Advance.

La traducción se distribuye como **parche IPS**. Necesitas tu propia copia del juego japonés para aplicarlo.

## Descargas

Versión actual: **[0.9 RC2 — Correcciones del selector y del teclado](https://github.com/johanderohan/magical-vacation-traduccion-es/releases/tag/v0.9-RC2)**.

- **[Descargar parche IPS](https://github.com/johanderohan/magical-vacation-traduccion-es/releases/download/v0.9-RC2/Magical.Vacation.ES.0.9-RC2.ips)**.
- [Todas las versiones](https://github.com/johanderohan/magical-vacation-traduccion-es/releases).

## Estado

| Parte | Alcance |
|---|---|
| Catálogo lingüístico | 7.777 entradas traducidas e insertadas: guion, nombres, menús y otros textos |
| Teclado | 46 filas adaptadas; tildes y ñ; seis casillas de nombre |
| Gráficos | Botones, cabeceras e indicadores adaptados; 20 rótulos de créditos traducidos |
| Prueba durante una partida | Parcial; pendiente el recorrido completo y la prueba en Steam Deck |

Los recuentos incluyen repeticiones y alias; no equivalen al porcentaje de una partida. El segundo cotejo se ha realizado con agentes de IA y no constituye una certificación de revisión humana. Se conservan las autorías y los avisos originales, así como la paleta japonesa opcional «Kan.».

### Correcciones de RC2

- **Antigüedad muestra la descripción de Clock**, que reduce la velocidad enemiga. Un error de tabla hacía aparecer la descripción de Fuego en su lugar.
- Ajustadas las **trece descripciones elementales** al límite interno para que se muestren completas, con sus afinidades y dificultad.
- Corregidos los **restos de caracteres japoneses en los botones del teclado**, incluido «Fin».
- Restaurada la última fila de la paleta de kanji y corregido el espacio que ocupan los iconos elementales.

### Pruebas y trabajo pendiente

Comprobados en mGBA para macOS el arranque, las trece opciones del selector, el recorrido inicial de la escuela, una conversación completa, menús, nombre con ñ, variante femenina y guardado/carga en una instancia nueva del núcleo. Se han revisado 22 fichas del bestiario mediante instrumentación de RAM, sin atribuir ese acceso a progreso normal de la partida. El parche aplicado al original produce exactamente la ROM verificada.

**Es una candidata de prueba.** Falta una partida completa, los combates y finales en su contexto, ramas opcionales, funciones de enlace y la comprobación en una Steam Deck real. No se ha reproducido el posible bloqueo escolar comunicado en un emulador online; la web y su configuración no pudieron identificarse.

## Cómo aplicar el parche

1. Descarga el **parche IPS** de Releases.
2. Usa tu copia **japonesa original** con estos datos:

   | Dato | Valor |
   |---|---|
   | Archivo de referencia | `Magical Vacation (Japan).gba` |
   | Tamaño | 8.388.608 bytes (8 MiB) |
   | Código | `AMVJ` |
   | SHA-256 | `a3209cc16050f458b5decf8008c9c76b95bd5078e5964446b84b9a4b6dfc17ee` |

3. Abre [Rom Patcher JS](https://www.marcrobledo.com/RomPatcher.js/), selecciona la ROM original y el archivo `.ips`, y aplica el parche. También puedes utilizar otra herramienta compatible con IPS.
4. Carga la ROM resultante en tu emulador de GBA. Si utilizas RetroArch, las pruebas locales se realizaron con el núcleo mGBA.

Aplica cada versión sobre el **original japonés**, no sobre una ROM ya traducida. La ROM resultante ocupa 16 MiB y su SHA-256 debe ser:

```text
aa8c604dd17fa7d82365832ffecb8381e84699269a002425a2dbc08af11c3ace
```

Usa el guardado interno del juego y conserva una copia de tu partida. No mezcles estados instantáneos de distintas versiones de la ROM; la compatibilidad de partidas anteriores no está certificada.

## Créditos

Traducción basada en el japonés de la ROM. Referencia técnica de formatos y tablas: [kcaze/magical_vacation_translation](https://github.com/kcaze/magical_vacation_translation), revisión `b4963ea743bcfcd8a6b0649962da9209c1abaabb`. No se aplica su parche inglés ni se utiliza su guion como texto de partida.

Proyecto de traducción no oficial. En este repositorio se publican el README y la descarga del parche; no se distribuye la ROM del juego.
