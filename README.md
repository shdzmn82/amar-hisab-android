# আমার হিসাব — Android App

বাংলা ভাষায় ব্যক্তিগত, স্কুল, কোচিং, ধার-পাওনা ও ব্যাংক হিসাব রাখার অফলাইন Android অ্যাপ।

## বর্তমান সংস্করণ (0.1.0)

- বাংলা Dashboard
- পাঁচটি প্রাথমিক হিসাবখাতা
- আয় ও ব্যয় এন্ট্রি
- Room offline database
- মোট আয়, ব্যয় ও বর্তমান ব্যালেন্স
- সাম্প্রতিক লেনদেন
- Android cloud backup configuration

## চালানোর নিয়ম

1. Android Studio-তে `AmarHisab` ফোল্ডারটি Open করুন।
2. Gradle Sync শেষ হতে দিন।
3. Android ফোনে USB debugging চালু করে Run চাপুন, অথবা Build > Build APK(s) ব্যবহার করুন।

ন্যূনতম Android 8.0 (API 26)।

GitHub দিয়ে APK তৈরির জন্য `GITHUB_APK_GUIDE.md` অনুসরণ করুন। প্রকল্পে প্রস্তুত
GitHub Actions workflow যুক্ত আছে।

## পরবর্তী সংস্করণ

- হিসাবখাতা নির্বাচন করে এন্ট্রি
- ফি ও শিক্ষার্থী ব্যবস্থাপনা
- ধার/পাওনা কিস্তি
- ব্যাংক হিসাব
- বাজেট ও ব্যয় সতর্কতা
- CSV/PDF রসিদ ও রিপোর্ট
- PIN/Fingerprint
- ব্যবহারকারী-নিয়ন্ত্রিত Google Drive backup/restore
