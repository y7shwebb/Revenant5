# Revenant 5

**Revenant 5** is an Android build configuration for the **GLUE 5** version of the GTA V WebAssembly (WASM) port. This repository allows you to compile and build the Android APK needed to run GTA V WASM locally and play multiplayer cross-platform with iOS players.

---

## 📌 Acknowledgments & Credits

* **Forked from:** [`almazblock`](https://github.com/almazblock) — Full credit goes to **almazblock** for the underlying work on the port.
* **Build Workflow:** I did **not** create the `build.yml` script. I am sharing this method publicly to make cross-platform multiplayer (Android & iOS) accessible to everyone who wants to run GLUE 5 on Android.

---

## ⚡ Important Notes & Requirements

* **GTA Online / Cross-Platform:** Designed specifically to enable playing GTA V WASM / GTA Online cross-platform with iOS players.
* **Performance:** This build currently lacks extensive graphics options and settings. **It is NOT recommended for low-end devices.** High-performance hardware is strongly recommended.
* **Game Files:** **NO GAME FILES OR PROPRIETARY ASSETS ARE PROVIDED IN THIS REPOSITORY.**

---

## 🛠️ Step-by-Step Setup Guide

### Part 1: Building the APK

1. **Fork this repository** to your GitHub account.
2. Prepare your own `game.wasm` file.
3. Create a **Draft Release** in your forked repository and attach your `game.wasm` file to it.
4. Go to the **Actions** tab in your GitHub repository.
5. Select the **`build.yml`** workflow and click **Run workflow**.
6. Select **Android** from the target options when prompted.
7. Once the build workflow finishes, navigate back to your **Draft Release** to download the compiled APK file.
8. Install the generated APK on your Android device.

---

### Part 2: Installing Game Files on Android

1. Obtain your official GTA V game assets.
2. Rename your main game asset folder to simply: `game`
3. Move the `game` folder to the following path on your Android storage:
   ```text
   Android/data/local.glue5/files/
   ```
   *(Full path structure: `Android/data/local.glue5/files/game/`)*

4. Open the game app on your Android device.
5. Navigate to **Settings** $\rightarrow$ **Game**.
6. Change the file source mode from **Server** to **Folder**.
7. Restart the app and launch!

---

## ⚖️ Legal Disclaimer

* This project is an open-source build helper intended strictly for personal research and educational purposes.
* No copyrighted Rockstar Games or Take-Two Interactive assets, binaries, or game data are included or distributed within this repository.
* Users must provide their own legally acquired copies of GTA V game files to use this software.