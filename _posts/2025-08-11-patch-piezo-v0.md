---
layout: single
title: "Patch piezoeléctrico v0 para neuromodulación con LIFU"
date: 2025-08-11
categories: [proyectos]
tags: [neuromodulacion, ultrasonidos, piezoelectrico, EEG, MATLAB, Arduino]
excerpt: "Prototipo PVDF-TrFE + MEA con LIFU; adquisición y seguridad térmica."
header:
  overlay_color: "#000"
  overlay_filter: "0.3"
  overlay_image: /assets/images/project_piezo_header.jpg
---

## Problema
Explorar neuromodulación no invasiva mediada por materiales piezoeléctricos con control de seguridad térmica.

## Solución
Desarrollé un **patch piezoeléctrico** (PVDF-TrFE) sobre sustrato flexible y lo integré con una **MEA** comercial. Genero US de 700 kHz con control de duty y monitoreo de temperatura.

## Tecnología
- **Hardware**: PVDF-TrFE, driver clase D, Arduino/Teensy, sensor de temperatura
- **Software**: MATLAB (adquisición/filtrado), Julia (optimización de parámetros), C++ (firmware)
- **Simulación**: k-Wave (US), COMSOL (acoplamiento mecanoeléctrico)

## Proceso (resumen)
1. Deposición y polarización de PVDF-TrFE; caracterización d33.
2. Set-up LIFU con medición de campo y control de duty.
3. Integración con MEA, registro y filtros.
4. Seguridad: límite de ΔT ≤ 0.5 °C.

## Resultados
Se observan cambios reproducibles en la potencia espectral en bandas teta–beta bajo protocolos sub-térmicos. Datos y scripts en el repo.

## Siguientes pasos
- Closed-loop con biomarcador EEG.
- Ensayo de estabilidad y repetibilidad.
- Publicación de dataset abierto.
