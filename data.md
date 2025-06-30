---
layout: default
title: Data
permalink: /data
---
# Limpieza de Datos

---

Principalmente recopilamos datos del corpus Fair Disclosure (FD) Wire en Nexis. Un cambio regulatorio en agosto de 2000 (“Regulation Fair Disclosure”) introdujo requisitos obligatorios de divulgación pública sobre cómo las empresas difunden información. Fair Disclosure (FD) Wire comenzó en abril de 2001 como un servicio de comunicados de prensa para difundir información de las empresas en respuesta a este cambio regulatorio. Uno de los servicios que ofrece FD Wire es la difusión de transcripciones de llamadas de resultados, a las que las empresas se adhieren voluntariamente. Estamos buscando transcripciones de FD Wire en LexisNexis, utilizando la API de Nexis. Parece que las llamadas de resultados no están disponibles de manera consistente antes de 2005, aunque para algunas empresas hay transcripciones disponibles desde 2001. Como resultado, no solo estamos analizando llamadas de resultados desde 2005 hasta 2024.

<img src="https://juliocedillo.github.io/neweconomy/assets/images/GICS.svg">

Estamos analizando tres sectores del Estándar de Clasificación Industrial Global (GICS®). GICS® es un marco de análisis industrial que ayuda a los inversionistas a comprender las principales actividades comerciales de las empresas en todo el mundo. MSCI y S&P Dow Jones Indices desarrollaron este estándar de clasificación para proporcionar definiciones de industria coherentes y exhaustivas. Los tres sectores incluyen finanzas, energía y materiales. A partir de ahí, filtramos las empresas no relevantes del dataframe según el PERMNO—un identificador único a nivel de acción (clase de acción), las ordenamos por fecha, y verificamos si tenemos las llamadas de resultados del periodo deseado, marcamos los duplicados y recuperamos las llamadas de resultados faltantes ya sea en Nexis Lexis o en Factiva.

# Procesamiento de Lenguaje Natural

---

_En preparación_

# Entrevistas en Profundidad

---

_En preparación_
