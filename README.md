# Laboratorio 1 - Esquemas de comunicación

Este repositorio contiene los reportes y archivos generados durante el desarrollo del laboratorio enfocado en **la transmisión de información y el análisis de paquetes con Wireshark**. El trabajo fue dividido en dos partes: una actividad grupal de comunicación entre parejas y una introducción individual al uso de Wireshark.

## 📁 Estructura del repositorio

```bash
.
├── README.md
├── data/
│   └── Wireshark_Masterclass_Lesson1_Setup.pcapng
├── data1/
│   └── Archivos de captura (.pcapng)
├── data2/
│   └── Archivo de captura para enlace dado (.pcapng)
├── docs/
│   ├── reporte_grupal.md
│   └── reporte_individual.md
├── images/
│   └── Capturas de pantalla
├── reporte_individual.pdf
└── reporte_grupal.pdf
```

## 👥 Parte 1 - Comunicación entre parejas

Durante esta actividad se realizó una simulación de comunicación entre dos parejas utilizando distintos esquemas de codificación para transmitir información.

📄 Archivo: [`docs/reporte_grupal.md`](docs/reporte_grupal.md)  
📄 Versión PDF: [`reporte_grupal.pdf`](reporte_grupal.pdf)

### Contenido del reporte grupal

- Nombres y carnets de ambas parejas participantes.
- Respuestas analíticas sobre:
  - Facilidad de transmisión de los esquemas utilizados.
  - Dificultades encontradas al enviar mensajes empaquetados.
  - Ventajas y desventajas de agregar conmutadores.
  - Análisis de errores en cada esquema.
- Protocolo de comunicación utilizado en la parte del conmutador:
  - Cómo se determinó el destino del mensaje.
  - Medidas para evitar la sobrecarga del conmutador.

## 🧪 Parte 2 - Introducción a Wireshark

Esta parte fue individual y consistió en configurar el entorno de Wireshark, capturar paquetes de red, y realizar un análisis detallado del protocolo HTTP.

📄 Archivo: [`docs/reporte_individual.md`](docs/reporte_individual.md)  
📄 Versión PDF: [`reporte_individual.pdf`](reporte_individual.pdf)

### 1.1 Personalización del entorno Wireshark

- Creación de perfil personalizado.
- Ajustes visuales: columnas, formatos de tiempo, colores.
- Botón de filtro TCP con bandera SYN.
- Interfaz limpia con solo las interfaces necesarias visibles.

### 1.2 Captura de paquetes con Ring Buffer

- Se ejecutó `ifconfig`/`ipconfig` para identificar las interfaces activas.
- Se realizó una captura de tráfico con configuración de buffer circular:
  - 10 archivos de 5 MB.
  - Generación de tráfico real para activación.

### 1.3 Análisis del protocolo HTTP

- Captura y análisis de tráfico HTTP al visitar una página específica.
- Se respondieron preguntas relacionadas con:
  - Versión del protocolo.
  - Contenido transferido.
  - Idiomas aceptados por el navegador.
  - Elementos relevantes para diagnóstico de red.

## 📝 Entregables incluidos

- ✅ Reporte grupal (`.md` y `.pdf`)
- ✅ Reporte individual (`.md` y `.pdf`)
- ✅ Capturas de pantalla del entorno personalizado y análisis de paquetes
- ✅ Archivos `.pcapng` generados con configuración de ring buffer
- ✅ Archivo de práctica descargado de Cloudshark

## 🧾 Referencias

- [Documentación oficial de Wireshark](https://www.wireshark.org/docs/)
- [Enlace del archivo Cloudshark](https://www.cloudshark.org/captures/e6fb36096dbb)
- [Demystifying ifconfig and network interfaces in Linux](https://codewithyury.com/demystifying-ifconfig-and-network-interfaces-in-linux/)
- [Significado de campos en eth0](https://superuser.com/questions/1153104/when-i-type-in-ifconfig-to-the-command-line-what-does-the-information-mean)
- [RX errors and Frame in ifconfig output](https://serverfault.com/questions/185331/exact-meaning-of-rx-errors-and-frame-in-ifconfig-output)
