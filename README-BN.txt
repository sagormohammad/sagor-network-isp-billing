SAGOR NETWORK ISP BILLING — Android App Project

আপনার দেওয়া billing HTML/design অপরিবর্তিত রাখা হয়েছে। Android WebView project-এর মধ্যে app চালানোর ব্যবস্থা আছে।

নতুন Google Drive backup/restore:
1. Billing app-এর Admin login করে Cloud Database Sync অংশে যান।
2. “Download Full Backup” চাপুন। তৈরি হওয়া JSON file Google Drive-এ upload করুন।
3. অন্য ফোনে Drive থেকে JSON file download করুন। app-এর একই অংশে “Google Drive থেকে backup file বাছাই করুন” দিয়ে file নির্বাচন করে “Restore Backup” চাপুন।
4. Restore করলে ওই ফোনের বর্তমান data backup file দিয়ে replace হবে। তাই আগে backup নিন।
5. এটি manual backup/restore; নিজে নিজে live sync নয়। একাধিক ফোনে automatic sync-এর জন্য Cloud Sync-এর সঠিক database URL ও access rules আলাদাভাবে সেট করতে হবে। Default URL কাজ করছে বলে ধরে নেবেন না।

APK status:
এই ZIP-টি Android Studio project, APK নয়। এই পরিবেশে Android SDK/Gradle build tools নেই, তাই installable APK compile করা যায়নি। APK বানাতে Android Studio-তে project খুলে Gradle Sync, তারপর Build > Build APK(s) করতে হবে।

সতর্কতা:
প্রথমে পরীক্ষামূলক data দিয়ে পরীক্ষা করুন। বাস্তব customer data দেওয়ার আগে cloud access/security rules নিশ্চিত করুন। MikroTik router control-এর জন্য আলাদা secure connector/server প্রয়োজন হতে পারে।
