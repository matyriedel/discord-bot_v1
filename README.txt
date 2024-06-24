✅ 1) Descargar Bot Cantidad Players y ponerlo en una carpeta del escritorio: 
(https://www.mediafire.com/file/deuzorz66j6u396/Bot+Cantidad+Players.rar/file)

✅ 2) Descargar e instalar Node JS en la pc:
(https://nodejs.org/es/download/)

✅ 3) Ir a Bot Cantidad Players en el escritorio abrir example_config.json y reemplazar:
- apiSite: 3
- apiUrl: https://api.battlemetrics.com/servers/12656299
- updateInterval: 10
Dejar abierto el archivo hasta tanto obtengas el resto de la config necesaria

✅ 4) Abrir un Chrome pegar discordapp.com/developers/applications como url: Loguearse con el discord del server si no estamos logueados. Solapa applications (izquierda), New Application (derecha), nombre Catarsis Players, create. Le agregás esta imagen de app icon: https://i.imgur.com/psb7kbG.png

✅ 5) Ahi mismo, salapa BOT a la izquierda, add bot. Buscás donde dice Click to reveal TOKEN y copias ese link entero.

✅ 6) Volvés al example_config.json y reemplazas el TOKEN por el copiado. Guardás el archivo.

✅ 7) En la web anterior (paso 5) de discord en chrome, solapa General Information, copiar el CLIENT ID y lo reemplazas en esta URL donde dice "YOUR_CLIENT_ID_HERE". Esto es para invitar al bot a tu discord.
https://discordapp.com/oauth2/authorize?&client_id=942925827333587005&scope=bot&permissions=0
Pones esa URL en chrome, le das enter y elegís el a donde tiene que ir el bot (en este caso, al discord de Catarsis)
MediaFire
Bot Cantidad Players

Node.js
Descarga | Node.js
Node.js® is a JavaScript runtime built on Chrome's V8 JavaScript engine.
Imagen

᲼
📌 PARTE 2: CARGANDO AUTOMATICAMENTE EL BOT CON WINDOWS
✅ 8) En la carpeta de Bot Cantidad Players, tocas File/Archivo, Abrir Windows Powershell y vas pegando estos comandos y dándole enter.
npm install (enter y esperár a que termine)
npm install -g node-windows (enter y esperár a que termine)
npm link node-windows (enter y esperár a que termine)
node installSVC.js (enter y esperár a que termine)

IMPORTANTE: Después de instalar estos, te crea un nuevo archivo config llamado example_config.json en la carpeta config, con valores default. Entonces vas a la carpeta del discord bot en el escritorio, abrís tu example_config.json y abrís el arcihvo config dentro de la carpeta config (seguramente se llame server1.json). En este último archivo pones exactamente la misma data que en el example_config.json. Después seguis con los comandos.

✅ 9) Una vez instalados esos 4 y cambiado el server1.json, ejecutas el BOT con el siguiente comando:
node app.js

✅ 10) Para desinstalarl abris el power shell y pones:
uninstallSVC.js
Seguro saltó el logo de Día Zero porque es el tuto que nos guardamos y abrá algo, pero fijate bien y adapta el nombre/imagen de lo que sea necesario