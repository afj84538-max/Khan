BUILD THE ANDROID APK (Endocrine Qbank)

EASIEST: read GET_THE_APK_WITHOUT_ANDROID_STUDIO.txt (cloud build, nothing to install).
Or use Android Studio as below.

This folder is a ready Android Studio project. The whole Qbank is inside it
(app/src/main/assets/index.html), so the app works fully offline.

STEPS (about 10 minutes, free)
1. Install Android Studio from developer.android.com/studio.
2. File > Open > choose this folder (Android_APK_Project). Wait while it syncs
   (it downloads Gradle the first time; internet needed once).
3. To test: connect a phone with USB debugging, or start an emulator, and press Run.
4. To make the APK file: Build > Build Bundle(s) / APK(s) > Build APK(s).
   The file appears in app/build/outputs/apk/debug/app-debug.apk
   Send it to a phone and open it (allow "install unknown apps" if asked).
5. For Google Play or a shareable signed APK: Build > Generate Signed Bundle / APK,
   create a keystore, and keep that keystore file safe.

WHAT THE APP DOES
- Full screen, works offline, keeps each student's progress on the phone.
- Export buttons save files to the phone's Downloads folder.
- Import buttons open the phone's file picker.
- "Print / save as PDF" in the Mistake Notebook uses Android's print dialog.
- The Back button closes pop-ups first.

UPDATING THE QUESTIONS OR DESIGN
Replace app/src/main/assets/index.html with a newer Endocrine_Qbank.html
(rename it to index.html), raise versionCode in app/build.gradle, and rebuild.

NO ANDROID STUDIO? Host the Qbank_Phone_App folder on a web address and use
pwabuilder.com: enter the address and download the Android package.
