# 🍊 Proyecto IAM & Ciberseguridad - Caso Naranja X

Este repositorio contiene una solución integral de Gestión de Identidades y Accesos (IAM) diseñada para mitigar riesgos de fraude y automatizar el ciclo de vida de identidades en un entorno financiero.

## 🚀 Desafío del Proyecto
Implementar un sistema que combine automatización por código, monitoreo en tiempo real y cumplimiento de normativas de auditoría para la protección de cuentas de usuarios.

## 🛠️ Tecnologías Utilizadas
- **Python (Pandas & Openpyxl)**: Automatización de desaprovisionamiento y limpieza dinámica de datos.
- **Power BI & DAX**: Tableros de control y métricas de auditoría cruzada.
- **Protocolos de Identidad**: Documentación estratégica sobre SSO, SAML y OAuth 2.0.
- **Git & GitHub**: Control de versiones y documentación técnica.

## 📋 Funcionalidades Implementadas
1. **Automatización de Bloqueo**: Script en Python que detecta intentos fallidos de inicio de sesión y bloquea identidades de forma automática si superan el umbral de riesgo.
2. **Dashboard de Monitoreo**: Visualización en Power BI de usuarios activos vs. bloqueados.
3. **Auditoría de Riesgo**: Implementación de lógica DAX para detectar inconsistencias (ej: transacciones fraudulentas de usuarios que aún figuran como activos).
4. **Gobierno de Datos**: Gestión de una "Fuente Única de Verdad" centralizada para reportes y automatizaciones.

## 📄 Documentación Técnica Incluida
- [Estándares de Autenticación (SSO, SAML, OAuth)](./ESTANDARES_AUTENTICACION.md)
- [Proceso de Auditoría y Hallazgos](./PROCESO_AUDITORIA.md)
