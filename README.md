# Distribución socioeconómica por universidad (GSE) — DEMRE 2004–2025

**Proyecto académico grupal (IMT-2200).**  
Este repositorio es un **resumen de mi aporte** dentro del proyecto del equipo.

## Highlights (resultados clave)
- **Ranking por universidad** según % del grupo **AB** (comparación directa entre instituciones).
- **Distribución porcentual AB/C/D/E** por universidad, construida desde el campo *ingreso familiar* (tramos 1–12).
- **Entregable principal:** gráfico de barras horizontales apiladas + tabla porcentual por institución.

> (Opcional: agrega 1–2 hallazgos concretos)
> - Hallazgo: **[EJ: “Las universidades X, Y, Z concentran mayor %AB”]**
> - Hallazgo: **[EJ: “Se observa mayor presencia de C/D en…”]**

## Imagen (output)
> Export del gráfico principal (generado desde el notebook):

![Distribución AB–E por universidad](pregunta3.png)

*(Si cambias la carpeta, ajusta la ruta. Recomendado: `assets/` o `graficos-imagenes/`.)*

## Qué hice yo (mi aporte)
### 1) Pregunta 3 — Distribución socioeconómica por universidad (GSE)
Analicé cómo se distribuyen los estudiantes que ingresan a educación superior según grupo socioeconómico **AB / C / D / E** usando el campo **ingreso familiar** disponible en datos DEMRE entre **2004 y 2025**.

**Metodología (resumen):**
- Extracción del tramo numérico **1–12** desde “ingreso familiar”.
- Agrupación a GSE:
  - **1–2 → E**
  - **3–4 → D**
  - **5–8 → C**
  - **9–12 → AB**
- Conteo por universidad y conversión a **porcentaje** (100% por universidad).
- Ordenado por **%AB** para comparar instituciones.

> Nota: En el repositorio grupal se indica que **Pregunta 3** fue mi responsabilidad.

### 2) Modelo predictivo / regresiones (apoyo)
Participé en el notebook de modelamiento y comparación de regresiones (**lineal vs polinomial**).  
En el sitio del proyecto se reporta la comparación y se concluye que el mejor modelo es el **polinomial grado 3**, con métricas aproximadas (**R² test ≈ 0.2735; RMSE ≈ 118.49; MAE ≈ 96.06**).

## Estructura del repo
- `notebooks/`
  - `Pregunta3.ipynb` (mi notebook principal)
  - `Modelo_Predictivo_NEM_ff.ipynb` (apoyo modelamiento)
- `requirements.txt`
- `graficos-imagenes/` (exports de gráficos)
  - `pregunta3.png`

## Datos
Los datos se obtienen desde **DEMRE (Portal de Transparencia)** o desde el link compartido por el equipo en el repo oficial.  
Este repo **no incluye datasets** (solo código/análisis).

## Cómo ejecutar (rápido)
```bash
pip install -r requirements.txt
jupyter notebook
