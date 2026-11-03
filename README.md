# پروژه آمار: خواب، دور کمر و علائم افسردگی

داده‌ها: NHANES اوت ۲۰۲۱ تا اوت ۲۰۲۳، مسیر الف.

## فایل‌ها

```text
PROJECT_CARD.md
README.md
requirements.txt
data/
    README.md
    raw/                 داده خام محلی، خارج از تحویل
src/
    run_phase1.py
notebooks/
    phase1.ipynb         کد، گزارش فارسی و خروجی‌های فاز اول
figures/                 نمودارهای تولیدشده با کد
reports/
    phase1.pdf           خروجی موردنیاز؛ هنوز ساخته نشده
    phase1/
    phase2/
    phase3/
    phase4/
    final/
```


## اجرا در PowerShell

از ریشه پروژه:

```powershell
python -m venv .venv
.venv\Scripts\python.exe -m pip install -r requirements.txt
.venv\Scripts\python.exe -m jupyter lab
```

فایل notebooks/phase1.ipynb را باز و همه سلول‌ها را به ترتیب اجرا کنید. مسیرها از داخل پوشه پروژه شناسایی می‌شوند. داده‌های لازم و روش دریافت آن‌ها در [data/README.md](data/README.md) آمده است.

اجرای کامل و ذخیره خروجی‌های نوت‌بوک از خط فرمان:

```powershell
.venv\Scripts\python.exe src/run_phase1.py
```

نمودارها دوباره در figures ساخته می‌شوند. داده تحلیلی در متغیر final_df داخل نوت‌بوک ساخته می‌شود؛ به فایل داده پاک‌شده از پیش آماده نیاز نیست.

## وضعیت فاز اول

کد و خروجی‌های توصیفی در نوت‌بوک موجودند. سوال آماری در بخش ۱۰ نهایی شده و PROJECT_CARD.md با آن هماهنگ است. ساخت و بررسی reports/phase1.pdf هنوز باقی مانده است.

طبق صورت پروژه، فایل PDF، کارت پروژه، کد قابل بازتولید و README به‌روز باید تحویل داده شوند. پس از تکمیل فاز و ثبت تغییرات در Git، برچسب phase-1 نیز لازم است. در پوشه فعلی مخزن Git راه‌اندازی نشده است.

پوشه‌های .venv، data/raw و فایل‌های خام XPT را در ZIP تحویل قرار ندهید. فایل‌های خام با .gitignore نیز از Git کنار گذاشته شده‌اند.
