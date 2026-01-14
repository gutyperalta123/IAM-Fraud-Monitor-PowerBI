# Administración y Optimización de Sistemas de Autenticación - Proyecto IAM Naranja X

## Objetivo
Centralizar la autenticación de la App Naranja X mediante protocolos estándar para mejorar la seguridad y la experiencia de usuario (SSO).

## Protocolos Implementados
- **SAML 2.0**: Utilizado para la federación de identidades en aplicaciones web corporativas, permitiendo el intercambio seguro de aserciones XML.
- **OAuth 2.0 / OIDC**: Implementado para la autorización en la aplicación móvil, utilizando flujos de 'Authorization Code' con PKCE para mitigar ataques de interceptación.

## Optimización de Seguridad
Para maximizar la seguridad en Naranja X, se aplicaron las siguientes optimizaciones:
1. **Control de Scopes**: Restricción de permisos en los tokens de OAuth para seguir el principio de Menor Privilegio (Ej: `openid profile email` únicamente).
2. **MFA Enforcement**: Configuración de políticas de acceso condicional para exigir un segundo factor de autenticación en logins desde redes externas.
3. **SSO (Single Sign-On)**: Integración con el IdP central para reducir la fatiga de contraseñas y unificar el ciclo de vida de la identidad.
