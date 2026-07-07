# 🔒 Auditoría Interna de Seguridad Informática y Cumplimiento Normativo
## Empresa: Botium Toys (Fictional Scenario)
**Rol:** Auditor de Ciberseguridad / Trainee en Seguridad de la Información
**Enlace al Portafolio:** [EduardoJavier45 - GitHub](https://github.com/EduardoJavier45/EduardoJavier45)

---

## 📝 1. Resumen Ejecutivo y Escenario de Negocio
**Botium Toys** es una pequeña empresa estadounidense dedicada al desarrollo y venta de juguetes que cuenta con una única ubicación física que funciona como oficina principal, escaparate de ventas y almacén. Debido a un acelerado y exitoso crecimiento en su presencia digital, la empresa ha expandido su mercado en línea atrayendo a clientes tanto locales como internacionales en la Unión Europea (UE). 

Este crecimiento global ha incrementado significativamente la presión operativa sobre el departamento de Tecnologías de la Información (TI), operando actualmente bajo una infraestructura vulnerable y **sin un plan formal de ciberseguridad**, lo que eleva el riesgo de incidentes, brechas de datos y sanciones legales.

### 🎯 Objetivos de la Auditoría
* **Evaluar la infraestructura actual:** Analizar el estado de los controles de seguridad administrativos, técnicos y físicos de la organización frente a estándares de la industria.
* **Identificar riesgos latentes:** Proveer una visión clara sobre las amenazas, vulnerabilidades y potenciales multas financieras derivadas de la postura de seguridad actual.
* **Garantizar el cumplimiento internacional:** Evaluar el nivel de alineación de los procesos internos de pagos y captación de datos personales con normativas globales vigentes (**PCI-DSS** y **GDPR**).

---

## 📊 2. Lista de Comprobación de Controles y Cumplimiento (Checklist)

Se aplicaron los lineamientos estratégicos del **Marco de Ciberseguridad del NIST (NIST CSF)** y del modelo fundacional de la **Tríada CID** (Confidencialidad, Integridad y Disponibilidad) para auditar las salvaguardas vigentes de la organización:

### A. Controles de Seguridad Administrativos
*¿Cuenta la organización con salvaguardas documentadas y políticas formales de gestión de riesgos?*

| Control Administrativo | ¿Implementado? | Justificación Técnica |
| :--- | :---: | :--- |
| **Políticas de Seguridad de la Información** | **NO** | La dirección de TI confirma que la empresa ha crecido orgánicamente sin un plan claro ni directrices documentadas de seguridad. |
| **Principio de Menor Privilegio (IAM)** | **NO** | No existen políticas de identidad ni roles estructurados que restrinjan el acceso de los empleados a información de bases de datos sensibles. |
| **Planes de Continuidad del Negocio (BCP)** | **NO** | La organización carece de una estrategia de resiliencia ante desastres para mantener la productividad durante crisis operativas. |
| **Planes de Respuesta a Incidentes (IRP)** | **NO** | No se dispone de manuales de estrategia (*playbooks*) operativos ni flujos organizados para contener o remediar ataques en progreso. |
| **Capacitación en Concientización** | **NO** | El personal de la empresa no recibe entrenamiento en ciberhigiene para identificar técnicas de Ingeniería Social, Phishing o Vishing. |

### B. Controles de Seguridad Técnicos
*¿Están configuradas las herramientas de software para proteger el ciclo de vida de los datos e infraestructura?*

| Control Técnico | ¿Implementado? | Justificación Técnica |
| :--- | :---: | :--- |
| **Mecanismos de Autenticación (Contraseñas)** | **SÍ** | Se cuenta con la configuración de autenticación local predeterminada del sistema operativo para el inicio de sesión del personal. |
| **Autenticación de Múltiples Factores (MFA)** | **NO** | No se encuentra habilitado un segundo factor de verificación, permitiendo vectores de ataque por fuerza bruta o robo de credenciales. |
| **Software Antivirus / Antimalware** | **SÍ** | Existe una solución básica para la protección de los endpoints corporativos, requiriendo monitorización continua y actualizaciones de firmas. |
| **Herramientas de Monitorización (SIEM / IDS)** | **NO** | Ausencia total de herramientas para la centralización de logs y visibilidad en tiempo real, imposibilitando el análisis oportuno de patrones anómalos. |
| **Cifrado de Datos (En tránsito y en reposo)** | **NO** | Los flujos financieros y la Información de Identificación Personal (PII) viajan en texto plano, vulnerando severamente la confidencialidad. |
| **Firewalls (Cortafuegos Perimetrales)** | **SÍ** | Se dispone de un firewall perimetral básico configurado para gestionar y restringir parcialmente el tráfico de red de la sede física. |

### C. Controles de Seguridad Físicos
*¿Se encuentran físicamente protegidos los accesos e instalaciones críticas de la organización?*

| Control Físico | ¿Implementado? | Justificación Técnica |
| :--- | :---: | :--- |
| **Sistemas de Videovigilancia (CCTV)** | **SÍ** | La única oficina, escaparate de ventas y almacén cuentan con cámaras instaladas para el monitoreo de seguridad física local. |
| **Personal de Control / Guardias** | **NO** | No se dispone de guardias de seguridad o personal exclusivo asignado para la custodia activa de los accesos a los activos físicos. |
| **Cerraduras Físicas Perimetrales** | **SÍ** | Los puntos de acceso críticos, almacenes y oficinas cuentan con cerrojos convencionales mecánicos instalados. |
| **Tarjetas Magnéticas / Control Biométrico** | **NO** | Los puntos de acceso a zonas sensibles de almacenamiento no están regulados por sistemas electrónicos ni mecanismos de autenticación biométrica. |

---

## ⚖️ 3. Evaluación de Cumplimiento Normativo (Conformidad)

| Estándar / Ley Regulatoria | ¿Se Cumple? | Impacto Organizacional Identificado |
| :--- | :---: | :--- |
| **PCI-DSS** *(Payment Card Industry Data Security Standard)* | **NO** | **Incumplimiento Crítico.** Al procesar, almacenar y aceptar pagos con tarjetas de crédito en línea sin aplicar cifrado criptográfico ni restringir accesos, la empresa está expuesta a la exfiltración de datos financieros y a severas multas por parte de las marcas de tarjetas. |
| **GDPR** *(General Data Protection Regulation)* | **NO** | **Incumplimiento Legal Internacional.** Botium Toys comercializa activamente en la Unión Europea (UE). Capturar, almacenar y procesar Información de Identificación Personal (PII) de ciudadanos europeos sin cifrado ni políticas estrictas de privacidad puede acarrear sanciones de hasta el 4% de la facturación global. |
| **Leyes de Privacidad Locales** *(Protección de Datos PII)* | **NO** | **Incumplimiento Operativo.** La ausencia de políticas documentadas sobre la retención, ciclo de vida útil y destrucción segura de datos sensibles compromete la responsabilidad corporativa frente a los estándares de privacidad legales vigentes en EE. UU. e internacionales. |

---

## 🛠️ 4. Recomendaciones del Auditor

De acuerdo con el análisis forense inicial del escenario, se recomienda a la gerencia priorizar los siguientes planes de remediación técnica y organizativa para mitigar de raíz las brechas críticas descubiertas:

1.  **Cifrado Criptográfico Integral (Mitigación de GDPR y PCI-DSS):** Implementar de forma inmediata el cifrado de datos en tránsito (protocolos TLS/HTTPS en el portal e-commerce) y datos en reposo para todas las bases de datos de clientes y pasarelas de pago.
2.  **Despliegue Obligatorio de MFA:** Configurar la Autenticación de Múltiples Factores en todos los portales de empleados y consolas de administración informática para neutralizar ataques basados en credenciales comprometidas.
3.  **Implementación de Solución SIEM:** Integrar un sistema de Gestión de Eventos e Información de Seguridad para centralizar y correlacionar los registros (*logs*) de la red, facilitando un *triage* efectivo y la detección temprana de intrusiones.
4.  **Desarrollo de Manuales de Estrategia (Playbooks):** Documentar planes formales paso a paso de respuesta a incidentes comunes (como ataques de Malware o campañas de Phishing), automatizando y estandarizando la contención operativa.

---
*Este reporte ha sido elaborado bajo un enfoque de mejora continua de procesos y aseguramiento de la calidad en la cadena de valor tecnológica de la empresa.*
