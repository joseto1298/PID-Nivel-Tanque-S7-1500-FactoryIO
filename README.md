# Control PID de Nivel para Tanque de Agua (Siemens S7-1500 & FactoryIO)

## ⚙️ Descripción del Proyecto

Este repositorio contiene la implementación de un **Controlador Proporcional-Integral-Derivativo (PID)** para mantener un nivel de agua constante en un tanque, utilizando un **PLC Siemens S7-1500** programado en **TIA Portal** y simulado en tiempo real con **FactoryIO**.

El objetivo principal es demostrar la aplicación práctica de la función `PID_Compact` de Siemens para lograr un control de proceso robusto y preciso en un entorno de automatización industrial simulado.

## 🛠️ Tecnologías Utilizadas

| Componente | Tecnología | Versión/Detalle | Función en el Proyecto |
| :--- | :--- | :--- | :--- |
| **Controlador Lógico** | Siemens SIMATIC S7-1500 | CPU 1511-1 PN (Simulado) | Ejecución del algoritmo de control PID. |
| **Software de Programación** | Siemens TIA Portal | V20 (o superior) | Desarrollo del programa PLC y configuración del `PID_Compact`. |
| **Simulación de Proceso** | FactoryIO | | Entorno virtual para la simulación del tanque de agua y sus actuadores/sensores. |
| **Algoritmo de Control** | `PID_Compact` | Objeto Tecnológico de TIA Portal | Implementación del lazo de control PID. |

## 💡 Conceptos Clave

*   **Control PID:** Un mecanismo de control de lazo cerrado que calcula un valor de "error" como la diferencia entre un valor medido (nivel actual) y un valor deseado (Set Point), y aplica una acción correctiva (apertura de válvula) basada en términos Proporcional, Integral y Derivativo.
*   **TIA Portal:** Entorno de ingeniería unificado de Siemens para la configuración, programación y diagnóstico de controladores SIMATIC.
*   **FactoryIO:** Software de simulación 3D que permite crear y ejecutar escenarios industriales virtuales, facilitando la prueba de programas de PLC.

## 📂 Estructura del Repositorio

El repositorio incluye los archivos esenciales para replicar el proyecto:

*   `Control PID de nivel_V20.zap20`: Archivo de proyecto archivado de TIA Portal (V20), que contiene la configuración del PLC, el programa Ladder/SCL y la instancia del bloque `PID_Compact`.
*   `Control PID de Nivel para Tanque de Agua S7-1500.factoryio`: Archivo de escena de FactoryIO con la configuración de drivers y la conexión al PLC virtual.
*   `Tia Portal Main.png`: Captura de pantalla del bloque de organización principal (OB1) en TIA Portal.
*   `Tia Portal PID.png`: Captura de pantalla de la configuración del bloque `PID_Compact`.
*   `LICENSE`: Licencia MIT del proyecto.

## 🚀 Puesta en Marcha

Para ejecutar la simulación, siga los siguientes pasos:

1.  **Restaurar Proyecto TIA Portal:** Abra TIA Portal y restaure el archivo `Control PID de nivel_V20.zap20`.
2.  **Iniciar PLCSIM Advanced:** Inicie la simulación del PLC S7-1500 (por ejemplo, con PLCSIM Advanced).
3.  **Cargar Programa:** Cargue el programa en el PLC simulado.
4.  **Abrir FactoryIO:** Abra el archivo de escena `.factoryio` en FactoryIO.
5.  **Configurar Drivers:** En FactoryIO, configure los drivers para conectar con el PLC simulado (Driver Siemens S7-1500/1200).
6.  **Ejecutar Simulación:** Ponga el PLC en modo **RUN** y la simulación de FactoryIO en modo **Play**.

## 📺 Funcionamiento y Resultados

A continuación, se presentan los recursos visuales que demuestran el funcionamiento del control PID, incluyendo la sintonización automática y la respuesta del sistema ante cambios en el Set Point.

| Tipo de Recurso | Descripción | Enlace |
| :--- | :--- | :--- |
| **Video Demostrativo** | Muestra la sintonización del PID y la respuesta del nivel del tanque a perturbaciones. | [Ver en YouTube](https://youtu.be/sQOj4CUoOwk) |
| **Imágenes de Configuración** | Capturas de pantalla de la configuración del PLC y el bloque PID en TIA Portal. | Ver abajo |


### Capturas de Pantalla de TIA Portal

**Bloque de Organización Principal (OB1)**

![Bloque de Organización Principal](https://github.com/joseto1298/PID-Nivel-Tanque-S7-1500-FactoryIO/blob/main/Tia%20Portal%20Main.png)

**Configuración del Bloque PID_Compact**

![Configuración del Bloque PID_Compact](https://github.com/joseto1298/PID-Nivel-Tanque-S7-1500-FactoryIO/blob/main/Tia%20Portal%20PID.png)


## 📄 Licencia

Este proyecto está bajo la **Licencia MIT**. Consulte el archivo [LICENSE](LICENSE) para más detalles.

## 👤 Autor

**joseto1298**

*   [GitHub Profile](https://github.com/joseto1298)
*   [LinkedIn Profile](https://www.linkedin.com/in/-josetomas)
