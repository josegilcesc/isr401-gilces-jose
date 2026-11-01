# TA-IND-01: Trabajo Autónomo - Tipos de Requisitos y Estándar IEEE 29148

**Asignatura:** Ingeniería de Requerimientos (ISR401)  
**Institución:** Universidad Técnica Estatal de Quevedo (UTEQ)  
**Carrera:** Ingeniería de Software  
**Caso de Estudio:** Sistema en línea de cobro de impuestos prediales para un GAD Cantonal (integrado con el SRI y pasarela de pagos local)  
**Código de Actividad:** TA-IND-01  

---

## Autores / Integrantes

- **José Ignacio Gilces Carranza**
- **Danela Dayana Arteaga Álava**
- **Winston Damián Cedeño Ávila**
- **Allan Jeremy Mendoza Palma**

---

## Descripción del Proyecto

Este repositorio contiene los archivos fuente en LaTeX y el documento PDF final compilado para la **Actividad Autónoma TA-IND-01**, correspondiente a la Unidad 1 de la asignatura. El informe desarrolla la identificación de stakeholders, la redacción de requisitos funcionales (RF) y no funcionales (RNF) cuantificables bajo la norma **ISO/IEC/IEEE 29148:2018**, la clasificación de RNF en las 9 características de **ISO/IEC 25010:2023**, y el modelado de restricciones y dependencias.

---

## Estructura del Repositorio

```text
.
├── .gitignore                # Exclusion de archivos temporales de compilacion
├── README.md                 # Documentacion e instrucciones del repositorio
├── main.tex                  # Archivo principal fuente en LaTeX
├── referencias.bib           # Bibliografia en formato BibTeX (estilo IEEE / biblatex)
├── main.pdf                  # PDF compilado final (maximo 6 paginas)
├── secciones/                # Modulos del informe (.tex)
│   ├── 01_stakeholders.tex
│   ├── 02_requisitos_funcionales.tex
│   ├── 03_requisitos_calidad_iso25010.tex
│   └── 04_restricciones_dependencias.tex
└── figuras/                  # Diagramas y esquemas de apoyo
```

---

## Instrucciones de Compilación (Reproducibilidad)

En cumplimiento del Criterio de Piso P2 del encuadre académico, se detallan las instrucciones para regenerar el documento PDF a partir de los archivos fuente en LaTeX.

### Requisitos del Entorno

- **Distribución LaTeX:** MiKTeX, TeX Live o MacTeX.
- **Compilador principal:** pdflatex.
- **Procesador bibliográfico:** biber (configurado con biblatex en formato IEEE).

### Secuencia Exacta de Comandos

Ejecute la siguiente secuencia en la consola desde la raíz del repositorio:

```bash
pdflatex -synctex=1 -interaction=nonstopmode main.tex
biber main
pdflatex -synctex=1 -interaction=nonstopmode main.tex
pdflatex -synctex=1 -interaction=nonstopmode main.tex
```

> **Configuración en TeXstudio:** Seleccionar Biber en *Opciones -> Configurar TeXstudio -> Compilación -> Herramienta de bibliografía por defecto*.

---

## Declaración de Uso de Inteligencia Artificial

De conformidad con las normas de integridad académica de la asignatura:

- **Herramientas de IA empleadas:** Gemini / ChatGPT.
- **Propósito del uso:** Asistencia en el maquetado en LaTeX, revisión de ortografía y soporte en la estructuración sintáctica.
- **Método de verificación humana:** Los integrantes del equipo verificaron, redactaron y validaron la totalidad de los requisitos, la cuantificación de las métricas de calidad y la autenticidad de las referencias bibliográficas oficiales (ISO/IEC/IEEE 29148:2018 e ISO/IEC 25010:2023).
