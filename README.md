# IMT-2200 — Resumen personal (Matías Pérez Unda)

Este repositorio es un **resumen personal y recruiter-friendly** de mi participación en el proyecto grupal de IMT-2200 (Introducción a la Ciencia de Datos): análisis de las pruebas de acceso a la educación superior en Chile (PSU/PTU/PAES) con datos DEMRE 2004–2025. 

✅ **Repositorio oficial del grupo (entrega completa):**  
https://github.com/Proyecto-IMT-2200/2025-2

---

## Qué hice yo (mi aporte)

### 1) Pregunta 3 — Distribución socioeconómica por universidad (GSE)
Analicé cómo se distribuyen los estudiantes que ingresan a educación superior según **grupo socioeconómico (AB/C/D/E)** usando el campo de ingreso familiar disponible en los datos DEMRE entre 2004 y 2025.

**Metodología (resumen):**
- Extracción de tramo numérico **1–12** desde “ingreso familiar”.
- Agrupación a GSE:
  - 1–2 → **E**
  - 3–4 → **D**
  - 5–8 → **C**
  - 9–12 → **AB** 
- Conteo por universidad y conversión a porcentaje (100% por universidad), ordenando por % de AB para comparar mejor.

> Nota: En el repo grupal se especifica que la **Pregunta 3** fue mi responsabilidad.

---

### 2) Modelo predictivo / regresiones (apoyo)
Además participé en el notebook de modelamiento y comparación de regresiones (lineal vs polinomial). En el sitio del proyecto se reporta la comparación y se concluye que el mejor modelo es el **polinomial grado 3**, con métricas (R² test ≈ 0.2735; RMSE ≈ 118.49; MAE ≈ 96.06). 

---

## Estructura de este repo
- `notebooks/`
  - `Pregunta3.ipynb` (mi notebook principal)
  - `Modelo_Predictivo_NEM_ff.ipynb` (apoyo modelamiento)
- `requirements.txt`
- (Opcional) `assets/` para imágenes/gráficos

---

## Datos
Los datos se obtienen desde DEMRE (Portal de Transparencia) o desde el link compartido por el equipo en el repo oficial.
**Este repo no incluye datasets** (solo código/analysis).

---

## Cómo ejecutar (rápido)
```bash
pip install -r requirements.txt
jupyter notebook
