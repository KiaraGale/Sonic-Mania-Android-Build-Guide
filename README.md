# ADVERTENCIA
Este tutorial no me pertenece todos los creditos a la (el) usuari@ (no me quiero meter en lios por pronombres) [KiaraGale](https://github.com/KiaraGale) por hacer el [Tutorial original](https://github.com/KiaraGale/Sonic-Mania-Android-Build-Guide)

# Decompilacion de Sonic Mania: ¿Como Compilar para android?

Esta es una guia para compilar tu propio APK de Sonic Mania APK. Esta guia esta diseñada para windows 10/11. Pronto habra una para linux

## Instrucciones (Windows)

1. Descargar y instalar Git por medio [de este enlace](https://gitforwindows.org/) *No hacer si ya lo tienes

2. Descargar y instalar Android Studio por medio [de este enlace](https://developer.android.com/studio) *No hacer si ya lo tienes

3. Descargar el script llamado **Sonic Mania Android Build Helper** por medio [de este enlace](https://raw.githubusercontent.com/SM2010Ficial/Sonic-Mania-Android-Build-Guide-espa-ol-/main/ManiaAndroidBuildHelper_2.0%20(espa%C3%B1ol).bat). Preciona "Ctrl + S" despues de clickear el link, y guardalo como `.bat`. Este script automatizara un monton de partes dificiles referentes a android studio.esto para hacer la compilacion mas facil.

4. Coloca `ManiaAndroidBuildHelper_2.0 (español).bat` en el lugar que mas te plazca

5. Haz click derecho sobre `ManiaAndroidBuildHelper_2.0 (español).bat` y luego dale click a "Ejecutar Como Administrador". Esto es muy importante. ***Si no lo ejecutas como Administrador, el script fallara y no compilara correctamente!!***

6. Sigue las direcciones en el CMD. Si quieres puedes precionar `s` (y enter obiamente) 2 veces para tener los Controles Tactiles y el soporte para pantallas ultra anchas, aun asi no son tecnicamente necesarios.

7. Una vez que el script diga `INSTALACION COMPLETA`, abre Android Studio. luego dale Click a `File` en la barra superior, luego dale click a `Open`, ahora ve a esta ubicacion `C:\Users\*TUUSUARIO\Sonic-Mania-Android-Sheeple\Sonic-Mania-Decompilation\dependencies\RSDKv5\android` (remplaza '*TUUSUARIO' con el nombre que tenga tu carpeta "Users") y luego dale click en `OK`. Android Studio va a hacer algunas cosas para poder importar el proyecto.

8. Asegurate que tengas instalada la ultima vercion de las "SDK tools". Puedes verificar esto yendo a "Tools --> SDK Manager". Ahora ve a la seccion `SDK Tools`. Si la ultima vercion de: `Android SDK Build-Tools 33`, `NDK (Side-by-Side)`, `CMake`, y `Android SDK Platform-Tools` no estan instaladas, haz click en los cuadrados y luego dale a `Apply`. Eso hara que automaticamente se descarguen las ultimas verciones de esas cosas. Cuando termine, preciona el boton que dice `Finish` para asi que el proyecto se sincronize con las cosas recien instaladas.

9. Eventualmente, Android Studio te va advertir en la esquina inferior derecha que tienes que actualizar algo que se llama "Gradle". esto es  necesario para que se compile correctamente asi que actualizalo.

10. Si tu solo quieres juegar el juego (sin cosas de depuracion y tal), ve a `Build --> Build Project`. Al instante Android Studio empezara a compilar tu APK, luego de terminar, tu apk estara en `C:\Users\username\Sonic-Mania-Android-Sheeple\Sonic-Mania-Decompilation\dependencies\RSDKv5\android\app\build\outputs\apk\debug`.

# 11. Este paso es solo para los que quieran jugar la RELEASE build. Si estas usando una Debug build, ve al paso 12.

11. Antes de que se compilete, ve a "Build --> Generate Signed Bundle/APK". Esto te va a abrir una seccion con muchos cuadrrados para llenar, Solo sigue estos pasos y todo saldra bien:
- 11a. Selecciona "APK" en la primera pagina, luego dale a "next" (esquina inferior derecha)

- 11b. En esta seccion hay 4 cuadrados: `Key store path`, `Key store password`, `Key alias`, y `Key password`.

- 11c. Para `Key store path`, dale click en el icono de la carpeta y ve a esta direccion `C:\Users\username\Sonic-Mania-Android-Sheeple\Sonic-Mania-Decompilation\dependencies\RSDKv5\android`. Deberia haber un archivo llamado `release-key.jks`. Escoje ese archivo.

- 11d. Para los otros 3 solo pon esto:
- **Key store password**: `retroengine`
- **Key alias**: `key0`
- **Key password**: `retroengine`

- 11e. Dale click en "Next", y luego escoje `release`. Al instante Android Studio empezara a compilar tu APK, luego de terminar, tu apk estara en `C:\Users\username\Sonic-Mania-Android-Sheeple\Sonic-Mania-Decompilation\dependencies\RSDKv5\android\app\release`.

# 12. Configurando los mods requeridos
- 12a. Instala tu APK de Mania y ejecuta la aplicacion. No habra nada pero eso se puede arreglar.

- 12b. Descargar el archivo `mods.zip` por medio [de este enlace](https://www.dropbox.com/s/czghcw7ps128qtj/mods.zip?dl=0).

- 12c. Extrae `mods.zip` en esta direccion: `[raiz]\RSDK\v5\mods`. Ahora deberias poder jugar sonic mania en tu telefono!

## Soporte

Si nececitas ayuda en algo, sientete libre de entrar a REMS ([Retro Engine Modding Server](http://dc.railgun.works/retroengine)) (aunque si vas a hacer esto tienes que saber ingles ya que hay muy pocos hispanohablantes en el servidor)
