# My AI Assistant (JARVIS-Style Android Personal AI)

A modern, native Android personal AI assistant built with Kotlin, Jetpack Compose, Material 3, and Firebase AI Logic / Gemini integration. It understands voice commands and natural language in Hindi, Hinglish, and English, executing real smartphone actions: floating screen assistant overlay over other apps, screen understanding with vision AI, opening apps, YouTube search, WhatsApp message drafting, voice synthesis (TTS), AI conversation, and progress tracking.

---

## 📱 How to Get the APK on Your Mobile Phone via GitHub

Even if you only have your Android mobile phone, you can build and download your APK directly through GitHub:

### Step 1: Open GitHub in your mobile browser or app
1. Go to your repository on [GitHub](https://github.com).
2. Tap the **Actions** tab near the top (if on mobile web, tap the navigation menu `...` to select **Actions**).

### Step 2: Run the Build Workflow
1. In the Actions list, tap **Build Android APK**.
2. Tap the **Run workflow** dropdown button, select branch `main` (or your current branch), and tap the green **Run workflow** button.
3. Wait approximately 2–4 minutes while GitHub Actions sets up Android SDK and compiles your APK. A green checkmark (`✓`) will appear when the build succeeds.

### Step 3: Download the APK Artifact
1. Tap on the completed workflow run.
2. Scroll down to the **Artifacts** section at the bottom of the summary page.
3. Tap on **my-ai-assistant-debug-apk** to download the ZIP file.
4. Extract the ZIP on your phone (using your phone's File Manager or Google Files) to reveal the `.apk` file.

### Step 4: Install the APK on Your Android Device
1. Tap on the `.apk` file in your File Manager.
2. If Android prompts you with a security warning stating **"Install unknown apps"**, tap **Settings** and allow your browser/file manager to install unknown apps.
3. Tap **Install** and then **Open**.

---

## 🚀 Features Included

### 1. 🌐 Floating Screen Assistant (Over Other Apps)
- **Movable Overlay Orb**: Drag the floating JARVIS icon anywhere on your screen while using other apps.
- **Compact HUD**: Tap the orb to expand a quick assistant window without closing your current app.
- **Voice & Text Interaction**: Speak or type commands in Hindi, Hinglish, or English directly from any screen.
- **No Background Recording**: Microphone activates strictly upon explicit user tap.

### 2. 👁️ Understand My Screen (Vision AI)
- **"Understand Screen" Action**: Tap the screen button or say *"JARVIS, screen par kya likha hai?"* or *"Is page ka summary batao"*.
- **MediaProjection Capture**: Captures a snapshot only upon explicit user consent to analyze layout, errors, or page content with Gemini Vision AI.
- **Privacy First**: Respects Android DRM and secure content flags; no private passwords or background screenshots stored.

### 3. ⛔ Emergency Stop & Action Safety
- Dedicated emergency stop button and voice command (*"Emergency stop"*, *"JARVIS ruko"*) halts all speech, voice listening, and pending actions immediately.
- Confirmation gate before sending WhatsApp messages or executing external phone actions.

### 4. 🎙️ Multilingual Voice & Speech Studio
- Real-time Speech-to-Text and Text-to-Speech in Hindi (`hi-IN`) and English (`en-IN`).
- Browse device TTS voices with pitch and speech speed sliders.

### 5. 📱 Phone Actions & App Launcher
- Launch apps: *"YouTube kholo"*, *"Chrome mein Google kholo"*, *"WhatsApp kholo"*, *"Camera kholo"*, *"Phone ki settings kholo"*.
- YouTube music search: *"YouTube par Arijit Singh ka gaana chalao"*.
- Installed apps discovery drawer.

### 6. 📊 "My Progress" Dashboard
- Transparent, verified completion dashboard tracking all 13 core features, device test statuses, limitations, and setup requirements.

---

## ℹ️ Publishing on Google Play Note
Publishing on the Google Play Store is a separate process that requires:
1. A Google Play Developer Console account ($25 one-time registration fee).
2. Creating an Android App Bundle (`.aab`) instead of an APK via `./gradlew bundleRelease`.
3. Signing the bundle with your private upload keystore.
4. Completing Google Play's Content Rating, Data Safety, Privacy Policy declarations, and Play Store listings.
