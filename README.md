# ELENORA – Android app (Capacitor)

Az app forrása az `index.html`. A GitHub Actions ebből építi az Android APK-t.

## APK megszerzése (nincs szükség helyi telepítésre)

1. Készíts ingyenes fiókot a github.com-on, majd hozz létre egy új **privát** repót (pl. `elenora`).
2. A repo oldalán: **Add file → Upload files**, és húzd be a mappa **teljes tartalmát**
   (`index.html`, `package.json`, `capacitor.config.json`, `.gitignore`, `README.md`
   és a **`.github`** mappa – a rejtett mappát is!). Commit.
3. Nyisd meg az **Actions** fület → „Android APK” → várd meg a zöld pipát (kb. 5–8 perc).
   Ha nem indult el: *Run workflow*.
4. A lefutott futásnál lent az **Artifacts → elenora-apk** letölthető (zip-ben az `app-debug.apk`).
5. Másold a telefonra, nyisd meg, engedélyezd az ismeretlen forrásból telepítést, és telepítsd.

## Első indítás után
- Engedélyezd az értesítéseket.
- Android 12+ rendszeren az ébresztő mentésekor felugró ablakban kapcsold be a **„Ébresztők és emlékeztetők”** engedélyt.
- Gyártói akkumulátor-spórolók (Xiaomi, Samsung, Huawei…) néha késleltetik az ébresztőt: állítsd az Elenora akkumulátor-használatát „Nincs korlátozás”-ra.

## Frissítés
Az `index.html` módosítása után töltsd fel újra a repóba – az Actions újra elkészíti az APK-t.
