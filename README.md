# Control de Velocidad Crucero de Automóvil 🚗⚙️

Este proyecto consiste en el diseño, modelado y simulación de un sistema de **control de velocidad crucero para un automóvil** utilizando técnicas de control automático. Fue desarrollado como trabajo integrador de la materia **Sistemas de Control 1** (2022).

## 🧩 Objetivo

Implementar un controlador que mantenga constante la velocidad del vehículo ante diferentes condiciones, permitiendo una conducción más eficiente y confortable.

## 📐 Modelado del sistema

- Se consideró un vehículo promedio con torque de 145 Nm y masa de 1084 kg.
- Se modelaron perturbaciones como resistencia aerodinámica, de rodadura y por pendiente.
- El sistema fue representado mediante un **diagrama de bloques** con funciones de transferencia de:
  - Motor
  - Vehículo
  - Sensor de velocidad
  - Adaptadores de unidades

## 🧠 Diseño del Controlador

- Se implementó un **controlador PI**.
- Se utilizó la técnica de cancelación de polos dominantes.
- Se cumplió con las siguientes especificaciones:
  - Error en estado estable < 10 km/h
  - Tiempo de establecimiento entre 10-30 segundos
  - Sobrepasamiento < 10%

## 🧪 Simulaciones

Se realizaron simulaciones en **Matlab/Simulink**, incluyendo:
- Comparación entre sistema compensado y no compensado.
- Evaluación con perturbaciones (ruido blanco en el sensor).
- Análisis de estabilidad (criterio de Routh-Hurwitz, lugar de raíces).

## 📊 Resultados

| Métrica                     | Sin Compensar | Compensado |
|----------------------------|---------------|-------------|
| Vel. final [km/h]          | 86            | 100         |
| Tiempo de establecimiento  | 24.23 s       | 25.64 s     |
| Sobrepasamiento            | 2.52 %        | 4.3 %       |
| Error en estado estable [%]| 13.9 %        | 0 %         |

## 👨‍💻 Autores

- Gaspar Segura – Ingeniería en Computación
- Gastón Marcelo Segura – Ingeniería en Computación

---

**Docentes:**  
Mg. Ing. Juan Pablo Pedroni  
Ing. Adrián Claudio Agüero
