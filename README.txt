BALANCEA ANDROID — PROYECTO PARA GENERAR APK

Este proyecto empaqueta la aplicación financiera Balancea en una app Android.
Los datos se guardan localmente dentro del WebView mediante localStorage.

MÉTODO FÁCIL: GENERAR APK GRATIS CON GITHUB ACTIONS

1. Descarga y descomprime este ZIP.
2. Crea una cuenta en https://github.com/ si no tienes una.
3. Crea un repositorio nuevo llamado BalanceaAndroid. Puede ser privado.
4. Sube el contenido de esta carpeta al repositorio (no subas el ZIP como un solo archivo).
5. Abre la pestaña Actions del repositorio.
6. Si GitHub pide habilitar Actions, habilítalo.
7. Abre el workflow "Build Balancea APK" y pulsa "Run workflow" (o espera a que termine el primer build después de subir los archivos).
8. Cuando el trabajo termine en verde, abre la ejecución y busca "Artifacts".
9. Descarga "Balancea-APK.zip" y descomprímelo. Dentro estará app-debug.apk.
10. Pasa el APK al teléfono Android y ábrelo. Si Android lo solicita, permite instalar aplicaciones desde esa fuente.

ALTERNATIVA: ANDROID STUDIO

1. Abre esta carpeta en Android Studio.
2. Espera a que Gradle sincronice el proyecto.
3. Usa Build > Build Bundle(s) / APK(s) > Build APK(s).
4. El APK de depuración aparecerá en app/build/outputs/apk/debug/app-debug.apk.

NOTAS IMPORTANTES

- Este es un APK de depuración, adecuado para instalar y probar en tu propio teléfono, no un lanzamiento firmado para Play Store.
- El proyecto requiere JDK 17 y Android SDK 35 para compilar.
- La app no pide permiso de internet: la interfaz está empaquetada dentro del APK.
- Los datos quedan guardados en el almacenamiento local de la app. Desinstalar la app puede borrar esos datos; exporta CSV periódicamente.
- El archivo APK todavía debe generarse ejecutando el workflow o compilando el proyecto. Este ZIP contiene el proyecto fuente, no el APK compilado.
