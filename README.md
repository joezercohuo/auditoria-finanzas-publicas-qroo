# 📊 Auditoría de Finanzas Públicas: Análisis de Contrataciones SEOP Quintana Roo

## 📌 Resumen del Proyecto
Análisis integral de los procedimientos de contratación pública (Licitación vs. Adjudicación Directa) de la Secretaría de Obras Públicas, utilizando datos abiertos de la Plataforma Nacional de Transparencia (PNT). El objetivo principal es evaluar la eficiencia del gasto gubernamental, detectar patrones de concentración de capital y validar estadísticamente las vías de asignación presupuestal.

## 🛠️ Stack Tecnológico
* **Extracción y Limpieza:** Python (Pandas) - Transformación de bases gubernamentales (UTF-8-SIG, depuración de 95 a 4 variables clave, estandarización de tipos de datos).
* **Estadística Inferencial:** Python (SciPy) - Pruebas de hipótesis (T-test de Welch) para análisis de varianza y medias poblacionales.
* **Visualización de Negocio:** Power BI - Creación de dashboard interactivo para tomadores de decisiones.

## 📈 Hallazgos Clave (Business Insights)
1. **Foco de Excepción como Regla:** El 52.26% del presupuesto total auditado fue asignado mediante Adjudicación Directa, evadiendo el esquema de competencia legal (Licitación Pública).
2. **Validación Estadística (T-Test):** Se aplicó una prueba de hipótesis (p-value: 0.422) que demostró matemáticamente la ausencia de diferencias significativas entre los montos licitados y los adjudicados, indicando un uso discrecional de cheques millonarios sin justificación de tope financiero.
3. **Concentración y Fraccionamiento:** Identificación de anomalías en la frecuencia de contratos, destacando empresas con hasta 12 adjudicaciones directas en el mismo periodo (posible fraccionamiento) frente a proveedores que concentran el mayor volumen de gasto en una sola asignación.

## 📁 Estructura del Repositorio
* `1_Limpieza_Datos.ipynb`: Script documentado con el proceso de extracción, limpieza y corrección de formato del padrón oficial.
* `2_Pruebas_Estadisticas.ipynb`: Código con el test de medias (T-test) y métricas de dispersión.
* `dashboard_auditoria.pbix`: Archivo fuente del panel de control (Dashboard).
* `contratos_limpios_qroo.csv`: Dataset optimizado listo para modelado.
