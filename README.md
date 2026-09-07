# VIRUS-INFORMATICOS

```markdown
# 🛡️ Investigación: Virus Informáticos y Ciberseguridad

Este repositorio contiene una guía explicativa y visual sobre los tipos de virus, categorías de malware, métodos de prueba inofensivos y estrategias de protección para sistemas informáticos.

---

## 1. 🦠 Tipos de Virus Informáticos

Los virus se clasifican principalmente según el **objetivo del sistema** que infectan y su **mecanismo de propagación**:


```

┌──────────────────────────────────────────────────────────┐
│               TIPOS DE VIRUS INFORMÁTICOS               │
├─────────────────┬────────────────────────────────────────┤
│ 📄 Archivos     │ Infecta ejecutables (.exe, .com)       │
│ 🔌 Arranque     │ Ataca el sector MBR del disco duro     │
│ 📝 Macro        │ Se ejecuta en docs (Word, Excel)       │
│ 🧬 Multipartito │ Combina infección de MBR y archivos    │
│ 🧠 Residente    │ Se aloja directamente en la memoria RAM│
└─────────────────┴────────────────────────────────────────┘

```

* **📄 Infectores de archivos:** Se adhieren a programas ejecutables (`.exe`, `.dll`, `.com`). Al ejecutar el programa, el virus se activa.
* **🔌 Sector de Arranque (Boot Sector):** Infecta el Registro de Arranque Maestro (MBR) del disco duro, ejecutándose antes de que cargue el sistema operativo.
* **📝 Macro Virus:** Escrito en lenguajes de macros integrados en documentos de ofimática (Word, Excel). Se activa al abrir el archivo.
* **🧬 Virus Multipartitos:** Posee capacidad dual para infectar tanto el sector de arranque como los archivos ejecutables simultáneamente.
* **🧠 Residentes en RAM:** Permanece oculto en la memoria principal del equipo para interceptar y controlar las operaciones del sistema operativo.

---

## 2. 🎭 Categorías de Virus

Clasificación según su **comportamiento**, capacidades de **evasión** y arquitectura de ataque:


```

```
              ┌──────────────────────┐
              │ CATEGORÍAS DE VIRUS  │
              └──────────┬───────────┘
     ┌───────────────────┼───────────────────┐
     ▼                   ▼                   ▼

```

🧬 Polimórficos     🥷 Sigilosos        🐴 Troyanos
Cambian su código   Ocultan cambios     Abren puertas
en cada infección   de tamaño/fecha     traseras (Backdoors)

```

* **🧬 Polimórficos / Metamórficos:** Cambian su estructura de código o encriptación en cada nueva infección para burlar la detección por firmas de los antivirus.
* **🥷 Sigilosos (Stealth):** Interceptan las solicitudes del sistema operativo para falsificar información y ocultar modificaciones en el tamaño o fecha de los archivos.
* **🐴 Troyanos:** Se presentan como programas legítimos u útiles, pero al ejecutarse abren accesos no autorizados (*backdoors*) para atacantes remotos.
* **🌐 Secuestradores de Navegador (Hijackers):** Modifican la configuración del navegador web (página de inicio, buscador predeterminado) para redirigir tráfico a sitios maliciosos.

---

## 3. 🧪 Creación de Virus de Daño Bajo (Conceptos de Prueba)

Para realizar pruebas académicas y de auditoría de seguridad sin poner en riesgo la estabilidad del equipo ni los datos, se utilizan métodos inocuos:

### ⚙️ A. Scripts Inofensivos de Prueba
Automatizaciones simples en scripts BATCH (`.bat`) o VBScript (`.vbs`) que solo muestran mensajes o crean archivos temporales para probar la ejecución sin causar daños.

### 🎯 B. Cadena de Prueba Estándar EICAR
Es un estándar internacional aceptado por la industria de ciberseguridad. Se trata de un archivo de texto inofensivo que cualquier antivirus debe detectar e interceptar inmediatamente como si fuera un virus real:

```text
X5O!P%@AP[4\PZX54(P^)7CC)7}}$EICAR-STANDARD-ANTIVIRUS-TEST-FILE!$H+H*

```

---

## 4. 🛡️ Tipos de Protección (Defensa en Profundidad)

Estrategia multinivel para proteger la infraestructura y los datos frente a infecciones:

```
 ┌─────────────────────────────────────────────────────────────┐
 │                CAPAS DE PROTECCIÓN INFORMÁTICA              │
 ├─────────────────┬───────────────────────────────────────────┤
 │ 🔍 Antivirus    │ Análisis en tiempo real, firmas y heurística│
 │ 🧱 Firewall     │ Control de puertos y filtrado de red      │
 │ 🔄 Parches      │ Actualizaciones continuas del sistema     │
 │ 💾 Backups      │ Respaldos periódicos fuera de línea       │
 │ 🧑‍💻 Educación   │ Prevención contra Phishing e Ing. Social  │
 └─────────────────┴───────────────────────────────────────────┘

```

1. **🔍 Protección Activa (Antivirus/Anti-Malware):** Monitoreo constante mediante firmas conocidas y análisis heurístico para detectar comportamientos sospechosos.
2. **🧱 Cortafuegos (Firewall):** Bloqueo y filtrado del tráfico de red saliente y entrante no autorizado.
3. **🔄 Gestión de Parches:** Mantener el sistema operativo y las aplicaciones actualizadas para cerrar vulnerabilidades (*exploits*).
4. **💾 Copias de Seguridad (Backups):** Respaldos periódicos de la información crítica guardados en medios desconectados (*offline*) para mitigar ataques de secuestro de datos.
5. **🧑‍💻 Educación del Usuario:** Capacitación en hábitos de navegación segura para evitar engaños por ingeniería social o correos fraudulentos (*phishing*).

---

## 5. ⚠️ 10 Tipos de Malware y sus Daños

| Icono | Malware | Descripción / Daño Principal |
| --- | --- | --- |
| 🔒 | **Ransomware** | Cifra los archivos del sistema y exige un rescate económico para devolver el acceso. |
| 🕵️ | **Spyware** | Recopila en secreto hábitos de navegación, información personal y credenciales. |
| 🪱 | **Gusano (Worm)** | Se replica autónomamente por la red consumiendo ancho de banda y recursos. |
| 📢 | **Adware** | Despliega publicidad masiva no deseada y ralentiza la navegación. |
| ⌨️ | **Keylogger** | Registra todas las pulsaciones de teclado para robar contraseñas y datos bancarios. |
| 👤 | **Rootkit** | Proporciona acceso administrativo oculto a nivel de kernel de forma no detectada. |
| 🤖 | **Botnet** | Recluta el equipo en una red "zombi" para lanzar ataques masivos de denegación de servicio (DDoS). |
| 🚨 | **Scareware** | Muestra falsas alertas de infección para engañar al usuario e inducirlo a comprar software estafa. |
| 🎯 | **Exploit Kit** | Aprovecha fallos de seguridad no corregidos en el navegador o programas para infectar el equipo. |
| 🏦 | **Troyano Bancario** | Intercepta sesiones de banca en línea y códigos SMS/MFA para realizar fraudes financieros. |

```

```
