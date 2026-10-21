# 3D YouTube Automation — Android Starter

यह Android Studio प्रोजेक्ट WebView के अंदर मोबाइल-फ्रेंडली हिंदी डैशबोर्ड चलाता है।

## अभी क्या काम करता है
- Android ऐप के रूप में खुलता है
- Topic input, भाषा/स्टाइल चयन, quick topic buttons
- Create Video दबाने पर demo project status दिखाता है
- responsive dashboard और automation workflow UI

## अभी क्या नहीं जुड़ा
AI से वास्तविक script/image/video/voice generation, final MP4 rendering और YouTube upload अभी सक्रिय नहीं हैं। इनके लिए provider APIs, secure backend, credentials, quota/billing और YouTube OAuth consent setup चाहिए। API keys को APK में hardcode न करें।

## Android APK बनाना (कंप्यूटर के बिना GitHub Actions)
1. GitHub पर नया repository बनाएं।
2. इस ZIP की सभी फाइलें repository में upload करें और `main` branch में commit करें।
3. GitHub repository में **Actions** खोलें।
4. **Build Android APK** workflow चुनें और **Run workflow** दबाएं।
5. Workflow सफल होने पर नीचे **Artifacts** में `3DYouTubeAutomation-debug-apk` डाउनलोड करें।
6. ZIP को Android मोबाइल में खोलें, `app-debug.apk` निकालें और install करें। Android पूछे तो इस स्रोत से install की अनुमति दें।

## लोकल बिल्ड
Android SDK और JDK 17 के साथ `gradle assembleDebug` चलाएं।
