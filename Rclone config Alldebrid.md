Descargue el último archivo 'rclone.exe' desde aquí: https://github.com/itsToggle/rclone_RD/releases
Crea una carpeta en tu escritorio llamada "rclone" y ábrela.
Copie el archivo "rclone.exe" descargado a esa carpeta.
Windows 10: en el explorador de Windows abierto, haga clic en la cinta "Archivo" y luego haga clic en "Abrir PowerShell aquí" para abrir una terminal . Windows 11: haga clic derecho en la carpeta "rclone" en su escritorio. Mantenga presionada la shifttecla en su teclado y haga clic en "Mostrar más opciones". Seleccione "Abrir PowerShell aquí". Se abrirá una terminal.
Dentro de la terminal escribe el comando ./rclone.exe configy presiona enter
Escriba npara crear un nuevo control remoto rclone
Ingrese realdebridcomo nombre del control remoto
Ingrese 47para elegir el tipo de control remoto "realdebrid"
Ingrese su clave API de realdebrid ( https://real-debrid.com/apitoken )
Seleccione nocuando se le solicite editar la configuración avanzada
Siga el resto de las instrucciones indicadas.
Enter qpara salir del menú de configuración de rclone
Ingresa para montar realdebrid. Debería aparecer en tu computadora ./rclone.exe cmount realdebrid: X: --dir-cache-time 10suna nueva unidad virtual con la letra Xnombrada . Deberías encontrar 3 carpetas dentro de ella: "películas", "programas" y "predeterminado".realdebrid
Mantén la terminal abierta para que rclone siga ejecutándose. Si todo funciona y quieres ejecutar rclone en segundo plano, puedes cerrar la terminal y abrirla de nuevo como se describe en el paso 4. Ahora ejecuta el comando ./rclone.exe cmount alldebrid: X: --dir-cache-time 10s --no-console. La consola debería cerrarse y rclone debería ejecutarse en segundo 