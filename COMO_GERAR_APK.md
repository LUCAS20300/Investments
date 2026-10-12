# Gerar o APK
## Opção A – GitHub (sem instalar nada)
1. Crie um repositório no GitHub e envie esta pasta (incluindo .github).
2. Aba Actions > "Build APK" > Run workflow.
3. Ao terminar, baixe o artefato `chocadeira-facil-apk` (app-debug.apk) e instale no celular.

## Opção B – No seu PC (Node 22, JDK 21, Android Studio)
npm install
npm install @capacitor/core @capacitor/cli @capacitor/android
npm run build
npx cap add android
npx cap sync android
cd android && ./gradlew assembleDebug
APK: android/app/build/outputs/apk/debug/app-debug.apk

## Opção C – PWABuilder.com
Publique o app (ex.: Vercel/Netlify) e gere o APK em pwabuilder.com.
