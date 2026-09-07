
# 🦠 Virus Informáticos

## 📚 Introducción

Los virus informáticos y otros tipos de malware son programas diseñados para afectar el funcionamiento de dispositivos, robar información, dañar archivos o realizar acciones no autorizadas.

En esta práctica se investigan los diferentes tipos de virus, categorías de malware, métodos de protección y algunos ejemplos de amenazas informáticas conocidas.

> ⚠️ **Nota:** La simulación incluida en esta práctica es únicamente educativa y no modifica, elimina, cifra ni roba archivos.

---

# 1. 🦠 Tipos de Virus

| Tipo de virus | Descripción |
|---|---|
| **Virus de archivo** | Se adjunta a archivos ejecutables y puede activarse cuando estos son ejecutados. |
| **Virus de sector de arranque** | Infecta el sector de arranque de un disco y puede afectar el inicio del sistema. |
| **Virus residente** | Permanece en la memoria del equipo y puede infectar otros archivos. |
| **Virus de macro** | Utiliza macros de documentos como Word o Excel para propagarse. |
| **Virus polimórfico** | Modifica parte de su código para intentar evitar la detección. |
| **Virus multipartito** | Puede infectar diferentes partes del sistema, como archivos y sectores de arranque. |
| **Virus de sobreescritura** | Sobrescribe el contenido de archivos y puede provocar pérdida de información. |
| **Virus de script** | Utiliza lenguajes de scripting para realizar acciones maliciosas. |

---

# 2. 🧩 Categorías de Malware

Aunque comúnmente se utiliza la palabra "virus" para cualquier amenaza informática, existen diferentes tipos de malware.

| Categoría | Descripción |
|---|---|
| **Virus** | Se replica infectando otros archivos. |
| **Gusano (Worm)** | Puede propagarse automáticamente entre computadoras y redes. |
| **Troyano** | Se presenta como un programa legítimo, pero realiza acciones maliciosas. |
| **Ransomware** | Cifra archivos y exige un pago para recuperarlos. |
| **Spyware** | Recopila información del usuario sin autorización. |
| **Adware** | Muestra publicidad no deseada. |
| **Keylogger** | Registra las pulsaciones realizadas en el teclado. |
| **Rootkit** | Intenta ocultar su presencia y mantener acceso al sistema. |
| **Botnet** | Convierte dispositivos infectados en equipos controlados remotamente. |
| **RAT** | Permite controlar determinadas funciones de un equipo de manera remota. |

---

# 3. 🧪 Creación de una Simulación de Virus de Daño Bajo

Para esta práctica se realizó una **simulación educativa y segura**.

El programa únicamente muestra una alerta simulada y no realiza ninguna acción dañina.

### Código de la simulación

```bat
@echo off
title Simulacion de Virus
echo =====================================
echo       SIMULACION EDUCATIVA
echo =====================================
echo.
echo Este programa NO es un virus real.
echo No modifica, elimina ni cifra archivos.
echo.
echo Se ha detectado una amenaza SIMULADA.
echo.
pause
¿Qué demuestra?

La simulación permite demostrar:

Ejecución de un archivo mediante CMD.
Uso de comandos básicos de Windows.
Presentación de mensajes al usuario.
Funcionamiento de un archivo .bat.
🔐 Seguridad

Esta simulación NO:

Elimina archivos.
Modifica archivos.
Cifra información.
Roba contraseñas.
Se propaga por la red.
Desactiva antivirus.
Oculta procesos.
4. 🛡️ Tipos de Protección

Existen diferentes métodos para proteger nuestros dispositivos.

Protección	Función
Antivirus	Detecta, bloquea y elimina diferentes tipos de malware.
Actualizaciones	Corrigen errores y vulnerabilidades de seguridad.
Firewall	Controla las conexiones de red entrantes y salientes.
Copias de seguridad	Permiten recuperar información perdida o dañada.
Contraseñas seguras	Ayudan a evitar accesos no autorizados.
Navegación segura	Reduce el riesgo de descargar archivos maliciosos.
Correo electrónico seguro	Evita abrir enlaces o archivos adjuntos sospechosos.
Control de permisos	Reduce las acciones que pueden realizar programas y usuarios.
5. 💻 Diez Virus y Malware Conocidos
#	Virus/Malware	Año	Daño principal
1	Brain	1986	Infectaba el sector de arranque de disquetes.
2	Michelangelo	1991	Podía sobrescribir sectores del disco y provocar pérdida de información.
3	Melissa	1999	Se propagaba mediante documentos de Word y correo electrónico.
4	ILOVEYOU	2000	Se propagó masivamente por correo electrónico y podía afectar archivos.
5	Code Red	2001	Explotaba vulnerabilidades de servidores Microsoft IIS y se propagaba por Internet.
6	Mydoom	2004	Se propagaba por correo electrónico y generaba gran cantidad de tráfico de red.
7	Conficker	2008	Infectó millones de computadoras aprovechando vulnerabilidades de Windows.
8	Stuxnet	2010	Atacó sistemas industriales y equipos utilizados para procesos de control.
9	WannaCry	2017	Cifraba archivos y exigía un pago para recuperarlos.
10	NotPetya	2017	Provocó daños e interrupciones importantes en empresas y organizaciones.
6. 🔎 ¿Cómo analizar si un dispositivo tiene virus usando CMD?

Windows cuenta con diferentes herramientas que pueden ayudar a revisar el estado del equipo.

6.1 Comprobar archivos del sistema
sfc /scannow

Este comando comprueba la integridad de determinados archivos protegidos de Windows y puede reparar archivos dañados.

6.2 Revisar procesos activos
tasklist

Muestra los procesos que actualmente están ejecutándose en el equipo.

6.3 Revisar conexiones de red
netstat -ano

Permite observar conexiones de red activas y los identificadores de los procesos relacionados.

6.4 Consultar Microsoft Defender

Desde CMD podemos consultar el estado de Microsoft Defender mediante PowerShell:

powershell Get-MpComputerStatus
6.5 Realizar un análisis rápido
powershell Start-MpScan -ScanType QuickScan

Este comando inicia un análisis rápido utilizando Microsoft Defender.

6.6 Realizar un análisis completo
powershell Start-MpScan -ScanType FullScan

Este comando inicia un análisis completo del equipo.

💡 Importante: Estos comandos sirven para diagnóstico y protección. La ausencia de resultados sospechosos no garantiza por sí sola que un equipo esté completamente libre de malware.

7. 📋 Recomendaciones de Seguridad

Para mantener un dispositivo protegido se recomienda:

Mantener Windows actualizado.
Mantener activo un antivirus confiable.
No descargar programas desde sitios desconocidos.
No abrir archivos adjuntos sospechosos.
No hacer clic en enlaces desconocidos.
Utilizar contraseñas seguras.
Activar la autenticación de dos factores cuando esté disponible.
Realizar copias de seguridad periódicas.
Evitar utilizar programas pirateados o de fuentes desconocidas.
Revisar periódicamente el dispositivo.
8. 📝 Conclusión

Los virus informáticos y otros tipos de malware representan una amenaza para la seguridad de los dispositivos y la información de los usuarios.

Conocer sus diferentes categorías permite identificar mejor los riesgos y tomar medidas de protección. Herramientas como Microsoft Defender, sfc, tasklist y netstat pueden ayudar a realizar comprobaciones básicas del sistema.

La mejor forma de prevenir una infección es mantener el sistema actualizado, utilizar herramientas de seguridad, realizar copias de seguridad y tener cuidado con los archivos, programas y enlaces que descargamos o abrimos.

👨‍💻 Información de la Práctica

Asignatura: Servicios Informáticos
Tema: Virus Informáticos
Actividad: Investigación y análisis de virus
Repositorio: Práctica de Virus Informáticos

📁 Contenido del Repositorio
Practica-Virus-Informaticos/
│
├── README.md
├── tipos-de-virus.md
├── categorias-malware.md
├── proteccion.md
├── 10-virus.md
└── simulacion-segura.bat
⚠️ Aviso de Uso Responsable

Este repositorio fue creado con fines educativos para aprender sobre seguridad informática.

Los ejemplos incluidos no están diseñados para causar daños, robar información, evadir sistemas de seguridad o afectar dispositivos de terceros.

La seguridad informática debe practicarse de manera responsable y únicamente en equipos y entornos autorizados.


### 📌 Nombre recomendado del repositorio

**`Practica-Virus-Informaticos`**

Y el archivo principal debe llamarse exactamente:

**`README.md`**

Con esto ya tienes la parte principal que pide el profesor: **investigación + tabla de virus + simulación
