# Distribución socioeconómica por universidad (DEMRE 2004–2025)

**Proyecto académico grupal – IMT 2200**  
Este repositorio documenta mi aporte individual a la **Pregunta 3** del proyecto.

---

## Descripción
Análisis de la distribución de estudiantes que ingresan a la educación superior según su **grupo socioeconómico (GSE)**, utilizando información de **ingreso familiar** proveniente de bases de datos del **DEMRE**, para el período **2004–2025**.

El objetivo es identificar patrones estructurales de acceso a la educación superior y comparar la composición socioeconómica entre universidades.

---

## Principales resultados
- Distribución porcentual por universidad para los grupos **AB, C, D y E**  
- Promedio del período **2004–2025**, lo que permite observar una composición socioeconómica estable por institución  
- Ordenamiento de universidades según el porcentaje del grupo **AB**, facilitando la comparación entre instituciones  

---

## Visualización principal
<p align="center">
  <img src="pregunta3.png" alt="Distribución socioeconómica por universidad" width="900">
</p>

---

## Metodología
1. A partir del campo de **ingreso familiar**, se extrajo un tramo numérico entre **1 y 12**  
2. Los tramos se agruparon en cuatro grupos socioeconómicos:  
   - **1–2 → E**  
   - **3–4 → D**  
   - **5–8 → C**  
   - **9–12 → AB**  
3. Para cada universidad, se contabilizaron los estudiantes por grupo socioeconómico  
4. Los conteos se transformaron en **porcentajes**, de modo que cada universidad suma 100 %  
5. Los resultados se promediaron para el período **2004–2025**  
6. Las universidades se ordenaron según el porcentaje del grupo **AB**, de mayor a menor  

---

## Interpretación y conclusiones
Los resultados evidencian una **fuerte desigualdad socioeconómica** en el acceso a la educación superior.  

Las universidades más selectivas y privadas concentran una mayor proporción de estudiantes pertenecientes a los grupos **AB y C**, mientras que en muchas otras instituciones predomina la matrícula de estudiantes de los grupos **D y E**.  

Este patrón se mantiene de forma consistente durante todo el período analizado (**2004–2025**), lo que sugiere que el acceso universitario en Chile continúa estando **fuertemente asociado al nivel de ingreso familiar**.

---

## Estructura del repositorio
notebooks/Pregunta3.ipynb
requirements.txt
graficos-imagenes/pregunta3.png


---

## Fuente de datos
Los datos utilizados provienen del **DEMRE**, obtenidos a través del **Portal de Transparencia** y del enlace compartido por el equipo en el repositorio grupal.  

Este repositorio **no incluye datasets**, únicamente código y análisis reproducible.

---

## Ejecución
```bash
pip install -r requirements.txt
jupyter notebook
