<div dir="rtl" align='justify'>
  
# آزمایش ۹ - آشنایی با وقفه ها 
# ۹.۱ مقدمه
وقفه یک سیگنال به ریزپردازنده است که به توجه و پاسخ سریع پردازنده نیاز دارد. هنگامی که یک وقفه رخ می دهد، پردازنده عملیات جاری خود را متوقف می کند تا به درخواست وقفه رسیدگی کند. 
ریزپردازنده های خانواده ٨٠٨۶ به وقفه های تولید شده به وسیله سخت افزار و نرم افزار پاسخ می دهند که به ترتیب به آن‌ها وقفه های سخت افزاری، و وقفه های نرم افزاری گفته می شود. 

هدف این آزمایش آشنایی با انواع وقفه ها است. به عبارت دیگر اهداف این آزمایش عبارتند از:
1. آشنایی با وقفه ها و انواع آن ها 
2. .آشنایی با وقفه های نرم افزاری 
3. آشنایی با سطح دسترسی به وقفه ها 
4. آشنایی با نحوه عملکرد بدافزارهای سوء استفاده کننده از وقفه

# ۹.۲ پیش نیاز نظری 
در سیستم های عامل داده ساختارهای متفاوتی وجود دارد. یکی از این داده ساختارها جدول توصیفگر وقفه های سیستم است. 

در سیستم عامل می توان وقفه ها را به سه گروه کلی تقسیم کرد: 
1. .**وقفه های داخلی سخت افزاری:** وقفه های داخلی سخت افزاری به دلیل رخ دادن وضعیت معینی که در حین اجرای یک برنامه پیش آمده تولید می شوند (مانند تقسیم بر صفر). وقفه هایی که در اثر خطا بوجود می آید تله (trap) هم نامیده می شود. تله باعث سقط برنامه می شوند. این وقفه ها توسط سخت افزار اداره می شوند و امکان تغییر آنها وجود ندارد. اما با وجودی که نمی توان آنها را مستقیما مدیریت کرد، این امکان وجود دارد که از اثر آن روی کامپیوتر به نحو مفیدی استفاده شود. به عنوان مثال سخت افزار، وقفه شمارنده ساعت کامپیوتر را چند بار در ثانیه فراخوانی می کند، تا زمان را نگه دارد. می توان برنامه ای نوشت که مقدار شمارنده ساعت را خوانده، آن را به شکل قابل درک کاربر به صورت ساعت و دقیقه تبدیل کند. 
2. **وقفه های خارجی سخت افزاری:** وقفه های خارجی سخت افزاری خارج از پردازنده و توسط دستگاه های جانبی، مانند صفحه کلید، چاپگر، کارت های ارتباطی و یا کمک پردازنده تولید می شوند. دستگاه های جانبی با ارسال وقفه به پردازنده خواستار قطع اجرای برنامه فعلی شده و پردازنده را متوجه خود می کنند.
3. **وقفه های نرم افزاری:** وقفه های نرم افزاری در نتیجه دستورالعمل int در یک برنامه درحال اجرا تولید می شوند. برنامه نویس می تواند با دادن دستور int یک وقفه نرم افزاری تولید کند. بدین طریق بلافاصله اجرای برنامه فعلی را متوقف می کند و پردازنده را به روتین وقفه هدایت می کند. برنامه نویس از طریق وقفه ها می تواند در برنامه با وسایل جانبی ارتباط برقرار کند. استفاده از وقفه ها باعث کوتاهتر شدن کد برنامه و درک آسانتر و اجرای بهترآن می شود. 

# ۹.۳ آزمایش ۱ 
یک برنامه بنویسید که تمام وقفه های موجود در سیستم عامل لینوکس را نمایش دهد. 

انتظار می رود خروجی این آزمایش شامل موارد زیر باشد:

1. یک فایل اجرایی که همان کد پیاده سازی شده توسط دانشجو است
2. یک مستند که حاوی موارد زیر است: 
- (آ) توضیحاتی در خصوص تمام کدهای موجود در فایل اجرایی. 
- (ب) تصاویری از خروجی فایل اجرایی. 
- (ج) نیازمندی های لازم جهت اجرای فایل اجرایی.

  
  - [Watch Live Interrupts](https://www.linuxjournal.com/content/watch-live-interrupts)
  - [Introduction to interrupts](https://www.thegeekstuff.com/2014/01/linux-interrupts/)
  
# ۹.۴ آزمایش ۲ 
یک وقفه نرم افزاری به سیستم عامل لینوکس اضافه نمایید. آیا امکان فراخوانی این وقفه جدید توسط یک برنامه سطح کاربر وجود دارد؟ چرا؟ 

انتظار می رود خروجی این آزمایش شامل موارد زیر باشد: 

1. یک فایل اجرایی که همان کد پیاده سازی شده توسط دانشجو است. 
2. یک مستند که حاوی موارد زیر است. 
- (آ) توضیحاتی در خصوص تمام کدهای موجود در فایل اجرایی. 
- (ب) تصاویری از خروجی فایل اجرایی. 
- (ج) نیازمندی های لازم جهت اجرای فایل اجرایی. 
  
</div>

- [Software-interrupt](https://stackoverflow.com/questions/26025850/generate-and-handle-software-interupt)
- [Writing an interrupt handler](https://www.qnx.com/developers/docs/6.5.0SP1.update/com.qnx.doc.neutrino_prog/inthandler.html)
- [Handle Interrupt](https://pretagteam.com/question/generate-and-handle-software-interupt)


