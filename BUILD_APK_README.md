# Сборка Android APK для FastCMS (`ru.fastcms.app`)

В архиве находится готовый проект Android-приложения для **FastCMS** (`https://fast-cms.ru/`).

## Что уже настроено в проекте
- Стартовый адрес: `https://fast-cms.ru/` (можно поменять в `app/src/main/res/values/strings.xml`, например на `https://fast-cms.online/`).
- Сохранение авторизации и cookies (сессии кабинета и суперадминки не сбрасываются).
- Загрузка фотографий и файлов из галереи в визуальный конструктор сайтов.
- Открытие внешних ссылок на Telegram (`t.me`), звонков (`tel:`) и почты (`mailto:`) в штатных приложениях телефона.
- Обновление страницы свайпом вниз (Pull-to-Refresh), экран при отсутствии интернета и обработка системной кнопки «Назад».
- Готовые иконки приложения FastCMS для всех разрешений экрана (`mipmap-mdpi` .. `mipmap-xxxhdpi`).

## Способ 1. Сборка готового `.apk` за 2 минуты через GitHub Actions (без установки Android Studio)
1. Создайте новый приватный репозиторий на GitHub и загрузите в него содержимое этого архива.
2. Откройте вкладку **Actions** → выберите **Build FastCMS Android APK** → нажмите **Run workflow**.
3. Через ~2 минуты внизу страницы сборки появится блок **Artifacts** → скачайте **`FastCMS-debug-apk`** — внутри готовый установочный файл `app-debug.apk` для Android.

## Способ 2. Сборка в Android Studio на ПК
1. Откройте папку `fastcms_android_apk_project` в **Android Studio**.
2. Дождитесь синхронизации Gradle.
3. В верхнем меню нажмите **Build → Build Bundle(s) / APK(s) → Build APK(s)**.
4. Готовый файл появится по пути `app/build/outputs/apk/debug/app-debug.apk`.
