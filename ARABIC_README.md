# Arabic localization patch (experimental)

Target source: Mindustry build 160.7 source snapshot.

Changes:
- Added `core/assets/bundles/bundle_ar.properties` with Arabic UI labels and selected item/block/unit names; untranslated entries intentionally retain English as fallback.
- Added Arabic locale to `core/assets/locales`.
- Added Noto Kufi Arabic font asset and a font override for Arabic locale.

Important limitations:
- Arabic text shaping and right-to-left layout are not implemented by this patch; depending on the UI component, Arabic may render disconnected or in an unexpected order.
- This is a partial translation, not a complete Arabic translation of every description and item.
- APK build was not completed in this environment because the Gradle wrapper distribution is not cached and external network access to services.gradle.org is unavailable. Build on a machine with network access/Gradle dependencies installed using `./gradlew :android:assembleRelease`.
