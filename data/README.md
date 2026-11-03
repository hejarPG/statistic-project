# داده‌های پروژه

## منبع

CDC / NCHS، پیمایش NHANES اوت ۲۰۲۱ تا اوت ۲۰۲۳.

[صفحه رسمی فایل‌های دوره](https://wwwn.cdc.gov/nchs/nhanes/search/datapage.aspx?Cycle=2021-2023)

| فایل | مستندات | دریافت |
|---|---|---|
| DEMO_L.xpt | [DEMO_L](https://wwwn.cdc.gov/Nchs/Data/Nhanes/Public/2021/DataFiles/DEMO_L.htm) | [XPT](https://wwwn.cdc.gov/Nchs/Data/Nhanes/Public/2021/DataFiles/DEMO_L.xpt) |
| SLQ_L.xpt | [SLQ_L](https://wwwn.cdc.gov/Nchs/Data/Nhanes/Public/2021/DataFiles/SLQ_L.htm) | [XPT](https://wwwn.cdc.gov/Nchs/Data/Nhanes/Public/2021/DataFiles/SLQ_L.xpt) |
| BMX_L.xpt | [BMX_L](https://wwwn.cdc.gov/Nchs/Data/Nhanes/Public/2021/DataFiles/BMX_L.htm) | [XPT](https://wwwn.cdc.gov/Nchs/Data/Nhanes/Public/2021/DataFiles/BMX_L.xpt) |
| DPQ_L.xpt | [DPQ_L](https://wwwn.cdc.gov/Nchs/Data/Nhanes/Public/2021/DataFiles/DPQ_L.htm) | [XPT](https://wwwn.cdc.gov/Nchs/Data/Nhanes/Public/2021/DataFiles/DPQ_L.xpt) |

تاریخ دریافت اولیه در فایل‌های موجود ثبت نشده و مشخص نیست. تاریخ اصلاح فایل به‌عنوان تاریخ دریافت فرض نشده است. هنگام دریافت دوباره، تاریخ واقعی دریافت را در این فایل ثبت کنید.

## بازسازی داده تحلیلی

۱. چهار فایل XPT را از منبع رسمی دریافت و بدون تغییر نام در data/raw قرار دهید.

۲. وابستگی‌های requirements.txt را نصب کنید.

۳. تمام سلول‌های notebooks/phase1.ipynb را از ابتدا اجرا کنید یا از src/run_phase1.py استفاده کنید.

۴. فایل‌ها با کلید SEQN و ادغام درونی یک‌به‌یک ترکیب می‌شوند. افراد ۲۰ سال و بالاتر انتخاب می‌شوند. کدهای ویژه و گمشدگی‌ها طبق بخش ۵ نوت‌بوک بررسی می‌شوند و PHQ-9 فقط با نه پاسخ معتبر ساخته می‌شود.

۵. نمونه کامل با خواب روزهای کاری، دور کمر، PHQ-9، جنسیت معتبر و وزن و طرح قابل استفاده در final_df ساخته می‌شود. تعداد حذف‌ها از داده محاسبه و در همان بخش گزارش می‌شود.

جدول‌ها و نمودارها در نوت‌بوک تولید می‌شوند. نمودارها در figures نیز ذخیره می‌شوند. فایل داده خام یا داده فردی پاک‌شده در Git یا ZIP تحویل قرار نمی‌گیرد.
