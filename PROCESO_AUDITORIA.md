# Proceso de Auditoría de Accesos (UAR) - Naranja X

## Metodología
Se implementó un control de auditoría cruzada entre los logs de transacciones y la base de identidades.

## Hallazgos de Seguridad
Utilizando DAX en Power BI, se creó un indicador de riesgo que detecta:
- Usuarios con transacciones fraudulentas confirmadas (`Es_Fraude = Si`).
- Cuentas que aún permanecen en estado `ACTIVO`.

## Acción Remediadora
Ante un hallazgo de "REVISIÓN URGENTE", el protocolo IAM establece:
1. Bloqueo manual inmediato de la identidad.
2. Revisión de privilegios otorgados.
3. Análisis de logs para ajustar el umbral del script de Python si fuera necesario.
