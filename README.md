# English Academy Business — Unified Offline-First Android Project

All three planned feature groups are available from one **Explore** hub. No learning-level prerequisites or phase locks. Existing lesson and progress data use the same localStorage key as the original app.

## Implemented in this update
- Original A1–C2 lesson content, practice, offline progress, word popup, starter Arabic glossary, saved vocabulary and flashcards
- Unified feature navigation with direct access to all modules
- Offline email templates and simple rule-based structural checks (not AI editing)
- Optional four-question diagnostic (not validated CEFR assessment)
- Offline business listening using device TTS and bundled dialogues
- Starter industry phrase collections
- Local completion record for finished lessons (not an accredited certificate)
- Speaking scripts and offline TTS model answer (no automatic scoring)
- Locally stored daily study plan
- Local-only corporate learning snapshot
- Subscription and online AI feature information screens

## Not yet implemented / needs external services
- Live AI email corrections and AI speaking partner, automated speech assessment
- Real payments, subscription entitlement validation
- Multi-user corporate accounts, centralized reporting and synchronization
- Full Arabic dictionary, full-length listening courses, accredited certificates

These cannot be described as working features until backend services, APIs, account management, billing and device tests are completed. Core learning works offline; online modules explicitly explain their current status.

## Build
Upload all extracted files to your GitHub repository, retaining `.github/workflows/build-apk.yml`, then run **Build offline Android APK** in Actions. Download the build artifact and extract `app-debug.apk`. Debug APK is for testing, not Play Store release.

Android TTS requires an installed English voice. The app requests INTERNET permission for future online integrations, but makes no API calls and has no configured server in this build.
