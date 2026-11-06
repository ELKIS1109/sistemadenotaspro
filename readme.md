# Mora Tech School Manager Pro
### Suite Administrativa Escolar y Control Académico MEDUCA

Sistema integral y autónomo de control académico, registro de calificaciones, consolidado de matrícula y generación de informes oficiales diseñado bajo la normativa del Ministerio de Educación de la República de Panamá (MEDUCA).

---

## 📋 Características Principales

- **Gestión Unificada de Estudiantes:** Matrícula oficial con cédula, datos personales, información de contacto de acudientes y estructura académica segmentada.
- **Validación Oficial de Calificaciones (MEDUCA):**
  - Escala oficial estricta de **1.0 a 5.0**.
  - Ponderación reglamentaria: 35% Promedio Diario ($P.ND$), 35% Promedio de Apreciación ($P.NA$) y 30% Examen Trimestral ($Exam$).
  - Control de asistencias: Ausencias ($A$), Tardanzas ($T$) y Fugas ($F$).
- **Filtro Inteligente de Rendimiento y Porcentajes:**
  - Al generar el informe de porcentajes desde las calificaciones, el sistema filtra de forma automática únicamente los grupos pertenecientes al **mismo nivel activo** (por ejemplo, si se evalúa 12°, compila exclusivamente 12° con sus respectivas asignaturas y modalidades).
  - Categorización académica automática:
    - **10° a 12°:** Modalidad Media con desglose de especialidad / bachillerato (*Tecnología, Ciencias, Humanidades, Comercio, Turismo, Marítimo*).
    - **7° a 9°:** Clasificación como **Premedia**.
    - **1° a 6°:** Clasificación como **Primaria**.
- **Motor de Impresión Limpia (1 Sheet Engine):**
  - **Libreta Oficial:** Formato vertical de exactamente 45 filas en una sola hoja lista para firma.
  - **Cuadro de Rendimiento y Rendición de %:** Formato oficial MEDUCA con cálculo automático de porcentajes de aprobados, fracasos y alumnos sin calificación.
  - **Expediente con Código QR Dinámico:** Ficha de verificación rápida con generación de código QR individual por estudiante.
  - **Informe Anual Consolidado:** Reporte trimestral con acumulado anual de calificaciones y asistencia.
- **Arquitectura Local First y Persistencia:**
  - Los datos residen en el navegador (`localStorage`), garantizando disponibilidad 100% offline sin necesidad de servidores o internet.
  - Sistema de **Forzar Respaldo** (`.json`) y **Restaurar Backup** para migrar o resguardar la información de forma segura entre dispositivos.

---

## 🚀 Instalación y Uso

El proyecto está diseñado bajo una arquitectura de **archivo único (Single File Application)**:

1. Clona o descarga el repositorio:
   ```bash
   git clone https://github.com/tu-usuario/tu-repositorio.git
   ```
2. Abre directamente el archivo `index.html` en cualquier navegador web moderno (Google Chrome, Mozilla Firefox, Microsoft Edge, Safari o navegadores móviles).
3. No requiere instalación de dependencias, Node.js ni bases de datos externas.

---

## 💾 Respaldo y Manejo de Datos

- **Subir cambios a GitHub:** Actualizar el código fuente en GitHub no borra los datos de los estudiantes registrados en tu navegador, ya que se almacenan de manera local (`localStorage`).
- **Recomendación de seguridad:** Antes de actualizar o limpiar el navegador, utiliza siempre el botón verde **Forzar Respaldo** de la barra lateral para descargar una copia de seguridad en formato `.json`.

---

## 🛠️ Tecnologías Empleadas

- **HTML5 & CSS3:** Maquetación responsiva y adaptada a hojas de estilo de impresión `@media print`.
- **JavaScript (Vanilla ES6+):** Lógica reactiva de cálculo aritmético, filtrado de datos y manipulación del DOM sin dependencias pesadas.
- **QRCode.js:** Librería ligera para la renderización de códigos QR en expedientes estudiantiles.

---

## 👨‍🏫 Autoría y Créditos

- **Desarrollador y Administrador:** Mgtr. Elkis H. Mora Ch.
- **Institución:** Instituto José Dolores Moscote
- **Contacto:** elkis.mora@meduca.edu.pa
- **Sitio Web:** [www.pcnetpanama.com](https://www.pcnetpanama.com)

---

*Todos los derechos reservados © Mgtr. Elkis H. Mora Ch. - Sistema de Gestión Escolar MEDUCA.*