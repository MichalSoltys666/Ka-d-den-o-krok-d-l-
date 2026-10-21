# Každý den o krok dál - Nativní Android Aplikace (Kotlin & Jetpack Compose)

Tento projekt byl navržen a připraven pro Android Studio (Ladybug / Koala nebo novější).

## Použité technologie a knihovny:
- Jazyk: Kotlin 2.0.21
- UI: Jetpack Compose s Material 3 (Compose BOM 2024.11.00)
- Lokální databáze: AndroidX Room 2.6.1 (KSP kompilátor, reaktivní Flow)
- Nastavení aplikace: AndroidX DataStore Preferences 1.1.1
- Správa stavu: ViewModel & StateFlow (Lifecycle 2.8.7)
- Asynchronní operace: Kotlin Coroutines 1.9.0
- Navigace: Navigation Compose 2.8.4
- Minimální SDK: 26 (Android 8.0 Oreo), Cílové SDK: 35 (Android 15)

## Jak získat instalační APK bez počítače a bez Android Studia (v cloudu zdarma):
1. Vytvořte si nový bezplatný repozitář na **GitHub.com** (přímo z mobilního prohlížeče).
2. Nahrajte do něj obsah tohoto rozbaleného archivu (včetně složky `.github/workflows/`).
3. GitHub Actions automaticky spustí cloudové sestavení na linuxovém serveru s předinstalovaným JDK 17 a Android SDK.
4. Za 2 minuty v záložce **Actions -> Sestavit Android APK** stáhněte hotový artefakt `KazdyDenOKrokDal-debug-apk` obsahující instalační `app-debug.apk` přímo do svého telefonu!

## Jak projekt sestavit v Android Studiu na počítači:
1. Rozbalte tento archiv do složky na svém počítači.
2. Otevřete **Android Studio**.
3. Zvolte **File -> Open...** a vyberte rozbalenou složku projektu.
4. Počkejte na dokončení úvodní synchronizace Gradle (Gradle Sync).
5. Připojte fyzické zařízení s povoleným USB laděním nebo spusťte Android Emulator.
6. Klikněte na zelené tlačítko **Run 'app'** (Shift + F10).

## Jak vytvořit instalační APK soubor v Android Studiu:
1. V horním menu Android Studia zvolte:
   **Build -> Build Bundle(s) / APK(s) -> Build APK(s)**
2. Po dokončení kompilace klikněte v pravém dolním rohu na **locate** v oznámení.
3. Výsledné APK najdete ve složce:
   `app/build/outputs/apk/debug/app-debug.apk`
4. Tento APK soubor můžete přímo nainstalovat do jakéhokoliv telefonu se systémem Android.

## Ověření lokálního ukládání dat:
- V Android Studiu otevřete nástroj **App Inspection -> Database Inspector**.
- Uvidíte živou tabulku `daily_entries` a všechny záznamy.
- Aplikace je 100% offline a neobsahuje žádná síťová oprávnění v AndroidManifest.xml.
