# Clara para Android

O projeto gera um APK Android instalável e não precisa ser hospedado. A tela do app é incluída no próprio APK; uma conexão com a internet é necessária para consultar as cotações da brapi.

## Gerar o APK

Com Java 17 e Android SDK (plataforma 35) instalados:

```bash
./gradlew assembleDebug
```

O APK de depuração será gerado em `app/build/outputs/apk/debug/app-debug.apk`. Para instalar em um aparelho Android conectado com depuração USB ativada:

```bash
adb install -r app/build/outputs/apk/debug/app-debug.apk
```
