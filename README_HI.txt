देश कर्तव्य मीडिया — मोबाइल न्यूज़ ऐप जैसा वेबसाइट पैकेज
====================================================

इस पैकेज में:
1. index.html          मुख्य मोबाइल-फ्रेंडली न्यूज़ ऐप
2. admin.html          खबर प्रकाशित/संपादित/हटाने का एडमिन पैनल
3. firebase-config.js  Firebase कनेक्शन सेटिंग
4. firestore.rules     डेटाबेस सुरक्षा नियम
5. manifest.json      ऐप इंस्टॉल करने की जानकारी
6. sw.js              बेसिक ऑफलाइन shell cache
7. icon.svg            ऐप आइकन

जरूरी स्पष्टता:
- यह एक installable PWA/वेबसाइट है, Google Play Store की APK फाइल नहीं।
- इसे HTTPS hosting (जैसे GitHub Pages) पर डालने के बाद Android Chrome में खोलें; मेन्यू ⋮ > Install app / Add to Home screen चुनें।
- Firebase config और Rules सेट किए बिना एडमिन से प्रकाशित खबरें सभी पाठकों को ऑनलाइन नहीं दिखेंगी।
- Firebase Rules में ADMIN_EMAIL_REPLACE_ME को अपने Firebase Authentication admin ईमेल से बदलना जरूरी है।
- Firebase Authentication में Email/Password sign-in चालू करें और admin user स्वयं बनाएं। सार्वजनिक signup न खोलें।
- Firebase की config values Firebase Console > Project settings > Your apps से लेकर firebase-config.js में भरें।
- Firestore database बनाएं और firestore.rules में दिए नियम Publish करें।
- PRGI नंबर CTMUL/25/A1797 को प्रकाशित करने से पहले मूल प्रमाणपत्र से सत्यापित करें।

GitHub Pages:
1. GitHub repository खोलें।
2. Add file > Upload files चुनें।
3. ZIP को मोबाइल में Extract करके इस पैकेज की सभी फाइलें repository के root में upload करें।
4. Commit changes दबाएं।
5. Repository > Settings > Pages > Deploy from a branch > main > /(root) > Save.
6. GitHub द्वारा दिखाया गया public URL खुलने में कुछ मिनट लग सकते हैं।

नोट: Firebase configuration और security rules सेट करने के बाद ही real online publishing इस्तेमाल करें। अपना password/OTP किसी से साझा न करें।
