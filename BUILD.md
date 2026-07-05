# Phone Simulator - Android App

## Структура проекта
```
android-app/
├── app/
│   ├── src/main/
│   │   ├── assets/public/index.html  (веб-приложение)
│   │   ├── java/com/phonesimulator/app/MainActivity.java
│   │   ├── res/ (ресурсы: иконки, стили, цвета)
│   │   └── AndroidManifest.xml
│   └── build.gradle
├── build.gradle
├── settings.gradle
├── gradle.properties
├── capacitor.config.json
└── package.json
```

## Что сделано:
1. ✅ Добавлена анимация иконок приложений (появление, пульсация при наведении)
2. ✅ Создан Android проект с WebView
3. ✅ Настроены иконки приложения

## Как собрать APK:

### Вариант 1: Через Android Studio
1. Открой папку `android-app` в Android Studio
2. Дождись синхронизации Gradle
3. Build → Build Bundle(s) / APK(s) → Build APK(s)

### Вариант 2: Через онлайн-сервис (рекомендуется)
1. Загрузи папку `android-app` на GitHub
2. Используй https://github.com/nickbutler/asset-merge или аналоги
3. Или используй https://capacitorjs.com/docs/guides/deploying-to-app-stores

### Вариант 3: Сборка через командную строку (требуется Android SDK)
```bash
cd android-app
./gradlew assembleDebug
```

## Логотип
Текущий логотип ссылается на `1774775893.png`. Для использования кадра из видео:
1. Извлеки кадр из видео с помощью ffmpeg: `ffmpeg -i video.mp4 -ss 00:00:01 -vframes 1 logo.png`
2. Сохрани файл как `1774775893.png` в папку `app/src/main/assets/public/`
