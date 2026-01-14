# Protocolo de Respuesta a Incidentes - IAM Naranja X

## Detección
Utilización del Dashboard de Power BI para monitorear anomalías en el estado de las cuentas. Un incremento inusual en 'DESACTIVADO - RIESGO' dispara una alerta de incidente de fuerza bruta.

## Contención (Playbook)
1. **Aislamiento**: El script de Python bloquea automáticamente las cuentas comprometidas al superar los 5 intentos fallidos.
2. **Investigación**: Cruce de datos con la columna 'Ubicación' para identificar si el ataque proviene de una geografía inusual (ej. IPs externas no corporativas).
3. **Erradicación**: Forzado de cambio de contraseña y reseteo de tokens de MFA para todos los usuarios afectados.

## Recuperación
Re-aprovisionamiento gradual de cuentas tras la validación de identidad por un canal seguro (Out-of-band).
