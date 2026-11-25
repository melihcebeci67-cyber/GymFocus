EVOLUTION HOME GYM V3 — Android-ready Capacitor project source
============================================================

What is included:
- Mobile-first workout app UI
- A procedural 3D mannequin drawn with Three.js primitives and movement demo templates
- HIIT, cardio, band and core exercise library
- Workout timers, movement navigation, set completion
- Synth beat demo
- Measurement tracking, trend chart, profile, weekly template and heuristic adaptation
- Capacitor Android project configuration and Vite build setup

This ZIP is an Android-ready source project, not a precompiled APK. This environment did not have the Android SDK/Gradle Android build setup available to compile an APK.

Build APK on a computer:
1. Install Node.js LTS and Android Studio, including Android SDK and platform tools.
2. Extract the ZIP, open a terminal in this project directory.
3. Run: npm install
4. Run: npm run build
5. Run: npx cap add android
6. Run: npx cap sync android
7. Run: npx cap open android
8. In Android Studio, allow Gradle sync. Build > Build APK(s).
   For command-line build after Android platform project generated: cd android && ./gradlew assembleDebug
9. APK normally appears at android/app/build/outputs/apk/debug/app-debug.apk

Android Studio can also generate a signed APK from Build > Generate Signed Bundle / APK.

Privacy note:
- User-entered data is stored locally via browser localStorage in this prototype.
- No cloud account, sync, or remote AI personalization.
- Program adaptation is heuristic and should not be treated as medical advice.
- Stop exercising if you experience pain, dizziness or unusual symptoms.
- Three.js module imports use a CDN, so an internet connection is required at runtime for the 3D module in this version.

Exercise animation note:
- Procedural avatar animation templates are demonstration motions, not medically validated instructional biomechanics. For a professional commercial app, each movement should be reviewed and replaced/validated with carefully authored animation clips.
