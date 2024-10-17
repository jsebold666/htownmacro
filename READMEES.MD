# Script Bot HTown para Integración con Webhook de Discord

Esta guía explica cómo instalar las bibliotecas `requests` y `discord_webhook`, configurar un webhook de Discord y configurarlo como una variable de entorno para su uso en tus scripts de Python.

## Requisitos

- Python (se recomienda la versión 3.x)
- Acceso a Internet para descargar paquetes
- Requests
- Discord_webhook

## Instalación

1. **Abre tu terminal (Mac/Linux) o símbolo del sistema (Windows).**

2. **Instala las bibliotecas requeridas:**

   - Para instalar la biblioteca `requests`, ejecuta:
     ```bash
     pip install requests
     ```

   - Para instalar la biblioteca `discord_webhook`, ejecuta:
     ```bash
     pip install discord-webhook
     ```

3. **Crear un Webhook de Discord**

   Ve a la configuración de tu servidor de Discord y navega al canal donde deseas recibir los mensajes.  
   Haz clic en **Integraciones** y luego en **Webhooks**.  
   Haz clic en **Nuevo Webhook**, asígnale un nombre y copia la URL del Webhook.

4. **Actualizar variables de webhooks**

   - Abre `script.py` y coloca la URL del webhook en la línea 13:  
     ```python
     DISCORD_WEBHOOK_HTOWN = "tu_webhook_url"
     ```

   - Abre `common_utils.py` y coloca la URL del webhook en la línea 77:  
     ```python
     DISCORD_WEBHOOK_HTOWN = "tu_webhook_url"
     ```

   - Abre `script.py` y cambia la línea 44:  
     ```python
     PASSARO_ONLY = False
     ```
     Si está en `True`, irá solo al "clawser"; si está en `False`, no irá solo.  
     Si está en `False`, puedes usarlo con otros mobs.

5. **Ejecutar el Script**

   Debes abrir `script.py` en UOStealth y ejecutarlo.  
   ¡Magia!