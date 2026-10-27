# NEXT

Actualizado: 2026-10-27
Issue activo: #3

## Siguiente paso
- Issue #3: preparar, antes de la reunión del 2026-10-28, el resumen de 1 página (dataset
  eritrocitos + malaria *P. Vivax*, 3 opciones de problema, preguntas abiertas). Ya se agregó ahí
  la pregunta sobre la convención de nombres del dataset de eritrocitos (ver Bloqueos).
- Issue #4: redactar título + objetivo general + 2-3 específicos. Última instancia de decisión:
  reunión del profesor el 2026-10-28. Entregable #1 vence el 2026-10-29.

## Estado
Issues #1 y #2 cerrados el 2026-10-27 (ver comentarios de cierre en GitHub para el detalle
completo):
- **#1** (eritrocitos, DHM↔fase) — `notebooks/01-eda-eritrocitos.ipynb`: descarga cacheada en
  Drive, ~9k pares emparejados del split `Training` (de 36.864 por carpeta, por nombres no 1:1),
  overlay+SSIM, distribución de valores de píxel y canales, outliers por z-score. Cerrado sin la
  sección "Observaciones y decisiones" del DoD (decisión explícita de cerrar igual).
- **#2** (malaria *P. Vivax*) — `notebooks/02-eda-malaria.ipynb`: descarga vía `kagglehub` +
  `getpass` (mismo directorio base `/content/data` que el notebook de eritrocitos), estructura
  (1328 imágenes RGB + 2 `.json` de anotaciones), agregación de anotaciones (86.035 total, 2.9%
  enfermas: trophozoite/ring/schizont/gametocyte), descripción de imágenes y recorte en parches
  256x256. Cerrado sin la captura lado a lado explícita del DoD (decisión explícita de cerrar
  igual).

Comparación de modalidad (insumo para #3): el malaria es campo brillante teñido, fondo saturado
en 255, media de píxel ≈185; los hologramas/fase son interferometría sin saturación, medias
≈78/137 — modalidades de captura muy distintas.

## Bloqueos y dudas
- Problema concreto bloqueado hasta la reunión del profesor el 2026-10-28.
- Fuente exacta del dataset de malaria: resuelta — `orvile/p-vivax-malaria-infected-human-blood-smears`
  en Kaggle (issue #2).
- Roles del equipo (Juan, Sahian, yo) sin definir (issue #5).
- Setup del entorno en el notebook de Colab sin definir (issue #6).
