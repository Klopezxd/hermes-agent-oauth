# Hermes Agent — Integración Personal de Gmail

Páginas estáticas de presentación y política de privacidad para la aplicación OAuth de Google Cloud (`glossy-mason-510523-g7`) de **Hermes Agent**.

## Propósito
Esta aplicación es una integración privada y de uso exclusivamente personal diseñada para consultar metadatos de correos entrantes no leídos en Gmail y generar resúmenes periódicos para el titular vía Telegram.

- **URL de Página Principal:** [https://klopezxd.github.io/hermes-agent-oauth/](https://klopezxd.github.io/hermes-agent-oauth/)
- **URL de Política de Privacidad:** [https://klopezxd.github.io/hermes-agent-oauth/privacy.html](https://klopezxd.github.io/hermes-agent-oauth/privacy.html)

## Alcance OAuth Autorizado
- `https://www.googleapis.com/auth/gmail.metadata`

### Restricciones Técnicas
- Solo consulta metadatos de encabezados (`From`, `To`, `Date`, `Subject`) y etiquetas del sistema (`labelIds`).
- No accede al cuerpo de los mensajes (`body`), no descarga adjuntos ni lee `snippets`.
- No puede enviar correos (`gmail.send`), no puede borrar correos ni modificar estados en la bandeja.
- La restricción de consulta a correos no leídos es una política operativa del agente Hermes.

## Despliegue
Alojado en **GitHub Pages** desde la rama `main`.
Sin cookies, sin analítica ni rastreadores de terceros.
