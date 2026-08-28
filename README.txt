RADIO ONLINE - PWA
==================

Archivos:
- index.html
- manifest.webmanifest
- sw.js
- icon-192.png
- icon-512.png

CONFIGURACIÓN DE LA SEÑAL
-------------------------
En la PC donde está Icecast puedes usar:
http://127.0.0.1:8000/radio

En un celular NO uses 127.0.0.1 porque apuntaría al propio celular.

Si el teléfono está en la misma red Wi‑Fi que la PC:
1. En Windows abre CMD.
2. Ejecuta: ipconfig
3. Busca "Dirección IPv4", por ejemplo 192.168.1.50
4. En la web, Ajustes > URL de transmisión:
   http://192.168.1.50:8000/radio
5. URL de estado opcional:
   http://192.168.1.50:8000/status-json.xsl

IMPORTANTE PARA USO FUERA DE CASA/RED LOCAL
-------------------------------------------
Necesitarás publicar Icecast en Internet con una URL accesible desde fuera.
Para una PWA pública alojada en HTTPS, lo recomendable es que la señal de audio
también esté disponible por HTTPS; de lo contrario, algunos navegadores pueden
bloquear el audio por contenido mixto.

INSTALACIÓN PWA
---------------
La PWA debe servirse desde HTTPS (o localhost para pruebas).
No basta con abrir index.html directamente desde el Explorador de archivos.

Puedes subir esta carpeta a un hosting estático compatible con HTTPS.
Una vez publicada, Chrome/Edge/Android podrán ofrecer "Instalar aplicación".

SEGURIDAD
---------
No expongas el panel de administración de Icecast sin una contraseña fuerte.
