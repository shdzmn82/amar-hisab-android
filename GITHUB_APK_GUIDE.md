# GitHub দিয়ে APK তৈরির নিয়ম

## ১. নতুন repository তৈরি

1. GitHub-এ লগইন করুন।
2. **New repository** চাপুন।
3. Repository name লিখুন: `amar-hisab-android`
4. **Private** নির্বাচন করতে পারেন।
5. README বা অন্য কোনো ফাইল যোগ না করে **Create repository** চাপুন।

## ২. প্রকল্পের ফাইল আপলোড

1. এই ZIP ফাইলটি কম্পিউটারে Extract করুন।
2. Extract করা `AmarHisab` ফোল্ডারের ভেতরের সব ফাইল নির্বাচন করুন।
3. GitHub repository-তে **Add file > Upload files** চাপুন।
4. ফাইলগুলো upload box-এ টেনে দিন। `.github` ফোল্ডারটিও অবশ্যই থাকতে হবে।
5. নিচে **Commit changes** চাপুন।

> সতর্কতা: repository-র প্রথম স্তরেই `app`, `.github`, `build.gradle.kts` এবং
> `settings.gradle.kts` থাকতে হবে। শুধু `AmarHisab` নামে আরেকটি বাইরের ফোল্ডারের
> নিচে রাখলে workflow সঠিক জায়গায় project খুঁজে পাবে না।

## ৩. APK Build চালু করা

Main branch-এ upload/commit হলে build স্বয়ংক্রিয়ভাবে শুরু হবে। না হলে:

1. Repository-র **Actions** tab খুলুন।
2. বাম পাশে **Build Android APK** নির্বাচন করুন।
3. **Run workflow > Run workflow** চাপুন।
4. Build শেষ হওয়া পর্যন্ত অপেক্ষা করুন। সবুজ টিক চিহ্ন সফল build বোঝায়।

## ৪. APK Download

1. সফল workflow run খুলুন।
2. পেজের নিচে **Artifacts** অংশে যান।
3. **AmarHisab-debug-apk** চাপুন।
4. ZIP download হবে; Extract করলে `app-debug.apk` পাওয়া যাবে।
5. APK ফোনে নিয়ে গিয়ে install করুন। প্রয়োজনে ফোনের **Install unknown apps** অনুমতি দিন।

## Build ব্যর্থ হলে

ব্যর্থ workflow run খুলে লাল চিহ্নযুক্ত **Build debug APK** ধাপের screenshot বা
error text দিন। সেই error অনুযায়ী source ঠিক করা হবে।
