# طريقة استخراج APK

## الطريقة الأسهل باستخدام Android Studio
1. فك الضغط عن المشروع.
2. افتح مجلد `EmployeePayrollApp-v3-ReadyToBuild` في Android Studio.
3. انتظر حتى ينتهي Gradle Sync.
4. اختر:
   **Build > Build APK(s)**
5. ستجد الملف عادةً في:
   `app/build/outputs/apk/debug/app-debug.apk`
6. انقل APK إلى الهاتف وثبته.

## بناء APK بدون تثبيت Android Studio
يمكنك رفع المشروع إلى GitHub، ثم تشغيل:
**Actions > Build Android APK > Run workflow**

بعد انتهاء العملية:
**Actions > العملية الأخيرة > Artifacts > EmployeePayrollApp-debug-apk**

ثم حمّل ملف APK إلى الهاتف.

## ملاحظات الحساب
التطبيق يستخدم عدد أيام الشهر الميلادي الفعلي:
28/29/30/31.

أجر اليوم = الراتب الأساسي ÷ عدد أيام الشهر.

الحاضر: اليوم مستحق.
الغائب: يخصم أجر يوم.
نصف يوم: يخصم نصف أجر اليوم.
الإجازة المدفوعة: لا تخصم.

الأيام غير المسجلة لا تعتبر غياباً تلقائياً.
