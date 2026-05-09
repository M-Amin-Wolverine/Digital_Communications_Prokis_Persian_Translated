
---
# فصل ۱: مقدمه

## 📖 معرفی فصل

در این کتاب، اصول بنیادینی را که زیربنای تحلیل و طراحی سیستم‌های مخابرات دیجیتال هستند، ارائه می‌دهیم. موضوع مخابرات دیجیتال شامل انتقال اطلاعات به شکل دیجیتال از منبعی که اطلاعات را تولید می‌کند به یک یا چند مقصد است. در تحلیل و طراحی سیستم‌های مخابراتی، مشخصات کانال‌های فیزیکی که اطلاعات از طریق آن‌ها منتقل می‌شوند، اهمیت ویژه‌ای دارند. مشخصات کانال عموماً بر طراحی بلوک‌های سازنده اصلی سیستم مخابراتی تأثیر می‌گذارند.

> 🔹 **کاربرد واقعی:** درک اولیه از اجزای یک سیستم مخابراتی (مثل گوشی همراه، مودم ADSL، یا لینک ماهواره‌ای)
> 🔗 **پیوند با فصول دیگر:** پایه‌ای برای تمام فصول بعدی — مدل‌های کانال در فصل ۴، نویز در فصل ۲، و کدگذاری در فصل ۷

---

## ۱.۱ اجزای یک سیستم مخابرات دیجیتال


![نمودار عملکردی و عناصر پایه یک سیستم مخابرات دیجیتال](data:image/png;base64,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)


.

**شکل ۱-۱-۱ نمودار عملکردی و عناصر پایه یک سیستم مخابرات دیجیتال را نشان می‌دهد.**
.**شکل ۱-۱-۱ نمودار عملکردی و عناصر پایه یک سیستم مخابرات دیجیتال را نشان می‌دهد.**

خروجی منبع ممکن است یا یک سیگنال آنالوگ، مانند سیگنال صوتی یا تصویری، و یا یک سیگنال دیجیتال، مانند خروجی یک کامپیوتر، باشد که در زمان گسسته بوده و تعداد متناهی کاراکتر خروجی دارد.

### ۱.۱.۱ کدگذاری منبع (Source Encoding)

در یک سیستم مخابرات دیجیتال، پیام‌های تولیدشده توسط منبع به دنباله‌ای از ارقام دودویی (باینری) تبدیل می‌شوند. در حالت ایده‌آل، مایلیم خروجی منبع (پیام) را با کمترین تعداد ارقام دودویی ممکن نمایش دهیم. به عبارت دیگر، ما به‌دنبال نمایشی کارا از خروجی منبع هستیم که حاصل آن افزونگی (redundancy) کم یا صفر باشد.

> 📌 **تعریف:** فرایند تبدیل کارای خروجی یک منبع آنالوگ یا دیجیتال به دنباله‌ای از ارقام دودویی، **کدگذاری منبع (source encoding)** یا **فشرده‌سازی داده (data compression)** نامیده می‌شود.

### ۱.۱.۲ کدگذاری کانال (Channel Encoding)

دنباله ارقام دودویی خروجی از کدگذار منبع، که آن را **دنباله اطلاعات** می‌نامیم، به کدگذار کانال (channel encoder) ارسال می‌شود. هدف کدگذار کانال این است که به شیوه‌ای کنترل‌شده، مقداری افزونگی در دنباله اطلاعات دودویی وارد کند که بتوان از آن در گیرنده برای غلبه بر اثرات نویز و تداخل ایجادشده در حین ارسال سیگنال از طریق کانال استفاده نمود.

> 💡 **نکته کلیدی:** افزونگی اضافه‌شده به افزایش قابلیت اطمینان داده‌های دریافتی کمک کرده و وفاداری سیگنال دریافتی را بهبود می‌بخشد.

**مثال ساده از کدگذاری کانال:** تکرار هر رقم دودویی به تعداد m بار که m عددی صحیح و مثبت است.

**کدگذاری‌های پیچیده‌تر:** شامل گرفتن k بیت اطلاعات در یک زمان و نگاشت هر دنباله k-بیتی به یک دنباله n-بیتی یکتا به نام **کلمه کد (codeword)**.

| مفهوم | تعریف |
|:------|:------|
| **میزان افزونگی** | نسبت n/k |
| **نرخ کد (code rate)** | k/n |

### ۱.۱.۳ مدولاتور دیجیتال (Digital Modulator)

دنباله دودویی در خروجی کدگذار کانال به مدولاتور دیجیتال ارسال می‌شود که به‌عنوان واسط با کانال مخابراتی عمل می‌کند. از آنجا که تقریباً تمام کانال‌های مخابراتی که در عمل با آن‌ها مواجه می‌شویم قادر به ارسال سیگنال‌های الکتریکی (شکل‌موج‌ها) هستند، هدف اصلی مدولاتور دیجیتال **نگاشت دنباله اطلاعات دودویی به شکل‌موج‌های سیگنال** است.

**مثال:** فرض کنید دنباله اطلاعات کدگذاری‌شده قرار است یک بیت در هر لحظه با نرخ یکنواخت R بیت بر ثانیه ارسال شود.

| نوع مدولاسیون | توضیح |
|:--------------|:------|
| **مدولاسیون دودویی (باینری)** | نگاشت رقم ۰ به s₀(t) و رقم ۱ به s₁(t) — هر بیت جداگانه ارسال می‌شود |
| **مدولاسیون M-تایی (M>2)** | گروه‌کردن b بیت با هم و استفاده از M=2ᵇ شکل‌موج مجزا |

### ۱.۱.۴ کانال مخابراتی (Communication Channel)

کانال مخابراتی، محیط فیزیکی است که برای ارسال سیگنال از فرستنده به گیرنده استفاده می‌شود.

| نوع کانال | مثال |
|:----------|:-----|
| **بی‌سیم** | اتمسفر (فضای آزاد) |
| **سیمی** | خطوط تلفن، کابل‌های مسی |
| **نوری** | کابل‌های فیبر نوری |
| **رادیویی** | مایکروویو |

**مکانیزم‌های تخریب سیگنال:**
- نویز گرمایی جمع‌شونده (تولیدشده توسط قطعات الکترونیکی)
- نویز ساخت بشر (مثلاً نویز جرقه‌زنی خودرو)
- نویز جوی (مثلاً تخلیه الکتریکی صاعقه در طوفان‌های تندری)

### ۱.۱.۵ دمودولاتور و دیکدر (Demodulator & Decoder)

در انتهای گیرنده:
- **دمودولاتور دیجیتال:** شکل‌موج ارسالیِ تخریب‌شده توسط کانال را پردازش کرده و شکل‌موج‌ها را به دنباله‌ای از اعداد که تخمینی از سمبل‌های داده ارسالی (دودویی یا M-تایی) هستند، تبدیل می‌کند.
- **دیکدر کانال:** تلاش می‌کند دنباله اطلاعات اصلی را با استفاده از دانش کد به‌کار رفته توسط کدگذار کانال و افزونگی موجود در داده‌های دریافتی، بازسازی کند.

### ۱.۱.۶ معیارهای عملکرد

| معیار | توضیح |
|:------|:------|
| **احتمال متوسط خطای بیت (BER)** | فراوانی رخداد خطا در دنباله دیکدشده |
| **اعوجاج (Distortion)** | تفاوت بین سیگنال اصلی و سیگنال بازسازی‌شده در خروجی دیکدر منبع |

احتمال خطا تابعی از:
- مشخصات کد
- انواع شکل‌موج‌های استفاده‌شده
- توان فرستنده
- مشخصات کانال (میزان نویز، ماهیت تداخل)
- روش دمودولاسیون و دیکدینگ

---

## 🔗 پیوند فصل ۱ با سایر فصول

```text
فصل ۱ (مقدمه)
    │
    ├──→ فصل ۲ (ریاضیات پایه) ← مدل‌سازی سیگنال و نویز
    │
    ├──→ فصل ۳ (مدولاسیون) ← بلوک مدولاتور
    │
    ├──→ فصل ۴ (گیرنده بهینه) ← بلوک دمودولاتور
    │
    ├──→ فصل ۶ (نظریه اطلاعات) ← کدگذاری منبع
    │
    ├──→ فصل ۷ و ۸ (کدگذاری کانال) ← بلوک کدگذار/دیکدر کانال
    │
    └──→ فصل ۱۳ و ۱۴ (محوشدگی) ← مدل‌سازی کانال.
```

---
💡 ایده‌های پایان‌نامه و طراحی محصول (بر اساس فصل ۱)
ایده‌های کارشناسی ارشد
M1-01: شبیه‌ساز آموزشی تعاملی اجزای یک سیستم مخابرات دیجیتال
فصول مرتبط: ۱، ۲، ۳، ۴

مسئله: دانشجویان در درک ارتباط بین بلوک‌های مختلف سیستم مخابراتی مشکل دارند

رویکرد: طراحی نرم‌افزار گرافیکی در MATLAB App Designer که تأثیر هر بلوک را به صورت زنده نشان دهد

خروجی: نرم‌آموزشی + مستندات

M1-02: مقایسه عملکرد کدگذاری‌های مختلف کانال در کانال‌های نویزی
فصول مرتبط: ۱، ۴، ۷، ۸

مسئله: انتخاب کد مناسب برای کاربردهای مختلف نیازمند تحلیل عملکرد است

رویکرد: شبیه‌سازی کدهای تکراری، بلوکی، کانولوشنال و LDPC در کانال AWGN

خروجی: جدول مقایسه + پیشنهاد برای کاربردهای مختلف (صوتی، تصویری، داده)

ایده‌های دکتری و طراحی محصول
P1-01: طراحی معماری نرم‌افزاری یک رادیو نرم‌افزاری (SDR) آموزشی
فصول مرتبط: ۱، ۳، ۴، ۵، ۱۱

مسئله: فقدان پلتفرم آموزشی منبع‌باز و کم‌هزینه برای تدریس مخابرات دیجیتال

رویکرد: پیاده‌سازی تمام بلوک‌های شکل ۱-۱-۱ روی یک پلتفرم SDR ارزان (مثل RTL-SDR + میکروکنترلر)

خروجی: سخت‌افزار + نرم‌افزار متن‌باز + محتوای آموزشی

P1-02: طراحی یک سیستم ارتباطی تطبیقی (Adaptive Communication System)
فصول مرتبط: ۱، ۴، ۵، ۱۰، ۱۳

مسئله: کانال‌های واقعی (مثل کانال سیار) دائماً در حال تغییر هستند

رویکرد: سیستمی که بر اساس تخمین نسبت سیگنال به نویز (SNR)، به طور خودکار:

نوع مدولاسیون (BPSK، QPSK، 16QAM، ...)

نرخ کد کانال (1/2، 2/3، 3/4، ...)
را تغییر دهد

خروجی: محصول نرم‌افزاری-سخت‌افزاری + الگوریتم تطبیق

P1-03: سیستم کدگذاری منبع-کانال توأم (Joint Source-Channel Coding) برای کاربردهای پزشکی از راه دور
فصول مرتبط: ۱، ۴، ۶، ۷، ۸

مسئله: در مخابرات پزشکی (مثل ارسال نوار قلب از راه دور)، قابلیت اطمینان بالا و تأخیر کم همزمان نیاز است

رویکرد: طراحی سیستمی که کدگذاری منبع (فشرده‌سازی) و کدگذاری کانال (تصحیح خطا) را به طور توأم و با توجه به مشخصات کانال بهینه‌سازی کند

خروجی: پایان‌نامه دکتری + پیاده‌سازی روی DSP

## 📱 مثال کاربردی: ارسال یک پیام صوتی (ویس)

فرض کن می‌خوای یه پیام صوتی (ویس) از خودت ضبط کنی و برای رفیقت بفرستی. کل این مسیر، همون سیستم مخابرات دیجیتاله. بیا ببینیم چه بلایی سر این ویس میاد:

---

### ۱. منبع اطلاعات (دهنت و گوشیت!)

تو حرف می‌زنی و یه سیگنال آنالوگ (صدا) تولید می‌شه. گوشی این صدا رو می‌گیره. مشکل اینجاست که این سیگنال خام خیلی پرحرفه. انگار یه بچه هی حرفای تکراری و بی‌ربط بزنه و اصل مطلب رو کش بده.

**کار سیستم (کدگذاری منبع):**
اینجا سیستم مثل یه خلاصه‌کننده حرفه‌ای عمل می‌کنه. میاد حرفای تکراری و بی‌خود رو حذف می‌کنه تا فایل ویس تا جای ممکن کم حجم بشه (فشرده‌سازی). مثلاً به جای اینکه ۱۰۰ بار بگه "سکوت"، می‌گه "۱۰۰ واحد سکوت". اینجوری حجم واقعی اطلاعات اصلی کم میشه، بدون اینکه اصل مطلب از دست بره. این کار رو **کدگذار منبع** انجام میده.

---

### ۲. محافظت از اطلاعات (کدگذاری کانال)

حالا یه فایل خلاصه و جمع‌وجور داری. می‌خوای اینو از طریق اینترنت (که پر از نویز و قطع و وصله) بفرستی. اگه همینجوری خام بفرستی، یه کم نویز میفته توش و نصف حرفات نامفهوم میشه.

**کار سیستم (کدگذار کانال):**
سیستم مثل یه جاساز ماهر عمل می‌کنه. یه سری اطلاعات اضافه و حساب‌شده (افزونگی) لای اطلاعات اصلی می‌ذاره. مثلاً برای هر کلمه مهم، یه مترادف یا توضیح کوچیک بغلش می‌ذاره.

- تو می‌گی: "ساعت ۵ بیا".
- سیستم می‌کنه: "ساعت (که همون تایم ۵ هستش) ۵ (پنج) بیا (حضور پیدا کن)".

اگه سر راه، کلمه "۵" خراب بشه، رفیقت از روی "پنج" و بقیه توضیحات می‌تونه حدس بزنه اصل مطلب چی بوده. این افزونگی هوشمندانه رو **کدگذار کانال** اضافه می‌کنه. مقدار این اطلاعات اضافه نسبت به کل، **"نرخ کد"** رو مشخص می‌کنه. نرخ کد پایین‌تر یعنی محافظت بیشتر ولی حجم بالاتر.

---

### ۳. سوار کردن روی موج (مدولاسیون دیجیتال)

اطلاعات محافظت‌شده‌ات الان یه مشت صفر و یکه. ولی اینترنت (کانال) فقط امواج الکترومغناطیسی (یا نوری تو فیبر) رو رد می‌کنه، نه صفر و یک رو.

**کار سیستم (مدولاتور):**
مدولاتور مثل یه خلبان می‌مونه. صفر و یک‌های تو رو سوار یه موج رادیویی (حامل) می‌کنه. خیلی ساده، قرارداد می‌کنه:
- هر وقت موج رو یه جور خاص بفرستم، یعنی "صفر".
- هر وقت جور دیگه‌ای بفرستم، یعنی "یک".

حالا ممکنه عجله داشته باشی و بخوای چندتا بیت رو یه‌جا سوار یه موج کنی. به این می‌گن **مدولاسیون M-تایی**. مثلاً با ۴ حالت مختلف موج، می‌تونی هم‌زمان دو بیت (۰۰, ۰۱, ۱۰, ۱۱) رو بفرستی. این کار سرعت رو می‌بره بالا، ولی موج رو در برابر نویز آسیب‌پذیرتر می‌کنه.

---

### ۴. جهنم کانال مخابراتی

موج سوار بر اطلاعات از گوشی تو خارج میشه و می‌ره تو کانال (هوا برای بی‌سیم، کابل برای وای‌فای، فیبر نوری...).

**اتفاق وحشتناک - هرچی بدبختیه سر این موج میاد:**

| نوع تخریب | توضیح |
|:----------|:------|
| **نویز گرمایی** | وسایل الکترونیکی خودشون یه هیس هیس زمینه‌ای تولید می‌کنن |
| **نویز ساخت بشر** | مایکروویو همسایه، موتور ماشین در حال عبور |
| **نویز جوی** | صاعقه و تخلیه‌های الکتریکی |
| **فیدینگ (محوشدگی)** | اگه تو خیابون راه بری، یهو سیگنال ضعیف و قوی میشه (بدترین نوع شکنجه برای سیگنال) |

خلاصه اینکه سیگنال تمیز و آراسته ما، حسابی لت و پار و گلی میشه می‌رسه دست رفیقت.

---

### ۵. نجات اطلاعات (دمودولاسیون و دیکدینگ)

گوشی رفیقت یه سیگنال زخمی تحویل می‌گیره.

**مرحله ۱: پیاده کردن (دمودولاتور)**
دمودولاتور مثل یه مأمور تخلیه بار عمل می‌کنه. با دقت به موج نگاه می‌کنه و سعی می‌کنه بفهمه فرستنده سعی داشته "صفر" بفرسته یا "یک". ولی از اونجایی که موج حسابی کتک خورده، ممکنه ته سیگنال رو اشتباه بگیره: یه "یک" رو "صفر" ببینه. اینجا یه سری اعداد به عنوان "حدس" از صفر و یک‌ها تولید میشه.

**مرحله ۲: ترمیم (دیکدر کانال)**
حالا نوبت حرکت طلایی جاسازیه! دیکدر کانال میاد و از همون ردپای افزونگی که فرستنده گذاشته بود استفاده می‌کنه. یه جاهایی که موج آسیب دیده و "یک" به "صفر" تبدیل شده رو با توجه به اطلاعات اضافی، مثل یه جدول کلمات متقاطع حل می‌کنه و خطاها رو می‌گیره. مثلاً:
- رسیده: "ساعت [خش‌خش] بیا".
- دیکدر با دیدن افزونگی و کدها می‌گه: آها! این [خش‌خش] که قبلش کلمه "ساعت" اومده و باهاش رمزگذاری شده، به احتمال ۹۹٪ همون "۵" بوده. تصحیحش می‌کنم.

به این میگن **احتمال خطای بیت (BER)** که چقدر دیکدر نتونه درست تشخیص بده. هدف کل این سیستم، صفر کردن این احتماله.

**مرحله ۳: بازگشایی (دیکدر منبع)**
حالا اطلاعات تمیز و دقیق شده. دیکدر منبع میاد اون فشرده‌سازی اولیه رو باز می‌کنه. "۱۰۰ واحد سکوت" رو دوباره به همون سکوت واقعی تبدیل می‌کنه تا ویس طبیعی بیاد بیرون.

---

### جمع‌بندی و تحلیل نهایی

هدف کل این غول مراحل، یه چیزه: **جابجایی سالم و کم‌حجم یک فکر از مغز تو به مغز رفیقت.**

| بلوک | وظیفه | هنر |
|:-----|:------|:----|
| **کدگذاری منبع** | کشتن افزونگی‌های بی‌خود | کارایی (کاهش حجم) |
| **کدگذاری کانال** | افزودن افزونگی هوشمند | قابلیت اطمینان (مقاومت به نویز) |
| **مدولاسیون** | وفق دادن اطلاعات با فیزیک | تبدیل بیت به موج |

**مهمترین معیار سنجش:** وقتی رفیقت صدای "ساعت ۵ بیا" رو مثل بلور بشنوه، یعنی **اعوجاج** کم بوده و احتمال خطای بیت پایین اومده. اگه بشنوه "ساعت ۳ شام" یعنی یه جای کار (مخصوصاً تو مرحله دیکدینگ یا تخمین فاز) حسابی لنگ زده.

> 💡 **نکته کلیدی:** این یه جنگ تمام‌عیار بین **حجم، سرعت، توان مصرفی، و دقت** است. هر چی پول بیشتری بدی (توان بیشتر، پهنای باند بیشتر)، سربازات (بیت‌ها) سالم‌تر می‌رسن. مهندس مخابرات، ژنرال این جنگه.

---

## 🏙️ مثال پیشرفته: سناریوی خیابان شلوغ

**سناریو:** تو خیابون شلوغی، موتور سیکلت گاز میده، داری میری و میخوای به رفیقت ویس بدی که "ساعت ۵ بازار".

### ۱. کدگذاری منبع - جلوی هدررفت حجم رو بگیر

گوشیت یه دیکتاتور بیرحمه. میبینه تو ۳ ثانیه سکوت کردی و گفتی "امممم... راستی... ساعت ۵.... بازار". میگه: 
- "سکوت" = کد ۰۱۰
- "اممم" = حذف
- "راستی" = کد ۱۰۱ (برای بازیابی)

کل اطلاعات واقعی "ساعت ۵ بازار" رو با مثلاً ۲ کیلوبیت میفرسته، نه ۲۰ کیلوبیت. این یعنی **نرخ فشرده‌سازی بالا**.

### ۲. کدگذاری کانال - زره تانک بپوشون

الگوریتم میگه: "خیابون شلوغه، نویز داریم". پس برای "ساعت ۵":
- "ساعت" رو میشکنه به قطعات کوچیک
- چندتا بیت اضافه میریزه لاش: "س-ا-ع-ت" + جمع‌آوری Parity (مثلاً اگه تعداد "س" ها فرد بود یه ۱ بذار)
- حتی ممکنه کل پیام رو با یه کد کانولوشنال یا توربو قاطی کنه. یعنی هر بیت اطلاعات، به ۲ یا ۳ بیت تبدیل میشه

**تحلیل تخصصی:** این کاری که میکنه، فدا کردن پهنای باند به ازای توان است. تو ممکنه ۶۴ کیلوبیت بر ثانیه پهنای باند بدی، اما اطلاعات واقعی‌ات ۸ کیلوبیته. چرا؟ چون اون ۵۶ کیلوبیت دژ محافظ دور اطلاعاتته. این کار `n/k` رو میبره بالا (نرخ کد میاد پایین).

> 🌌 **نکته جالب:** تو سیستم‌های فضایی (مثل ویجر)، نرخ کد ۱/۶ هم دیدیم! یعنی ۱ بیت اطلاعات رو با ۶ بیت میفرستن چون سیگنال رسیده به زمین از پشت پلوتو، از ته سیگنال وای‌فای خونه هم ضعیف‌تره.

### ۳. مدولاسیون - انتخاب اسلحه

تو شرایط سخت (نویز زیاد)، نمیای از ۲۵۶-QAM استفاده کنی که نقاط صورت فلکی چسبیدن به هم. میای از QPSK یا حتی BPSK استفاده میکنی.

**چرا؟** چون **فاصله اقلیدسی** بین نقاط تو BPSK زیاده. دوتا نقطه رو دو سر یه خط فرض کن. نویز باید خیلی قوی باشه که بتونه "یک" رو به "صفر" تبدیل کنه.

| مدولاسیون | مقاومت به نویز | سرعت |
|:----------|:-------------|:-----|
| BPSK | بالا | پایین |
| QPSK | متوسط | متوسط |
| 16QAM | پایین | بالا |
| 256QAM | خیلی پایین | خیلی بالا |

> ⚔️ **سه‌گانه مرگ:** ستاد فرماندهی مخابرات همیشه درگیر این سه‌گانه مرگه: **سرعت داده، توان مصرفی، و پهنای باند**.

### ۴. کانال - جهنم روی زمین

تو خیابون راه میری. سیگنال از تو گوشیت میپره بیرون، میخوره به شیشه برج، به ماشین، و با هزار تا فاز مختلف میرسه به دکل BTS. به این میگن **چندمسیره (Multipath)**.

**فاجعه چیه؟** یکی از اون کپی‌ها که از روی شیشه اومده، دیرتر میرسه و میفته روی **سمبل بعدی**. به این میگن **تداخل بین سمبلی (ISI)**. عملاً سمبل قبلی، سمبل جدید رو ترور میکنه.

### ۵. گیرنده - عملیات نجات با چاشنی خشونت

دمودولاتور سیگنال رو میگیره. قاطی پاتی شده. اینجا **اکوالایزر تطبیقی** وارد میشه. میگه: "من میدونم این کانال چه بلایی سر سیگنال من میاره". یه فیلتر معکوس میذاره که اثرات شیشه و ماشین رو خنثی کنه (همون داستان LMS و RLS تو فصل ۱۰).

بعدش میره سراغ دیکدر: سیگنال -۱ و +۱ رو داریم. ولی به خاطر اون نویز، یهو میبینیم رسیده ۰.۳- . دیکدر کانال (مثلاً Viterbi تو کدهای کانولوشنال) نمیگه "اها، ۰.۳-، پس قطعاً -۱ بوده". میگه: "بذار ببینم مسیر تریلیس چی میگه. با توجه به قانون کدگذاری، غیرممکنه که بعد از این دنباله، یه بیت دیگه بیاد. پس این احتمالاً -۱ بوده که نویز خورده".

به این میگن **دیکدینگ نرم (Soft Decoding)**. این بزرگترین برگ برنده سیستم‌های مدرنه.

---

## 🎯 نتیجه نهایی

ویس رفیقت رو میشنوه: "ساعت ۵ بازار". **اعوجاج صفر مطلق نیست.** ممکنه یه "ر" رو یه کم خش‌خش داشته باشه. ولی اون "۵" رو درست تشخیص داده. این یعنی سیستم جواب داده.

### آمار خیره‌کننده

کل این سیستم‌ها برای این طراحی شدن که **احتمال خطای بیت (BER)** رو از ۰.۵ (حدس تصادفی) برسونن به:

$$BER = 10^{-5} \quad \text{یا حتی} \quad 10^{-9}$$

یعنی از هر **۱۰ میلیارد بیت**، **یکی** اشتباه دربیاد. این معجزه ریاضیات و مهندسیه.

> 🌍 **تحسین برانگیز:** وقتی تو سنترال پارک نیویورک با موبایل داری با یکی تو تهران حرف میزنی، اون ویس از بین هزاران منبع تداخل، دکل، ماهواره، و کابل رد میشه و سالم میرسه. این یعنی **فتح فیزیک و ریاضیات**.


---## ۱.۲ کانال‌های مخابراتی و مشخصات آن‌ها

همان‌طور که در بحث قبلی اشاره شد، کانال مخابراتی ارتباط بین فرستنده و گیرنده را فراهم می‌کند. کانال فیزیکی ممکن است یک جفت سیم باشد که سیگنال الکتریکی را حمل می‌کنند، یا یک فیبر نوری که اطلاعات را روی یک باریکه نور مدوله‌شده حمل می‌کند، یا یک کانال زیرآبی اقیانوسی که در آن اطلاعات به‌صورت صوتی ارسال می‌شود، یا فضای آزاد که سیگنال حامل اطلاعات با استفاده از یک آنتن در آن تابانده می‌شود. سایر رسانه‌هایی که می‌توان آن‌ها را به‌عنوان کانال‌های مخابراتی توصیف کرد، رسانه‌های ذخیره‌سازی داده، مانند نوار مغناطیسی، دیسک‌های مغناطیسی و دیسک‌های نوری هستند.

### انواع تخریب سیگنال در کانال

یکی از مشکلات رایج در ارسال سیگنال از طریق هر کانالی، **نویز جمع‌شونده** است. به‌طور کلی، نویز جمع‌شونده به‌صورت داخلی توسط قطعاتی مانند مقاومت‌ها و ادوات نیمه‌هادی که برای پیاده‌سازی سیستم مخابراتی استفاده می‌شوند، تولید می‌شود. این نویز گاهی **نویز گرمایی** نامیده می‌شود.

سایر منابع نویز و تداخل ممکن است به‌صورت خارجی برای سیستم به وجود آیند، مانند تداخل ناشی از سایر کاربران کانال. وقتی چنین نویز و تداخلی همان باند فرکانسی سیگنال مطلوب را اشغال کنند، می‌توان اثر آن‌ها را با طراحی مناسب سیگنال ارسالی و دمودولاتور آن در گیرنده به حداقل رساند.

انواع دیگر تخریب سیگنال که ممکن است در ارسال از طریق کانال با آن‌ها مواجه شویم:
- **تضعیف سیگنال (Attenuation)**
- **اعوجاج دامنه و فاز (Amplitude & Phase Distortion)**
- **اعوجاج چندمسیره (Multipath Distortion)**

### محدودیت‌های اساسی کانال

اثرات نویز را می‌توان با افزایش توان سیگنال ارسالی به حداقل رساند. با این حال، تجهیزات و سایر محدودیت‌های عملی، سطح توان سیگنال ارسالی را محدود می‌کنند. محدودیت اساسی دیگر، **پهنای باند کانال** در دسترس است.

> 💡 **نکته کلیدی:** این دو محدودیت (توان و پهنای باند)، مقدار داده‌ای را که می‌توان به‌طور قابل اطمینان روی هر کانال مخابراتی ارسال کرد، محدود می‌سازند. (قضیه شانون در فصل ۶)

---

## 📡 انواع کانال‌های مخابراتی

### ۱. کانال‌های باسیم (Wired Channels)

شبکه تلفن به‌طور گسترده از خطوط سیمی برای ارسال سیگنال صوتی و همچنین ارسال داده و تصویر استفاده می‌کند.

| نوع کانال | پهنای باند | کاربرد |
|:----------|:-----------|:--------|
| **سیم تلفن (زوج به‌هم‌تابیده)** | چندصد کیلوهرتز | اتصال مشتری به مرکز تلفن |
| **کابل هم‌محور (Coaxial)** | چند مگاهرتز | تلویزیون کابلی، اینترنت |
| **فیبر نوری** | چندین گیگاهرتز | مخابرات داخلی و بین قاره‌ای |

**مشکلات کانال‌های باسیم:**
- اعوجاج دامنه و فاز
- نویز جمع‌شونده
- تداخل هم‌شنوایی (Cross-talk) از کانال‌های مجاور

> 🔗 **پیوند با فصول دیگر:** روش‌های طراحی سیگنال بهینه و دمودولاسیون در **فصل ۹**، و یکسان‌سازهای کانال برای جبران اعوجاج در **فصل ۱۰** بررسی می‌شوند.

---

### ۲. کانال‌های فیبر نوری (Fiber Optic Channels)

فیبرهای نوری پهنای باند کانالی را در اختیار طراح سیستم مخابراتی قرار می‌دهند که چندین مرتبه بزرگی بزرگ‌تر از کانال‌های کابل هم‌محور است.

**اجزای سیستم فیبر نوری:**
- **فرستنده (مدولاتور):** منبع نوری (LED یا لیزر) که با سیگنال پیام مدوله می‌شود
- **رسانه:** فیبر نوری
- **گیرنده:** فوتودیود که شدت نور را به سیگنال الکتریکی تبدیل می‌کند

**منابع نویز:** فوتودیودها و تقویت‌کننده‌های الکترونیکی

> 📈 **پیشرفت:** طی دو دهه گذشته، کابل‌های فیبر نوری با تضعیف سیگنال نسبتاً کم و ادوات فوتونیکی بسیار قابل اطمینان ساخته شده‌اند.

---

### ۳. کانال‌های الکترومغناطیسی بی‌سیم (Wireless Electromagnetic Channels)

در سیستم‌های مخابراتی بی‌سیم، انرژی الکترومغناطیسی توسط آنتنی که به‌عنوان تشعشع‌کننده عمل می‌کند، به محیط انتشار کوپل می‌شود.

> 📐 **نکته فنی:** برای به‌دست آوردن تشعشع کارای انرژی الکترومغناطیسی، آنتن باید بلندتر از یک‌دهم طول موج باشد. مثال: در فرکانس 1 MHz (طول موج 300 متر)، به آنتنی حداقل 30 متری نیاز داریم.

#### باندهای فرکانسی و مدهای انتشار

| مد انتشار | محدوده فرکانسی | ویژگی |
|:----------|:---------------|:-------|
| **موج زمینی (Ground Wave)** | MF (0.3-3 MHz) | برد ~150 کیلومتر، استفاده در پخش AM |
| **موج آسمانی (Sky Wave)** | HF (3-30 MHz) | بازتاب از یونوسفر، برد قاره‌ای |
| **خط‌دید (LOS)** | VHF به بالا | نیاز به دید مستقیم، برد محدود |

**نویز در باند MF:**
- نویز جوی (طوفان‌های تندری)
- نویز ساخت بشر
- نویز گرمایی قطعات

> 🌙 **نکته جالب:** در طول شب، جذب فرکانس در لایه‌های پایینی یونوسفر کاهش می‌یابد و ایستگاه‌های پرقدرت AM می‌توانند در فواصل بسیار دور (قاره‌ای) دریافت شوند.

---

## 🚢 مثال کاربردی پیشرفته: فرستادن پیام حیاتی از زیردریایی به مرکز فرماندهی

> **سناریو:** زیردریایی نظامی در عمق ۳۰۰ متری اقیانوس آرام باید پیام رمزنگاری‌شده **"موقعیت دشمن: ۴۵ درجه شمالی، ۶۰ درجه غربی"** را به مرکز فرماندهی در واشنگتن بفرستد.

این سناریو ترکیبی از چندین نوع کانال است:
- کانال آکوستیک زیرآب
- کانال رادیویی از سطح به ماهواره
- کانال ماهواره به زمین
- کانال فیبر نوری روی خشکی

---

### مرحله صفر: تولید پیام (منبع اطلاعات)

فرمانده می‌گوید: "موقعیت... دشمن... ۴۵ درجه شمالی... ۶۰ درجه غربی..."

**کدگذاری منبع - فشرده‌سازی (فصل ۶):**

| عبارت | کد اختصاصی |
|:------|:-----------|
| "موقعیت" | ۱۰۱ |
| "دشمن" | ۰۱۱ |
| "۴۵" | ۱۰۰۱ |
| "شمالی" | ۱۱۰ |
| "۶۰" | ۱۰۱۰ |
| "غربی" | ۱۱۱ |

- حجم داده خام: ~۵۰۰ بیت
- حجم فشرده‌شده: ~۱۰۰ بیت
- **نرخ فشرده‌سازی: ۵:۱**

> 🔗 **مبحث مرتبط:** فصل ۶.۳ - کدگذاری بدون اتلاف منابع اطلاعات

---

### مرحله اول: محافظت جهنمی (کدگذاری کانال)

**چالش‌های کانال آکوستیک زیرآب:**
- نویز پس‌زمینه (صدای وال‌ها، میگوها)
- تضعیف شدید سیگنال
- پهنای باند محدود (چند کیلوهرتز)
- تغییر سرعت صوت با دما و شوری

**راه‌حل کدگذار کانال (فصل ۷ و ۸):**
استفاده از **کد توربو** یا **کد LDPC** با نرخ ۱/۳

- ۱۰۰ بیت اطلاعات → ۳۰۰ بیت کدگذاری‌شده
- ۲۰۰ بیت افزونگی هوشمند
- قابلیت بازیابی اطلاعات حتی با ۲۰٪ خرابی بیت‌ها

---

### مرحله دوم: سوار کردن روی موج صوتی (مدولاسیون آکوستیک)

**محدودیت:** آب امواج رادیویی را عبور نمی‌دهد ← استفاده از **صوت** در باند ۱-۵۰ کیلوهرتز

**انتخاب مدولاسیون (فصل ۳.۳):**
- **CPM (مدولاسیون فاز پیوسته)** یا **FSK**
- دلیل: در آب، فاز و فرکانس بهتر از دامنه حفظ می‌شوند
- **CPFSK:** فاز پیوسته → پهنای باند کمتر، تداخل کمتر

**مدولاسیون M-تایی با M=4 (هر سمبل = ۲ بیت):**

| بیت‌ها | فرکانس |
|:------:|:-------:|
| ۰۰ | 10 kHz |
| ۰۱ | 12 kHz |
| ۱۰ | 14 kHz |
| ۱۱ | 16 kHz |

- ۳۰۰ بیت → ۱۵۰ سمبل
- سرعت ارسال: ۱۰۰ سمبل در ثانیه
- **زمان ارسال: ۱.۵ ثانیه**

---

### مرحله سوم: جهنم کانال (اقیانوس آرام!)

#### ۱. تضعیف (Attenuation)
هر چه فرکانس بالاتر، آب بیشتر جذب می‌کند. فرکانس 16 kHz پس از 2 کیلومتر تقریباً محو می‌شود.

#### ۲. نویز جمع‌شونده (Additive Noise)

| منبع نویز | مشخصات |
|:----------|:--------|
| **میگوها (Snapping Shrimp)** | نویز ضربه‌ای با پهنای باند وسیع |
| **وال‌ها** | صداهای فرکانس پایین (20 Hz تا 2 kHz) |
| **کشتی‌های عبوری** | نویز پروانه و موتور |
| **تجهیزات الکترونیکی** | نویز گرمایی |

#### ۳. چندمسیره (Multipath) و ISI

صدا از کف اقیانوس، سطح آب و لایه‌های حرارتی منعکس می‌شود:
- یک سمبل → ۵-۶ کپی با تأخیرهای مختلف
- **نتیجه:** تداخل بین سمبلی (ISI) - سمبل قبلی روی سمبل جدید می‌افتد

> 🔗 **مبحث مرتبط:** فصل ۹ (کانال‌های محدود باند) و فصل ۱۳ (محوشدگی)

---

### مرحله چهارم: نجات در گیرنده (شناور روی سطح آب)

#### ۱. اکوالایزر تطبیقی (فصل ۱۰)
- جبران ISI و اعوجاج کانال
- استفاده از الگوریتم **LMS** برای تنظیم ضرایب فیلتر

#### ۲. دمودولاتور (فصل ۴)
استفاده از **بانک فیلتر منطبق (Matched Filter Bank)**:
- ۴ فیلتر، هر کدام حساس به یک فرکانس
- هر فیلتر با فرکانس مرجعش **کورولیشن** می‌کند

#### ۳. دیکدینگ کانال (فصل ۸)
- دیکدر توربو با **دیکدینگ تکراری**
- ورودی نرم (احتمالات) → خروجی سخت (بیت)
- مثال: "بیت سوم ۷۰٪ احتمال ۱ → با توجه به کد، ۹۹٪"

#### ۴. دیکدینگ منبع (فصل ۶)
بازسازی پیام اصلی از روی جداول فشرده‌سازی

---

## 📊 تحلیل نهایی سیستم

| مرحله | عملیات | فداکاری | دستاورد |
|:------|:-------|:--------|:--------|
| **کدینگ منبع** | حذف افزونگی بیهوده | هیچ | کاهش حجم ۵ برابر |
| **کدینگ کانال** | افزودن افزونگی هوشمند | افزایش حجم ۳ برابر | مقاومت در برابر خطا |
| **مدولاسیون CPM** | سوار شدن بر موج | توان و پهنای باند | امکان ارسال در آب |
| **اکوالایزر** | خنثی‌سازی ISI | پیچیدگی محاسباتی | دریافت تمیزتر |
| **دیکدینگ نرم** | حدس هوشمند احتمالاتی | تأخیر پردازشی | BER نزدیک به صفر |

---

## 🎯 سه‌گانه معروف مخابرات (Trade-off Triangle)

```text
              توان (Power)
                /\
               /  \
              /    \
             /      \
            /________\
    پهنای باند          پیچیدگی
    (Bandwidth)      (Complexity)

```    
---

💡 فلسفه کلیدی: کل این سیستم یک تریدآف سه‌گانه دارد بین توان، پهنای باند، و پیچیدگی.

اگر توان نامحدود داشتیم → BPSK ساده + توان بالا → نویز دفن می‌شود

اگر پهنای باند نامحدود داشتیم → سیگنال‌های متعامد + نرخ کد بالا

در دنیای واقعی: هیچ‌کدام نامحدود نیست → نیاز به مصالحه هوشمندانه → هنر مهندس مخابرات

کتاب Digital Communications پروکیس، کتاب مقدس همین مصالحه‌هاست.

---
### 📡 ادامه انتشار امواج الکترومغناطیسی و کانال‌های مختلف

**یک مشکل متداول** در انتشار امواج الکترومغناطیسی از طریق موج آسمانی در محدوده فرکانس بالا (HF)، پدیده **چندمسیره بودن سیگنال** است. چندمسیره بودن سیگنال زمانی رخ می‌دهد که سیگنال ارسالی از طریق چندین مسیر انتشار با تأخیرهای مختلف به گیرنده برسد. این پدیده عموماً منجر به **تداخل بین سمبلی (ISI)** در یک سیستم مخابرات دیجیتال می‌شود.

علاوه بر این، مؤلفه‌های سیگنال که از مسیرهای انتشار مختلف می‌رسند، ممکن است به‌طور تخریبی با یکدیگر جمع شوند و پدیده‌ای به نام **محوشدگی سیگنال (Fading)** را به وجود آورند؛ پدیده‌ای که بیشتر افراد هنگام گوش دادن به یک ایستگاه رادیویی دور در شب، زمانی که موج آسمانی مد غالب انتشار است، تجربه کرده‌اند. نویز جمع‌شونده در محدوده HF ترکیبی از نویز جوی و نویز گرمایی است.

---

### 🌐 انتشار در فرکانس‌های بالاتر

انتشار یونوسفری موج آسمانی در فرکانس‌های بالاتر از تقریباً ۳۰ مگاهرتز (انتهای باند HF) دیگر وجود ندارد. با این حال، امکان داشتن **انتشار پراکنشی یونوسفری (Ionospheric Scatter Propagation)** در فرکانس‌هایی در محدوده ۳۰ تا ۶۰ مگاهرتز وجود دارد که ناشی از پراکنش سیگنال از لایه‌های پایینی یونوسفر است.

همچنین می‌توان با استفاده از **پراکنش تروپوسفری (Tropospheric Scatter)** در فرکانس‌هایی در محدوده ۴۰ تا ۳۰۰ مگاهرتز، در فواصل چندصد مایلی مخابره برقرار کرد. پراکنش تروپوسفری ناشی از پراکنش سیگنال توسط ذرات موجود در اتمسفر در ارتفاعات ۱۰ مایل یا کمتر است.

> ⚠️ **نکته مهم:** به‌طور کلی، پراکنش یونوسفری و پراکنش تروپوسفری شامل تلفات انتشار سیگنال زیادی بوده و نیازمند توان فرستنده بالا و آنتن‌های نسبتاً بزرگ هستند.

---

### 🛰️ انتشار خط‌دید (Line-of-Sight)

فرکانس‌های بالاتر از ۳۰ مگاهرتز با تلفات نسبتاً کمی از یونوسفر عبور می‌کنند و مخابرات ماهواره‌ای و فرازمینی را ممکن می‌سازند. از این رو، در فرکانس‌های باند VHF و بالاتر، مد غالب انتشار الکترومغناطیسی، **انتشار خط‌دید (LOS)** است.

برای سیستم‌های مخابرات زمینی، این بدان معناست که آنتن‌های فرستنده و گیرنده باید در دید مستقیم با موانع نسبتاً کم یا بدون مانع قرار داشته باشند. به همین دلیل، ایستگاه‌های تلویزیونی که در باندهای VHF و UHF ارسال می‌کنند، آنتن‌های خود را روی برج‌های بلند نصب می‌کنند تا پوشش گسترده‌ای به دست آورند.

**محاسبه فاصله تا افق رادیویی:**

اگر آنتن فرستنده در ارتفاع \( h \) متری بالای سطح زمین نصب شده باشد، فاصله تا افق رادیویی، با فرض نبود موانع فیزیکی مانند کوه‌ها، تقریباً برابر با:

\[
d = \sqrt{15h} \quad \text{(کیلومتر)}
\]

> **مثال:** یک آنتن تلویزیونی نصب‌شده روی برجی به ارتفاع ۳۰۰ متر، پوششی تقریباً معادل \( d = \sqrt{15 \times 300} = \sqrt{4500} \approx 67 \) کیلومتر را فراهم می‌کند.

---

### ☔ اثرات جوی در فرکانس‌های بالا

در فرکانس‌های باند SHF بالای ۱۰ گیگاهرتز، شرایط جوی نقش عمده‌ای در انتشار سیگنال ایفا می‌کند.

| فرکانس | باران سبک | باران سنگین |
|:------:|:---------:|:-----------:|
| 10 GHz | 0.003 dB/km | 0.3 dB/km |
| 100 GHz | 0.1 dB/km | 6 dB/km |

> ⚠️ در فرکانس‌های بالا، باران سنگین می‌تواند تلفات انتشار بسیار بالایی ایجاد کند که منجر به **قطعی سرویس (Outage)** کامل سیستم مخابراتی شود.

---

### 🌌 کانال‌های آکوستیک زیرآب (Underwater Acoustic Channels)

طی چند دهه گذشته، فعالیت اکتشاف اقیانوس‌ها به‌طور پیوسته افزایش یافته است. همراه با این افزایش، نیاز به ارسال داده‌های جمع‌آوری‌شده توسط حسگرهای قرارگرفته در زیر آب به سطح اقیانوس وجود دارد.

#### چرا از امواج رادیویی زیر آب نمی‌توانیم استفاده کنیم؟

امواج الکترومغناطیسی در زیر آب، به جز در فرکانس‌های بی‌نهایت پایین، در فواصل طولانی منتشر نمی‌شوند. تضعیف امواج الکترومغناطیسی در آب را می‌توان بر حسب **عمق نفوذ پوستی (Skin Depth)** بیان کرد:

\[
\delta = \frac{250}{\sqrt{f}} \quad \text{(در آب دریا)}
\]

که در آن \( f \) بر حسب هرتز و \( \delta \) بر حسب متر است.

> **مثال:** در 10 کیلوهرتز، عمق نفوذ پوستی فقط \( \delta = 250 / \sqrt{10000} = 250 / 100 = 2.5 \) متر است!

#### مزیت کانال آکوستیک

در مقابل، سیگنال‌های آکوستیک در فواصلی به بزرگی ده‌ها و حتی صدها کیلومتر منتشر می‌شوند.

**مشخصات کانال آکوستیک زیرآب:**
- **کانال چندمسیره:** به دلیل بازتاب‌های سیگنال از سطح و بستر دریا
- **محوشدگی سیگنال:** به دلیل حرکت امواج و تأخیرهای انتشار متغیر با زمان
- **تضعیف وابسته به فرکانس:** تقریباً با مجذور فرکانس سیگنال متناسب است
- **سرعت صوت:** حدود 1500 متر بر ثانیه (متغیر با دما، شوری و عمق)

**نویز آکوستیک محیطی:**
- میگوها، ماهی‌ها و پستانداران دریایی
- نویز ساخت بشر در نزدیکی بنادر

---

### 💾 کانال‌های ذخیره‌سازی (Storage Channels)

سیستم‌های ذخیره‌سازی و بازیابی اطلاعات، بخش بسیار مهمی از فعالیت‌های روزمره مربوط به جابه‌جایی داده‌ها را تشکیل می‌دهند.

| رسانه ذخیره‌سازی | کاربرد |
|:----------------|:--------|
| نوار مغناطیسی | نوار صوت دیجیتال (DAT)، نوار ویدئو |
| دیسک‌های مغناطیسی | ذخیره‌سازی حجم عظیم داده‌های کامپیوتری |
| دیسک‌های نوری | دیسک‌های فشرده (CD)، DVD، Blu-ray |

> 💡 **آنالوج مخابراتی:** فرایند ذخیره‌سازی داده روی یک نوار یا دیسک، معادل ارسال یک سیگنال از طریق یک کانال است. فرایند بازخوانی نیز معادل عملکردهای گیرنده در یک سیستم مخابراتی است.

**چالش‌های کانال ذخیره‌سازی:**
- نویز جمع‌شونده از قطعات الکترونیکی
- تداخل ناشی از شیارهای مجاور (Inter-track Interference)
- محدودیت چگالی ذخیره‌سازی

> 📈 **پیشرفت:** چگالی بسته‌بندی \( 10^9 \) بیت در هر اینچ مربع در سیستم‌های ذخیره‌سازی دیسک مغناطیسی به نمایش گذاشته شده است!

---

## 🚀 سناریوی پیشرفته: "پیام نجات از قطب جنوب به مریخ"

> **داستان از این قراره:** یه تیم تحقیقاتی تو اعماق اقیانوس منجمد جنوبی، زیر یخ‌های قطبی، یه سیگنال عجیب فرازمینی کشف کردن. این سیگنال رو ضبط کردن و باید بفرستن به مرکز فضایی ناسا تو هوستون. از اونجا هم باید فوراً به مریخ‌نورد "پرسویرنس" که تو دهانه جیزرو مریخه برسه. یه پیام ۵۰۰ بیتی که سرنوشت بشریت بهش بستگی داره (!) باید از سه کانال کاملاً متفاوت عبور کنه.

---

### کانال اول: آکوستیک زیرآب (از زیردریایی به سطح)

**مشخصات فنی کانال:**
| پارامتر | مقدار |
|:--------|:------|
| نوع | آکوستیک زیرآب |
| فرکانس کاری | 15-25 kHz |
| پهنای باند | ~10 kHz |
| سرعت صوت | 1450 m/s (آب سرد قطبی) |
| عمق | 400 متر |
| دمای آب | -2°C |

**فجایع و راه‌حل‌ها:**

| فاجعه | توضیح | راه‌حل (منبع کتاب) |
|:------|:------|:-------------------|
| **تضعیف فرکانسی** | \( \delta = 250/\sqrt{f} \) ⇒ در 20 kHz فقط ~1.7m | استفاده از توان بالا + کدگذاری قوی |
| **چندمسیره جهنمی** | اختلاف مسیر 200m ⇒ تأخیر 138ms (13.8 برابر طول سمبل!) | اکوالایزر تطبیقی DFE (فصل 10.2) |
| **نویز محیطی** | صدای ترک خوردن یخ، نهنگ‌ها | فیلتر منطبق (فصل 4.2) |

**پارامترهای طراحی:**
- **کدگذاری:** توربو با نرخ 1/2 (فصل 8.9) → 500 بیت → 1000 بیت
- **مدولاسیون:** CPFSK با M=4 (فصل 3.3) → 500 سمبل
- **نرخ ارسال:** 100 سمبل/ثانیه → زمان ارسال: 5 ثانیه
- **BER هدف:** \( 10^{-3} \) قبل از دیکدینگ → \( 10^{-6} \) بعد از دیکدینگ

---

### کانال دوم: ماهواره‌ای (از شناور به ناسا)

**مشخصات فنی:**
| پارامتر | مقدار |
|:--------|:------|
| نوع | LOS + لینک ماهواره LEO |
| فرکانس | 8 GHz (باند X) |
| پهنای باند | 50 MHz |
| فاصله شناور-ماهواره | 800 km |
| فاصله ماهواره-ناسا | 13,200 km |

**محاسبه تضعیف فضای آزاد:**
\[
\lambda = \frac{c}{f} = \frac{3\times10^8}{8\times10^9} = 0.0375 \text{ m}
\]
\[
L_{\text{fs}} = \left(\frac{4\pi \times 800\times10^3}{0.0375}\right)^2 \approx 168 \text{ dB}
\]

**چالش‌های اضافی:**
- **اثر دوپلر:** ماهواره با سرعت 7.5 km/s ⇒ شیفت فرکانس ≈ 200 kHz
- **نویز کیهانی:** تابش پس‌زمینه در 2.7K

**پارامترهای طراحی:**
- **مدولاسیون:** QPSK (10 Msym/s → 20 Mbps)
- **کدگذاری:** LDPC با نرخ 3/4 (فصل 8.11)
- **دایورسیتی:** فضایی 2×2 (فصل 13.4)
- **هم‌سازی:** حلقه کاستاس (فصل 5.2)

**تحلیل بودجه لینک (فصل 4.10):**
| مؤلفه | مقدار (dB) |
|:------|:----------:|
| توان فرستنده (10W) | +40 |
| بهره آنتن فرستنده | +30 |
| تلفات مسیر | -168 |
| بهره آنتن گیرنده | +35 |
| نویز فیگر | -2 |
| پهنای باند (50 MHz = 77 dB-Hz) | -77 |
| **SNR دریافتی** | **~32 dB** |

⇒ BER < \( 10^{-12} \) (عملاً بدون خطا)

---

### کانال سوم: فضای عمیق (از ناسا به مریخ)

**مشخصات فنی:**
| پارامتر | مقدار |
|:--------|:------|
| فاصله زمین-مریخ | ~225 میلیون km |
| تأخیر نور | 225,000,000 / 300,000 = 750 ثانیه = 12.5 دقیقه! |
| فرکانس | 32 GHz (باند Ka) |
| پهنای باند | 10 MHz |
| توان فرستنده | 50 kW |

**محاسبه تضعیف:**
\[
\lambda = \frac{3\times10^8}{32\times10^9} = 0.009375 \text{ m}
\]
\[
L_{\text{fs}} = \left(\frac{4\pi \times 2.25\times10^{11}}{0.009375}\right)^2 \approx 290 \text{ dB!!!}
\]

> ⚠️ سیگنال \( 10^{29} \) برابر تضعیف می‌شود!

**راه‌حل مهندسی:**

**کدگذاری Concatenated (فصل 7.13):**
- کد بیرونی: Reed-Solomon (255,223)، نرخ 0.875
- کد درونی: کد کانولوشنال نرخ 1/2
- نرخ کلی: \( 0.875 \times 0.5 = 0.4375 \)
- 500 بیت → 1143 بیت کدگذاری‌شده

**مدولاسیون:** BPSK (ساده‌ترین، فاصله اقلیدسی بیشتر)

**نرخ ارسال:** 50 bps فقط! (زمان ارسال: 23 ثانیه برای 1143 بیت)

**تحلیل بودجه لینک (جزئیات فنی):**
| مؤلفه | مقدار (dB) |
|:------|:----------:|
| توان فرستنده (50 kW) | +77 dBm |
| بهره آنتن فرستنده (دیش 70m در 32 GHz) | +85 dBi |
| تلفات مسیر فضای آزاد | -290 dB |
| بهره آنتن گیرنده (دیش 2m) | +50 dBi |
| دمای نویز سیستم (30K) | +15 dB-K |
| k (ثابت بولتزمن) | -228.6 dBW/K/Hz |
| پهنای باند (10 MHz = 70 dB-Hz) | -70 dB |

**SNR خام محاسباتی:**
\[
77 + 85 - 290 + 50 - 15 + 228.6 - 70 = 65.6 \text{ dB}
\]

> **کسر تلفات:** Atmosphere Loss + Pointing Loss + Implementation Loss ≈ 15 dB

**SNR نهایی:** ≈ 50.6 dB

> 🎯 **نتیجه:** با SNR=50 dB و کدگذاری Concatenated، BER نهایی ≤ \( 10^{-9} \)

---

## 📊 جدول مقایسه سه کانال

| ویژگی | آکوستیک زیرآب | ماهواره‌ای (LEO) | فضای عمیق |
|:------|:-------------|:----------------|:----------|
| **فاصله** | 400 متر | 14,000 km | 225 میلیون km |
| **تضعیف** | ~80 dB | ~168 dB | ~290 dB |
| **پهنای باند** | 10 kHz | 50 MHz | 10 MHz |
| **تأخیر** | 0.3 ثانیه | 0.044 ثانیه | 750 ثانیه (12.5 دقیقه!) |
| **نویز غالب** | آکوستیک محیطی | کیهانی + حرارتی | کیهانی (خنک‌شده) |
| **مدولاسیون** | CPFSK (M=4) | QPSK | BPSK |
| **کدگذاری** | توربو (1/2) | LDPC (3/4) | Concatenated (RS+Conv) |
| **نرخ داده** | 200 bps | 20 Mbps | 50 bps |
| **BER نهایی** | \(10^{-6}\) | \(10^{-12}\) | \(10^{-9}\) |

---

## 💎 جمع‌بندی فلسفی

ببین چطور مهندس مخابرات برای هر کانال، یه استراتژی کاملاً متفاوت می‌چینه:

- **در کانال آکوستیک:** مشکل اصلی ISI و پهنای باند کم است ← راه‌حل: CPFSK + اکوالایزر DFE
- **در کانال ماهواره‌ای:** مشکل اصلی تضعیف فضای آزاد و دوپلر است ← راه‌حل: QPSK + LDPC + دایورسیتی
- **در کانال فضای عمیق:** مشکل اصلی تضعیف فوق‌العاده بالا و تأخیر زیاد است ← راه‌حل: BPSK + کدگذاری Concatenated

> 📖 **نکته کلیدی:** هر سه کانال از **همان اصول پایه کتاب پروکیس** استفاده می‌کنند، ولی با تنظیمات کاملاً متفاوت. این هنر مهندسی است که بداند برای هر سناریو، کدوم ابزار را از جعبه ابزار مخابرات بردارد.

---

## 🧮 جاییکه کانال فضای عمیق تبدیل به صحنه نبرد نهایی با فیزیک می‌شود

**سناریو مشخص:** از ایستگاه زمینی "گلداستون" در کالیفرنیا (دیش ۷۰ متری) می‌خواهیم فرمان به کاوشگر "نیوهورایزنز" (New Horizons) بفرستیم که الان از پلوتو گذشته و در کمربند کویپر قرار دارد.

> 📍 **فاصله:** 5 میلیارد کیلومتر | ⏱️ **تأخیر نور:** 4.5 ساعت! | 🎯 **این دیگه فقط مخابرات نیست، یه جور سفر در زمان است.**

### مدل ریاضی کانال فضای عمیق (فراتر از AWGN)

مدل AWGN ساده (فصل 4) برای این سناریو کافی نیست. مدل واقعی شامل موارد زیر است:

#### 1. تضعیف فضای آزاد (Free Space Path Loss)

\[
L_{\text{fs}} = \left( \frac{4\pi d}{\lambda} \right)^2
\]

که در این معادله:
- \( L_{\text{fs}} \) = تلفات مسیر فضای آزاد (نسبت توان)
- \( d \) = فاصله بین آنتن فرستنده و گیرنده (متر)
- \( \lambda \) = طول موج سیگنال ارسالی (متر)

> 🔑 **نکته بنیادین:** تلفات توان سیگنال با **مجذور فاصله** و به‌طور معکوس با **مجذور طول موج** (یعنی به‌طور مستقیم با مجذور فرکانس) متناسب است. هر چه فاصله بیشتر یا فرکانس بالاتر باشد، سیگنال به شدت ضعیف‌تر می‌شود.

---

**ادامه دارد...** در بخش بعدی، مدل‌های ریاضی کانال‌های مخابراتی را تکمیل خواهیم کرد.

## 🧮 ادامه محاسبات کانال فضای عمیق (نیوهورایزنز)

حالا عدد بذاریم توش:

- **فرکانس:** ۳۲ گیگاهرتز (باند Ka)
- **طول موج:** \( \lambda = c/f = 3\times10^8 / 32\times10^9 = 0.009375 \) متر (۹.۳۷ میلی‌متر)
- **فاصله:** \( d = 5\times10^{12} \) متر

**محاسبه تضعیف فضای آزاد:**

\[
L_{fs} = \left(\frac{4\pi \times 5 \times 10^{12}}{0.009375}\right)^2 \approx 4.5 \times 10^{31}
\]

به دسی‌بل:

\[
L_{fs,dB} = 10\log_{10}(4.5 \times 10^{31}) \approx 316 \text{ dB}
\]

> 😱 **یعنی ۳۱۶ دسی‌بل تضعیف!** برای درکش: اگه ۱۰۰ کیلووات بفرستی، بعد از این تضعیف، \( 3.16\times10^{-27} \) وات میرسه. یعنی یه الکترون باید با خودش کلنجار بره که این توان رو اندازه بگیره.

---

## 📊 بودجه لینک دقیق (Link Budget Analysis)

### فرستنده زمینی (گلداستون - DSS-14)

| پارامتر | مقدار | محاسبه |
|:--------|:-----:|:-------|
| توان خروجی تقویت‌کننده | ۵۰ kW | \( 10\log_{10}(50000) = 47 \text{ dBW} = 77 \text{ dBm} \) |
| بهره آنتن ۷۰ متری | 75.8 dBi | \( G = 0.7 \times (\pi \times 70 / 0.009375)^2 \) |
| **EIRP** | **152.8 dBm** | \( 77 + 75.8 \) |

### مسیر انتشار

| پارامتر | مقدار | توضیح |
|:--------|:-----:|:------|
| تلفات فضای آزاد | -316 dB | محاسبه شد |
| تلفات اتمسفری | -2 dB | در فرکانس 32 GHz، هوای صاف |
| تلفات نشانه‌روی (Pointing Loss) | -1 dB | دقت 0.005 درجه |

### گیرنده فضاپیما (نیوهورایزنز)

| پارامتر | مقدار | محاسبه |
|:--------|:-----:|:-------|
| آنتن سهموی ۲.۱ متری | ~52 dBi | \( G_r = 0.6 \times (\pi \times 2.1 / 0.009375)^2 \) |
| دمای نویز سیستم | 100 K | نمی‌شود مثل زمین خنک کرد |
| نویز فیگر | ~0.5 dB | \( NF = 1 + T_{sys}/290 \) |

### محاسبه توان دریافتی

\[
P_{rx} = \text{EIRP} - L_{fs} - L_{atm} - L_{point} + G_r
\]
\[
P_{rx} = 152.8 - 316 - 2 - 1 + 52 = -114.2 \text{ dBm}
\]

### محاسبه نویز

\[
N_0 = kT_{sys} = 1.38\times10^{-23} \times 100 = 1.38\times10^{-21} \text{ W/Hz} = -208.6 \text{ dBW/Hz}
\]

\[
N = N_0 \times B = -208.6 + 10\log_{10}(B)
\]

---

## 🎯 تصمیم بزرگ: انتخاب پهنای باند

اگر پهنای باند \( B = 1 \text{ MHz} \) در نظر بگیریم:

\[
N = -208.6 + 60 = -148.6 \text{ dBW} = -118.6 \text{ dBm}
\]

\[
\text{SNR} = -114.2 - (-118.6) = 4.4 \text{ dB}
\]

> ⚠️ با SNR=4.4 dB، هیچ غلطی نمیشه کرد! BER بدون کدگذاری برای BPSK در این SNR حدود \( 10^{-2} \) است.

---

## ✨ جادوی کدگذاری: نجات معجزه‌آسا از دل نویز

### کدهای الحاقی (Concatenated Codes) - بخش ۷.۱۳ کتاب

از یک ترکیب قدرتمند استفاده می‌کنیم:

```text
┌─────────────┐    ┌─────────────┐    ┌─────────────┐    ┌─────────────┐
│ اطلاعات     │───▶│ Reed-Solomon│───▶│ اینترلیور   │───▶│ کانولوشنال  │
│ 223 بایت    │   │ (255,223)   │   │ 5×255       │   │ نرخ 1/2     │
└─────────────┘    └─────────────┘    └─────────────┘    └─────────────┘
```

| لایه | مشخصات | نقش |
|:----:|:------:|:-----|
| **کد درونی** | کانولوشنال، نرخ 1/2، طول محدودیت 7 | تصحیح خطاهای تصادفی |
| **اینترلیور** | بلاکی 5×255 | پاشیدن خطاهای بسته‌ای |
| **کد بیرونی** | Reed-Solomon (255,223) | تصحیح خطاهای باقیمانده |

**نرخ کلی:** \( 0.875 \times 0.5 = 0.4375 \)

---

## 🔄 پردازش در گیرنده (Decoding Pipeline)

```text
┌─────────────┐    ┌─────────────┐    ┌─────────────┐    ┌─────────────┐
│ سیگنال      │───▶│ دیکدر       │───▶│ دی‌اینترلیور│───▶│ Reed-Solomon│
│ دریافتی     │    │ Viterbi     │    │ معکوس       │    │ Decoder     │
│ (LLR ها)    │    │ (نرم)       │    │             │    │             │
└─────────────┘    └─────────────┘    └─────────────┘    └─────────────┘
```

**نتایج عملکرد (طبق نمودارهای فصل ۸):**
- SNR=4.4 dB + کد کانولوشنال نرخ 1/2 ⇒ BER ≈ \( 5\times10^{-3} \)
- بعد از Reed-Solomon ⇒ BER ≈ \( 10^{-6} \)

> 🎉 یعنی از هر ۱ میلیون بیت، فقط **۱ بیت** خطا!

---

## 📡 هم‌سازی و ردیابی

### اثر دوپلر (Doppler Shift)

فضاپیما با سرعت ۱۵ کیلومتر بر ثانیه از ما دور می‌شود:

\[
\Delta f = f_c \times \frac{v}{c} = 32\times10^9 \times \frac{15000}{3\times10^8} = 1.6 \text{ MHz}
\]

> ⚠️ فرکانس دریافتی ۱.۶ مگاهرتز جابجا می‌شود!

**راه‌حل:** PLL با پهنای باند بسیار باریک (چند هرتز) که بتواند این شیفت را ردیابی کند.

### حلقه کاستاس (Costas Loop) برای BPSK

از آنجا که BPSK حامل سرکوب‌شده دارد، از **Costas Loop** استفاده می‌کنیم (بخش ۵.۲ کتاب). این حلقه فاز را از خود سیگنال مدوله‌شده استخراج می‌کند، بدون نیاز به حامل پایلوت.

---

## 📦 پروتکل‌های فضایی: وقتی تأخیر یعنی مرگ

تأخیر ۴.۵ ساعته یعنی با نرخ ۲ بیت بر ثانیه (با احتساب کدگذاری)، **۳۲۴۰۰ بیت در راه است**!

**راه‌حل - پروتکل CFDP (CCSDS File Delivery Protocol):**

| ویژگی | توضیح |
|:------|:------|
| **شماره‌گذاری بسته‌ها** | هر بسته شناسه یکتا دارد |
| **بدون ACK لحظه‌ای** | نیازی به تأیید فوری نیست |
| **Erasure Coding** | بسته‌های گمشده از روی بسته‌های دیگر بازسازی می‌شوند |

---

## 💎 جمع‌بندی: چرا این جهنمی است؟

مخابرات فضای عمیق، اثبات قضیه شانون (بخش ۶.۵) است: **"ظرفیت کانال با SNR رابطه لگاریتمی دارد، نه خطی"**. حتی در SNRهای منفی هم می‌توان مخابره کرد، به شرطی که به اندازه کافی صبور باشی.

| استراتژی | دلیل |
|:---------|:-----|
| **نرخ داده پایین (1-2 bps)** | کاهش پهنای باند ⇒ کاهش نویز |
| **کدگذاری قوی (نرخ 0.44)** | نزدیک به حد شانون |
| **گیرنده خنک‌شده (100K)** | کاهش نویز حرارتی |
| **دیش عظیم (70m)** | افزایش بهره آنتن |

> 🌟 **برگ برنده مهندس مخابرات:**
> - کدگذاری نزدیک به حد شانون (توربو، LDPC، کدهای الحاقی)
> - گیرنده‌های خنک‌شونده با هلیوم مایع
> - دمدولاتورهای همدوس با PLLهای فوق دقیق
> - و از همه مهمتر: **صبوری** - ۴.۵ ساعت صبر کنی تا یک عکس از پلوتو بیاد

---

## 🔄 اینترلیور (Interleaver) - قاطی‌کن حرفه‌ای داده‌ها

### تعریف ساده

اینترلیور یک **قاطی‌کن** یا **برهم‌زننده ترتیب** داده‌هاست. دنباله بیت‌ها یا سمبل‌های ورودی را به یک ترتیب شبه‌تصادفی جابجا می‌کند.

**مثال ساده:**

دنباله اصلی:
\[
x = [x_1, x_2, x_3, x_4, x_5, x_6, x_7, x_8]
\]

بعد از اینترلیور (نوشتن سطری، خواندن ستونی):
\[
x' = [x_1, x_3, x_5, x_7, x_2, x_4, x_6, x_8]
\]

در گیرنده، **دی‌اینترلیور** دقیقاً برعکس عمل می‌کند و ترتیب اصلی را برمی‌گرداند.

---

### چرا به قاطی‌کن نیاز داریم؟ (مشکل خطای بسته‌ای - Burst Error)

خیلی از کانال‌های مخابراتی، خطاهایشان **بسته‌ای (Bursty)** است:

| نوع کانال | مثال خطای بسته‌ای |
|:----------|:------------------|
| **بی‌سیم** | محوشدگی (Fading) - 5-10 میلی‌ثانیه قطع کامل |
| **صنعتی** | روشن شدن موتور، جرقه - قطار کامل بیت خراب |
| **ذخیره‌سازی** | خش روی CD/DVD - یک مسیر ممتد از بین رفته |

**مشکل اصلی:** کدهای تصحیح خطا (Reed-Solomon، کانولوشنال) برای **خطاهای تصادفی** طراحی شده‌اند، نه خطاهای بسته‌ای.

---

### راه‌حل: پاشیدن خطاها با اینترلیور

```text
فرستنده:
[داده] → [کدگذار] → [اینترلیور] → [کانال]

کانال:
یک خطای بسته‌ای 50 سمبلی رخ می‌دهد

گیرنده:
[دی‌اینترلیور] → [دیکدر] → [داده تصحیح‌شده]
                      ↑
                 خطاها پخش شدند!
```

---

### مثال فنی: ترکیب Reed-Solomon و اینترلیور

کد **Reed-Solomon (255, 223)** می‌تواند \( t = 16 \) سمبل خطا را تصحیح کند.

**بدون اینترلیور:**
- خطای بسته‌ای ۵۰ سمبل → همه در یک کلمه کد → ۵۰ خطا → دیکدر می‌گوید: "من فقط ۱۶ تا می‌توانم!"

**با اینترلیور بلاکی \(16 \times 255\):**
- ۱۶ کلمه کد در ۱۶ سطر نوشته می‌شوند
- داده‌ها ستونی ارسال می‌شوند
- خطای بسته‌ای ۵۰ سمبلی → به ستون‌های متوالی آسیب می‌زند
- بعد از دی‌اینترلیو کردن → ۵۰ خطا بین ۱۶ کلمه کد **پخش** می‌شوند
- هر کلمه کد فقط ۳-۴ خطا می‌بیند → دیکدر به راحتی تصحیح می‌کند!

> 🎯 **نتیجه:** یک کد Reed-Solomon ساده که در برابر خطای بسته‌ای فلج بود، با یک اینترلیور ساده به یک غول مقاوم تبدیل می‌شود.

---

## 📊 مفاهیمی که در تحلیل‌هایمان جا ماند (غول‌های فراموش‌شده)

### ۱. کدگذاری منبع در برابر کدگذاری کانال

| کدگذاری منبع | کدگذاری کانال |
|:------------|:--------------|
| کاهش **افزونگی آماری** داده | اضافه کردن **افزونگی ساختاریافته** |
| مثال: کد هافمن | مثال: بیت‌های Parity |
| هدف: **کارایی** (کاهش حجم) | هدف: **قابلیت اطمینان** (مقاومت به خطا) |
| فصل ۶ کتاب | فصل ۷ و ۸ کتاب |

### ۲. منحنی عملکرد (Waterfall Curve)

رابطه بین SNR و BER را نشان می‌دهد:

```text
BER
  │
10⁻⁰│    
  │     ╲
10⁻²│      ╲___
  │         ╲___  ← زانویی (Knee)
10⁻⁴│            ╲___
  │               ╲___  ← Waterfall
10⁻⁶│                 ╲___
  │                    ╲___
  └────────────────────────── SNR
      0    2    4    6    8   10 dB
```

> 💡 کدهای توربو و LDPC این زانو را تا نزدیکی **حد شانون** می‌برند!

### ۳. نرخ کد (Code Rate)

\[
R = \frac{k}{n}
\]

| نرخ کد | معنی | فداکاری | بهره |
|:------:|:----:|:--------|:-----|
| 1/2 | هر بیت → ۲ بیت | ۲ برابر پهنای باند | ~5-7 dB |
| 1/3 | هر بیت → ۳ بیت | ۳ برابر پهنای باند | ~8-10 dB |
| 3/4 | ۳ بیت → ۴ بیت | ۱.۳۳ برابر پهنای باند | ~3-4 dB |

### ۴. فاصله همینگ در برابر فاصله اقلیدسی

| نوع فاصله | تعریف | کاربرد |
|:----------|:------|:--------|
| **فاصله همینگ** | تعداد بیت‌های متفاوت بین دو کلمه کد | کدگذاری کانال |
| **فاصله اقلیدسی** | فاصله هندسی بین نقاط صورت فلکی | مدولاسیون |

\[
d_{min} \text{ (اقلیدسی)} \Rightarrow \text{احتمال خطا} \propto Q\left(\sqrt{\frac{E_s}{N_0} \cdot d_{min}^2}\right)
\]

### ۵. معیار نایکوئیست (Nyquist Criterion)

برای ارسال بدون ISI در کانال با پهنای باند \( W \):

\[
\text{حداکثر نرخ سمبل} = 2W \quad \text{(سمبل بر ثانیه)}
\]

**پالس‌های Nyquist** مانند **raised cosine** برای این هدف طراحی شده‌اند (فصل ۹ کتاب).

### ۶. دمدولاسیون همدوس (Coherent) در برابر غیرهمدوس (Noncoherent)

| نوع | نیاز به فاز حامل | BER (نسبت به همدوس) | کاربرد |
|:---:|:---------------:|:-------------------:|:--------|
| **همدوس** | دارد (PLL, Costas) | مرجع | فضای عمیق، ماهواره |
| **غیرهمدوس** | ندارد (DPSK, Noncoherent FSK) | +3 dB بدتر | IoT، رادیوهای ارزان |

### ۷. تکنیک‌های دایورسیتی (Diversity)

| نوع | روش | کاربرد |
|:----|:----|:--------|
| **فضایی** | چند آنتن (MIMO, Alamouti) | MIMO، 5G |
| **زمانی** | ارسال چندباره + اینترلیوینگ | کدهای توربو |
| **فرکانسی** | چند فرکانس (OFDM + کدگذاری) | Wi-Fi, 4G/5G |
| **قطبی** | دو قطبش عمودی/افقی | ماهواره، پخش |

### ۸. نرخ قطع کانال (Channel Cutoff Rate - \( R_0 \))

معیاری قدیمی‌تر از ظرفیت شانون برای طراحی کدهای کانولوشنال:

\[
R_0 = \log_2\left(1 + \frac{E_s}{N_0}\right) \quad \text{(برای AWGN)}
\]

> امروزه با توربو و LDPC، ظرفیت شانون معیار اصلی است.

### ۹. کدهای سوراخ‌شده (Punctured Codes)

تکنیکی برای افزایش نرخ کد از یک کد پایه:

```text
کد پایه نرخ 1/2:  [x1 x2 x3 x4 x5 x6 ...]
                         ↓ حذف (Puncture)
کد نرخ 3/4:      [x1 x2 x4 x5 ...]
                        (x3, x6 حذف شدند)

در دیکدر: صفرها را جایگزین بیت‌های حذف‌شده می‌کنیم
```

**مزیت:** انعطاف‌پذیری نرخ کد با یک کدگذار پایه (فصل ۸.۴ کتاب)

---

## 📈 جمع‌بندی نهایی غول‌های فراموش‌شده

| مفهوم | فصل | اهمیت |
|:------|:----:|:------|
| کدگذاری منبع | ۶ | فشرده‌سازی |
| منحنی Waterfall | ۴، ۷ | ارزیابی عملکرد |
| نرخ کد \(R = k/n\) | ۷-۸ | تریدآف پهنای باند/بهره |
| فاصله همینگ و اقلیدسی | ۳، ۷ | طراحی مدولاسیون و کد |
| معیار نایکوئیست | ۹ | جلوگیری از ISI |
| همدوس/غیرهمدوس | ۴ | انتخاب گیرنده |
| دایورسیتی | ۱۳ | مقابله با محوشدگی |
| نرخ قطع \(R_0\) | ۶، ۱۴ | تحلیل کدهای کانولوشنال |
| کدهای سوراخ‌شده | ۸ | انعطاف نرخ کد |

> 🎓 **نکته نهایی:** هر کدوم از این مفاهیم، یک "سلاح" در جعبه ابزار مهندس مخابرات است. دانستن اینکه دقیقاً کدام ابزار را در چه شرایطی استفاده کنیم، هنر این حرفه است.


## ۱.۳ مدل‌های ریاضی برای کانال‌های مخابراتی

در طراحی سیستم‌های مخابراتی برای ارسال اطلاعات از طریق کانال‌های فیزیکی، ساختن مدل‌های ریاضی که مهم‌ترین خصوصیات رسانه انتقال را منعکس می‌کنند، ضروری است. سپس، مدل ریاضی کانال در طراحی کدگذار کانال و مدولاتور در فرستنده، و دمودولاتور و دیکدر کانال در گیرنده استفاده می‌شود.

---

### 📡 کانال با نویز جمع‌شونده (Additive Noise Channel)

ساده‌ترین مدل ریاضی برای یک کانال مخابراتی، کانال با نویز جمع‌شونده است که در شکل ۱-۳-۱ نشان داده شده است. در این مدل، سیگنال ارسالی s(t) توسط یک فرایند تصادفی نویز جمع‌شونده n(t) تخریب می‌شود.

**منابع فیزیکی نویز:**
- قطعات الکترونیکی و تقویت‌کننده‌ها در گیرنده
- تداخل ایجادشده در حین ارسال (مانند ارسال سیگنال رادیویی)

**نویز گاوسی (Gaussian Noise):** اگر نویز عمدتاً توسط قطعات الکترونیکی و تقویت‌کننده‌ها در گیرنده تولید شود، می‌توان آن را به‌عنوان **نویز گرمایی** مشخصه‌سازی کرد. این نوع نویز از نظر آماری به‌عنوان یک فرایند نویز گاوسی مشخصه‌سازی می‌شود. از این رو، مدل ریاضی حاصل برای کانال معمولاً **کانال با نویز گاوسی جمع‌شونده (AWGN)** نامیده می‌شود.

**مدل ریاضی با تضعیف:**

وقتی سیگنال در هنگام ارسال از طریق کانال دچار تضعیف می‌شود، سیگنال دریافتی به صورت زیر است:

\[
r(t) = \alpha s(t) + n(t) \qquad (1.3-1)
\]

که در آن α ضریب تضعیف است.

---

### 📡 کانال فیلتر خطی (Linear Filter Channel)

در برخی کانال‌های فیزیکی، مانند کانال‌های تلفن باسیم، از فیلترها برای اطمینان از این‌که سیگنال‌های ارسالی محدودیت‌های پهنای باند مشخص‌شده را نقض نکرده و در نتیجه با یکدیگر تداخل نکنند، استفاده می‌شود. چنین کانال‌هایی معمولاً از نظر ریاضی به‌عنوان **کانال‌های فیلتر خطی با نویز جمع‌شونده** مشخصه‌سازی می‌شوند.

**مدل ریاضی:**

اگر ورودی کانال سیگنال s(t) باشد، خروجی کانال سیگنال زیر است:

\[
r(t) = s(t) \ast c(t) + n(t) = \int_{-\infty}^{\infty} c(\tau) s(t - \tau) \, d\tau + n(t) \qquad (1.3-2)
\]

که در آن:
- \( c(t) \) = پاسخ ضربه فیلتر خطی
- \( \ast \) = عمل کانولوشن

---

### 📡 کانال فیلتر متغیر با زمان خطی (Linear Time-Varying Filter Channel)

کانال‌های فیزیکی مانند کانال‌های آکوستیک زیرآب و کانال‌های رادیویی یونوسفری که منجر به انتشار چندمسیره متغیر با زمان سیگنال ارسالی می‌شوند، می‌توانند از نظر ریاضی به‌عنوان فیلترهای خطی متغیر با زمان مشخصه‌سازی شوند.

**مدل ریاضی عمومی:**

چنین فیلترهای خطی با یک پاسخ ضربه کانال متغیر با زمان \( c(\tau; t) \) مشخص می‌شوند، که در آن \( c(\tau; t) \) پاسخ کانال در زمان t ناشی از اعمال یک ضربه در زمان \( t - \tau \) است.

برای یک سیگنال ورودی s(t)، سیگنال خروجی کانال به صورت زیر است:

\[
r(t) = s(t) \ast c(\tau; t) + n(t) = \int_{-\infty}^{\infty} c(\tau; t) s(t - \tau) \, d\tau + n(t) \qquad (1.3-3)
\]

---

### 🔥 مدل خاص: کانال چندمسیره (Multipath Channel)

یک مدل خوب برای انتشار سیگنال چندمسیره از طریق کانال‌های فیزیکی، مانند یونوسفر (در فرکانس‌های زیر ۳۰ مگاهرتز) و کانال‌های رادیویی سلولی موبایل، یک حالت خاص از معادله (۱-۳-۳) است که در آن پاسخ ضربه متغیر با زمان به شکل زیر است:

\[
c(\tau; t) = \sum_{k=1}^{L} a_k(t) \delta(\tau - \tau_k) \qquad (1.3-4)
\]

که در آن:
- \( \{a_k(t)\} \) = ضرایب تضعیف احتمالاً متغیر با زمان برای L مسیر انتشار چندمسیره
- \( \{\tau_k\} \) = تأخیرهای متناظر با آن‌ها

**سیگنال دریافتی نهایی:**

با جایگذاری معادله (۱-۳-۴) در (۱-۳-۳):

\[
r(t) = \sum_{k=1}^{L} a_k(t) s(t - \tau_k) + n(t) \qquad (1.3-5)
\]

بنابراین، سیگنال دریافتی از L مؤلفه چندمسیره تشکیل شده است، که در آن مؤلفه k-ام با \( a_k(t) \) تضعیف شده و به اندازه \( \tau_k \) تأخیر یافته است.

---

## 🚨 سناریوی ترکیبی: فروپاشی زیرساخت

> **سناریو:** یک زمین‌لرزه مهیب در یک کلان‌شهر رخ داده است. تمام خطوط فیبر نوری و دکل‌های مخابراتی نابود شده‌اند. یک تیم امداد در زیر آوار یک بیمارستان فروریخته، با استفاده از یک ربات مارمانند فیبر نوری، بازماندگانی را پیدا می‌کند. ربات یک پیام حیاتی حاوی **علائم حیاتی و موقعیت دقیق** را از طریق کابل فیبر نوری خود به یک دستگاه فرستنده در بیرون آوار می‌فرستد. این فرستنده باید این داده‌ها را از میان گرد و غبار، دود و تداخل شدید رادیویی به یک پهپاد رله مخابراتی در حال پرواز برساند.

پیام از سه کانال کاملاً مجزا عبور می‌کند که به ترتیب با سه مدل ریاضی ما مطابقت دارند.

---

### گام ۱: از ربات در زیر آوار تا فرستنده (کانال فیلتر خطی)

**مدل ریاضی:** \( r(t) = s(t) * c(t) + n(t) \) - معادله (1.3-2)

| مؤلفه | توضیح |
|:------|:------|
| **s(t)** | ربات داده‌های حیاتی را به سیگنال دیجیتال پرسرعت (۱ گیگابیت بر ثانیه) تبدیل کرده و با لیزر مادون قرمز به درون کابل فیبر نوری می‌فرستد |
| **c(t)** | کابل آسیب‌دیده یک فیلتر خطی ایجاد می‌کند: تضعیف (~10 dB) + پاشندگی (Dispersion) |
| **n(t)** | نویز حرارتی در آشکارساز نوری (فوتودیود) |

**فاجعه پاشندگی:** سرعت انتشار نور در فیبر برای فرکانس‌های مختلف متفاوت است. یک پالس نوری باریک در طول مسیر پخش می‌شود و به پالس‌های مجاور نشت می‌کند → **تداخل بین سمبلی (ISI)**

**راه‌حل مهندسی:** استفاده از **یکسان‌ساز خطی (Linear Equalizer)** با تابع \( c^{-1}(t) \) برای وارونه کردن اثر فیلتر.

---

### گام ۲: از فرستنده روی زمین به پهپاد رله (کانال فیلتر متغیر با زمان خطی)

**مدل ریاضی:** \( r(t) = \sum_{k=1}^{L} a_k(t) s(t - \tau_k) + n(t) \) - معادله (1.3-5)

**محیط:** شهر ویران شده، پر از ساختمان‌های نیمه‌فرو ریخته، جرثقیل‌های امدادی و گرد و غبار. خبری از دید مستقیم (LOS) پایدار نیست.

**تولید چندمسیر (L=4):**

| مسیر | نوع | تأخیر نسبی |
|:----:|:----|:----------:|
| ۱ | مستقیم (لحظه‌ای باز و بسته می‌شود) | \( \tau_1 \) |
| ۲ | انعکاس از برج فلزی نیمه‌کاره | \( \tau_2 > \tau_1 \) |
| ۳ | انعکاس از زمین | \( \tau_3 > \tau_1 \) |
| ۴ | پراش از لبه تیز تخته سنگ | \( \tau_4 > \tau_1 \) |

**پارامترهای متغیر با زمان:**

- پهپاد در حال حرکت است
- بیل‌های مکانیکی و آمبولانس‌ها در صحنه تردد دارند
- حرکات باعث تغییر طول مسیرها → تغییر تأخیرهای \( \tau_k(t) \)

**محوشدگی (Fading):** تغییرات فاز هر مسیر در گیرنده:
- فازها هم‌فاز → جمع سازنده → سیگنال قوی
- فازها غیرهم‌فاز → جمع تخریبی → سیگنال ضعیف (محوشدگی)
- توان سیگنال می‌تواند تا ۳۰-۴۰ دسی‌بل نوسان کند!

**نتیجه:** خطای بسته‌ای (Burst Error) - یک "دره محوشدگی" می‌آید و صدها بیت پشت سر هم را نابود می‌کند.

**راه‌حل‌های مهندسی (بر اساس فصول کتاب):**

| راه‌حل | فصل | توضیح |
|:-------|:----:|:------|
| **دایورسیتی فضایی** | ۱۳.۴ | دو آنتن با فاصله روی پهپاد - احتمال دره مشترک کمتر |
| **اینترلیور عمیق** | ۷.۱۳ | قاطی کردن بیت‌ها → خطای بسته‌ای → خطای تصادفی |
| **دمودولاتور RAKE** | ۱۳.۵ | گیرنده هوشمند: هر مسیر را جدا می‌گیرد، هم‌فاز می‌کند و جمع می‌زند |

---

## 🏛️ ۱.۴ چشم‌اندازی تاریخی در توسعه مخابرات دیجیتال

### داستان حماسی: از دود مورس تا معجزه توربو

---

### پرده اول: تولد دود (۱۸۳۷ - ساموئل مورس)

ساموئل مورس یک نقاش بود، نه مهندس! ولی وقتی نامه‌ای که با اسب فرستاده بودند دیر رسید و همسرش مرد، قسم خورد راهی برای ارتباط سریع پیدا کند.

**چالش:** فقط یک سیم مسی دارد که جریان الکتریکی را رد می‌کند. چطور حروف الفبا را با یک سیم که فقط "قطعه" یا "وصله" می‌فرستد؟

**راه‌حل:** یک کد با طول متغیر اختراع کرد:
- حرف پرتکرار **E** → یک نقطه **(.)**
- حرف کم‌تکرار **Q** → خط خط نقطه خط **(--.-)**

**تحلیل خفن:**
مورس ناخودآگاه یک اصل بهینه‌سازی را کشف کرد: به حروف پرتکرار کد کوتاه بده. این دقیقاً همان کاری است که **کد هافمن** (فصل ۶ کتاب) ۱۱۰ سال بعد به صورت ریاضی اثبات کرد.

- نرخ متوسط بیت در کد مورس برای انگلیسی: ~۲.۵ بیت بر حرف
- اگر همه حروف کد ۵ بیتی داشتند (مثل بودو): ۵ بیت بر حرف
- **صرفه‌جویی پهنای باند: ۵۰٪!** (بدون دانستن ریاضیات)

---

### پرده دوم: محدودیت سرعت (۱۹۲۴ - هری نایکوئیست)

۷۰ سال از مورس گذشته. تلگراف همه‌جا را گرفته. ولی یک مشکل: اگر پالس‌ها را خیلی سریع پشت هم بفرستی، در گیرنده قاطی می‌شوند.

**سؤال نایکوئیست:** "روی این کابل با پهنای باند W هرتز، حداکثر چند پالس در ثانیه می‌توانیم بفرستیم بدون این که قاطی بشوند؟"

**فرمول جادویی نایکوئیست:**

\[
s(t) = \sum_{n} a_n g(t - nT)
\]

فهمید که اگر پالس‌ها را به شکل \( \frac{\sin(2\pi Wt)}{2\pi Wt} \) (پالس سینک) بفرستی، می‌توانی با نرخ **۲W پالس در ثانیه** بفرستی بدون ISI در لحظات نمونه‌برداری.

> 📌 **نرخ نایکوئیست = 2W پالس/ثانیه**

**تحلیل خفن:**
نایکوئیست فهمید که مشکل ISI، یک مشکل **طراحی پالس** است، نه محدودیت فیزیکی. اگر پالس‌ها را طوری طراحی کنی که در لحظه نمونه‌برداری پالس همسایه صفر باشد، ISI غیب می‌شود. این بینش، پایه تمام سیستم‌های مخابرات دیجیتال مدرن شد.

---

### پرده سوم: معمای نویز (۱۹۲۸-۱۹۴۸ - هارتلی تا شانون)

حالا می‌دانیم چقدر سریع می‌توانیم پالس بفرستیم. ولی یک سؤال مرگبار: در حضور نویز، چقدر **اطلاعات** می‌توانیم بفرستیم؟

**هارتلی (۱۹۲۸):**
فهمید که تعداد سطوح دامنه‌ای که گیرنده می‌تواند تشخیص بدهد، به نسبت حداکثر دامنه به عدم قطعیت نویز بستگی دارد.

مثال: سیگنال بین -1V تا +1V، نویز 0.1V → 20 سطح قابل تشخیص → \( \log_2(20) \approx 4.3 \) بیت بر پالس
→ حداکثر نرخ ≈ \( 2W \times 4.3 \)

این یک تقریب شهودی بود، نه یک قضیه دقیق.

**کلود شانون (۱۹۴۸) - سلطان وارد می‌شود:**

در یک مقاله ۵۵ صفحه‌ای که دنیا را تکان داد، نشان داد:

\[
C = W \log_2\left(1 + \frac{P}{N_0 W}\right) \quad \text{(bits/second)}
\]

که در آن:
- \( C \) = ظرفیت کانال (حداکثر نرخ اطلاعات با خطای صفر)
- \( W \) = پهنای باند (هرتز)
- \( P \) = متوسط توان ارسالی (وات)
- \( N_0 \) = چگالی طیف توان نویز (وات/هرتز)

**تحلیل خفن فرمول شانون:**

| سناریو | نتیجه |
|:-------|:------|
| \( W \to \infty \) | \( C \to \frac{P}{N_0 \ln 2} \) (ظرفیت محدود به توان، نه پهنای باند) |
| SNR = 0 dB (\( P = N_0W \)) | \( C = W \log_2(2) = W \) (هنوز هم به اندازه پهنای باند می‌توان اطلاعات فرستاد!) |
| SNR منفی | \( C > 0 \) (می‌توان در SNR منفی هم ارتباط برقرار کرد، فقط نرخ را کم کن) |

**تأثیر زلزله‌آسا بر مهندسی مخابرات:**

| قبل از شانون | بعد از شانون |
|:------------|:-------------|
| برای کاهش خطا: توان را زیاد کن یا نرخ را کم کن | با کدگذاری هوشمند می‌توان خطا را بدون افزایش توان به صفر نزدیک کرد |
| طراحی سیستم = سرانگشتی | طراحی سیستم = تلاش برای رسیدن به ظرفیت شانون |
| محدودیت فیزیکی کانال = معمای حل‌نشده | محدودیت فیزیکی = \( C = W \log_2(1 + \text{SNR}) \) |

---

### جدول زمانی قهرمانان مخابرات دیجیتال

| سال | قهرمان | کشف | فصل کتاب |
|:---:|:-------|:----|:--------:|
| 1837 | ساموئل مورس | کد مورس (کدگذاری منبع با طول متغیر) | ۶ |
| 1875 | امیل بودو | کد با طول ثابت ۵ بیت | ۶ |
| 1924 | هری نایکوئیست | نرخ نایکوئیست = 2W پالس/ثانیه | ۹ |
| 1928 | رالف هارتلی | حدس ظرفیت کانال با سطوح دامنه | ۶ |
| 1942 | نوربرت وینر | فیلتر وینر (تخمین سیگنال در نویز) | ۱۰ |
| 1948 | کلود شانون | قضیه ظرفیت کانال \( C = W \log_2(1 + \text{SNR}) \) | ۶ |
| 1950 | ریچارد همینگ | کدهای آشکارسازی و تصحیح خطا | ۷ |
| 1963 | رابرت گالاگر | کدهای LDPC | ۸ |
| 1967 | اندرو ویتربی | الگوریتم ویتربی برای دیکدینگ کانولوشنال | ۸ |
| 1982 | گوتفرید اونگربوک | مدولاسیون کدشده تریلیس (TCM) | ۸ |
| 1993 | برو، گلاویو، تیتیمارشا | کدهای توربو و دیکدینگ تکراری | ۸ |

---

## 📊 جمع‌بندی سه مدل کانال

| مدل | فرمول | کاربرد | مشکل اصلی | راه‌حل (فصل) |
|:----|:-----:|:-------|:----------|:------------:|
| **نویز جمع‌شونده (AWGN)** | \( r = \alpha s + n \) | ماهواره، فضای عمیق | نویز حرارتی | کدگذاری قوی (۷,۸) |
| **فیلتر خطی** | \( r = s * c + n \) | فیبر نوری، کابل | ISI ناشی از پاشندگی | یکسان‌ساز (۹,۱۰) |
| **متغیر با زمان (چندمسیره)** | \( r = \sum a_k s(t-\tau_k) + n \) | موبایل، رادیو | محوشدگی + ISI | RAKE, اینترلیور (۱۳) |


> 📖 **ادامه دارد...** در بخش بعدی، چشم‌اندازی کامل‌تر از توسعه کدهای تصحیح خطا و انقلاب توربو و LDPC را بررسی خواهیم کرد.
---
# 🎯 سناریوی نهایی: سفر یک عکس از مریخ به زمین

## صحنه: مریخ، دهانه جیزرو، ۱۸ فوریه ۲۰۲۱

مریخ‌نورد **پرسویرنس (Perseverance)** تازه روی مریخ فرود اومده. اولین عکس رنگی با کیفیت بالا (۴۰۹۶ × ۲۱۶۰ پیکسل، ۲۴ بیت رنگ) از سطح مریخ گرفته شده. این عکس باید به زمین برسه تا دانشمندان بتونن محل مناسب برای جستجوی حیات باستانی رو انتخاب کنن.

**حجم عکس خام:** \( 4096 \times 2160 \times 24 \approx 212 \) میلیون بیت \( \approx 26.5 \) مگابایت

این داده حیاتی باید از مریخ به زمین بره. اما چطور؟

---

## 📜 مرحله صفر: چشم‌انداز تاریخی (بخش ۱.۴)

قبل از این که وارد جزئیات فنی بشیم، بذار یه لحظه به تاریخ ادای احترام کنم:

| سال | قهرمان | کشف | تأثیر بر مأموریت |
|:---:|:-------|:----|:-----------------|
| 1837 | مورس | کد مورس | اگر امروز از کد مورس استفاده می‌کردیم، ارسال عکس **چندین سال** طول می‌کشید! |
| 1924 | نایکوئیست | نرخ \( 2W \) پالس/ثانیه | به ما می‌گه با پهنای باند محدود، چقدر سریع می‌تونیم پالس بفرستیم |
| 1928 | هارتلی | سطوح دامنه چندگانه | پایه مدولاسیون‌های M-تایی برای افزایش نرخ داده |
| 1948 | شانون | \( C = W \log_2(1 + \text{SNR}) \) | سقف آسمونی: هر طراحی باید زیر این سقف باشه |
| 1950-1993 | همینگ، رید-سولومون، ویتربی، برو | کدهای تصحیح خطا | کدهایی که امروز تو پرسویرنس استفاده میشه |

**نتیجه تاریخی:** امروز پرسویرنس می‌تونه تا 2 مگابیت بر ثانیه به مدارگرد مریخ بفرسته. چیزی که برای مورس معجزه بود، امروز روتینه.

---

## 🗜️ مرحله ۱: کدگذاری منبع (بخش ۶.۴ - فشرده‌سازی داده با اتلاف)

عکس 26.5 مگابایتی خام، افزونگی (Redundancy) زیادی داره. آسمان مریخ در خیلی از پیکسل‌ها یک رنگه. کدگذار منبع باید این افزونگی آماری را حذف کنه.

**استاندارد:** CCSDS 122.0 (مخصوص فضا) - فشرده‌سازی با تبدیل موجک (Wavelet Transform) شبیه JPEG2000

**نتیجه:** نرخ فشرده‌سازی 10:1
- 26.5 مگابایت → 2.65 مگابایت (21.2 میلیون بیت)

**چرا 10:1؟** فشرده‌سازی بدون اتلاف (Lossless) فقط 2:1 جواب میده. ما از فشرده‌سازی با اتلاف (Lossy) کنترل‌شده استفاده می‌کنیم. دانشمندان قبول کردن که کمی کیفیت فدا بشه تا حجم کمتر بشه. این یعنی **Rate-Distortion Theory** (بخش ۶.۴ کتاب).

> 💡 **تحلیل:** مثل اینه که به جای این که تک‌تک پیکسل‌های آسمون رو بفرستی (که همشون قرمز-نارنجی‌ان)، بگی "از پیکسل ۱۰۰۰ تا ۲۰۰۰، همه یک رنگ". این فرمول ساده، ۵۰٪ حجم رو کم می‌کنه بدون این که اطلاعات علمی از دست بره.

---

## 🛡️ مرحله ۲: کدگذاری کانال (بخش ۷ و ۸ - محافظت از عکس)

حالا 21.2 میلیون بیت اطلاعات فشرده داریم. باید از فاصله 225 میلیون کیلومتری مریخ به زمین بفرستیم.

### مشخصات کانال (مدل ریاضی - بخش ۱.۳)

**الف) مدل ریاضی پایه:** \( r(t) = \alpha s(t) + n(t) \)

- **فرکانس:** 8.4 گیگاهرتز (باند X، مخصوص فضا)
- **طول موج:** \( \lambda = c/f = 3\times10^8 / 8.4\times10^9 \approx 0.0357 \) متر
- **فاصله:** \( d = 2.25\times10^{11} \) متر
- **تضعیف مسیر:** \( L = (4\pi d/\lambda)^2 \approx 6.3 \times 10^{27} \approx 278 \) دسی‌بل!

**توان دریافتی از 20 وات فرستنده پرسویرنس:**
\[
P_r = 20 \times 10^{43.5} / 10^{27.8} \approx 1.26 \times 10^{-17} \text{ وات}
\]

> 😱 **12.6 آتووات!** (atto = 10⁻¹⁸). توان یک لامپ 100 واتی خانه \( 10^{19} \) برابر این است!

**ب) نویز \( n(t) \):** دمای نویز سیستم در گیرنده Deep Space Network با خنک‌سازی هلیوم مایع: 25 کلوین
\[
N_0 = kT = 1.38 \times 10^{-23} \times 25 \approx 3.45 \times 10^{-22} \text{ W/Hz} = -214.6 \text{ dBW/Hz}
\]

**ج) SNR قابل دستیابی:** با پهنای باند 6 مگاهرتز
\[
P_n = N_0 \times B = 3.45 \times 10^{-22} \times 6 \times 10^6 \approx 2.07 \times 10^{-15} \text{ W}
\]
\[
\text{SNR} = \frac{1.26 \times 10^{-17}}{2.07 \times 10^{-15}} \approx 0.00608 \approx -22.2 \text{ dB}
\]

> ⚠️ **SNR = -22 دسی‌بل!!!** این یعنی سیگنال 150 برابر ضعیف‌تر از نویزه! بدون کدگذاری، هیچ شانسی برای ارتباط نیست. ولی شانون میگه اگر \( R < C \) باشد، می‌شود.

**ظرفیت کانال (فرمول شانون - معادله 1.4-3):**
\[
C = 6 \times 10^6 \times \log_2(1 + 0.00608) \approx 6 \times 10^6 \times 0.00876 \approx 52,560 \text{ bps}
\]

پس حداکثر 52.5 کیلوبیت بر ثانیه می‌تونیم با خطای صفر بفرستیم.

### انتخاب کدگذاری (فصل‌های ۷ و ۸)

ناسا از استاندارد **CCSDS 131.0** استفاده می‌کنه: **کدهای الحاقی (Concatenated Codes)** - بخش ۷.۱۳

```text
┌─────────────┐    ┌─────────────┐    ┌─────────────┐    ┌─────────────┐
│ اطلاعات     │───▶│ Reed-Solomon│───▶│ اینترلیور   │───▶│ کانولوشنال  │
│ 21.2 Mb     │   │ (255,223)   │   │ عمق 5       │   │ نرخ 1/2     │
└─────────────┘    └─────────────┘    └─────────────┘    └─────────────┘
```

| لایه | مشخصات | نقش |
|:----:|:------:|:-----|
| **کد درونی** | کانولوشنال، نرخ 1/2، طول محدودیت 7 | تصحیح خطاهای تصادفی |
| **اینترلیور** | عمق 5 | پاشیدن خطاهای بسته‌ای |
| **کد بیرونی** | Reed-Solomon (255,223) | تصحیح خطاهای باقیمانده |

**نرخ کلی:** \( 0.875 \times 0.5 = 0.4375 \)

اطلاعات 21.2 میلیون بیتی → بعد از کدگذاری 48.5 میلیون بیت

**زمان ارسال با نرخ 50 کیلوبیت بر ثانیه:**
\[
t = \frac{48.5 \times 10^6}{50 \times 10^3} = 970 \text{ ثانیه} \approx 16 \text{ دقیقه}
\]

**چرا این ترکیب؟**
- کد کانولوشنال (Viterbi decoding) برای خطاهای تصادفی خوب است
- Reed-Solomon برای خطاهای بسته‌ای خوب است
- اینترلیور بین آنها خطاهای بسته‌ای را می‌پاشاند
- این دقیقاً عمل به توصیه شانون است: نزدیک شدن به ظرفیت با کدگذاری هوشمند

---

## 📡 مرحله ۳: مدولاسیون (بخش ۳.۲ - روش‌های مدولاسیون بدون حافظه)

حالا 48.5 میلیون بیت کدگذاری‌شده باید سوار موج بشن.

**انتخاب:** BPSK با فرکانس حامل 8.4 گیگاهرتز

**چرا BPSK نه QPSK یا QAM؟**
- در SNR = -22 dB (قبل از کدگذاری)، BPSK محکم‌ترین عملکرد را دارد
- BER بدون کدگذاری در این SNR ≈ 0.48 (تقریباً شانس!). ولی با بهره کدگذاری حدود 10 dB، BER مؤثر بعد از دیکدینگ به \( 10^{-6} \) می‌رسد.

**نرخ سمبل:** با نرخ بیت 50 کیلوبیت بر ثانیه و BPSK (1 بیت بر سمبل): \( R_s = 50,000 \) سمبل/ثانیه

**پهنای باند اشغالی:** با فیلتر Raised Cosine (\( \alpha = 0.5 \)):
\[
B = R_s(1 + \alpha) = 50,000 \times 1.5 = 75 \text{ kHz}
\]

**مدل سیگنال ارسالی (معادله 1.4-1 نایکوئیست):**
\[
s(t) = \sum_{n} a_n g(t - nT)
\]

که \( a_n \in \{+1, -1\} \) و \( g(t) \) پالس Raised Cosine با نرخ سقوط 0.5 است. این پالس طبق **معیار نایکوئیست** طراحی شده تا در لحظات نمونه‌برداری، ISI صفر باشد.

---

## 🌌 مرحله ۴: کانال فضای عمیق (مدل فیلتر متغیر با زمان - بخش ۱.۳)

کانال واقعی از مدل ساده \( r = \alpha s + n \) پیچیده‌تر است:

**الف) تأخیر انتشار:** \( 225 \text{ میلیون km} / 300,000 \text{ km/s} = 750 \text{ ثانیه} = 12.5 \text{ دقیقه} \)

**ب) شیفت دوپلر:** زمین و مریخ نسبت به هم حرکت می‌کنند. سرعت نسبی ≈ 10 km/s
\[
\Delta f = f_c \times \frac{v}{c} = 8.4 \times 10^9 \times \frac{10^4}{3\times10^8} \approx 280 \text{ kHz}
\]

> ⚠️ فرکانس حامل 280 کیلوهرتز جابجا می‌شود! گیرنده باید این را ردیابی کند.

**ج) محوشدگی رایان (Rician Fading) - بخش ۱۳.۳:**
اتمسفر مریخ (رقیق) + اتمسفر زمین + باد خورشیدی → محوشدگی با توزیع رایان (K-factor ≈ 10 dB). یعنی یک مؤلفه غالب (LOS) هست، ولی چند مؤلفه پراکنده نیز هستند.

**مدل دقیق کانال (معادله 1.3-5):**
\[
r(t) = \sum_{k=1}^{L} a_k(t) s(t - \tau_k) + n(t)
\]

که:
- \( L = 3 \) (مسیر مستقیم + دو مسیر پراکنده از جو مریخ)
- \( a_k(t) \) با توزیع رایان
- \( \tau_k \) تأخیر چندمسیر (کمتر از 1 میکروثانیه)

---

## 📡 مرحله ۵: گیرنده روی زمین (Deep Space Network)

**آنتن:** دیش 34 متری در گلداستون، کالیفرنیا. بهره ≈ 68 dBi در 8.4 گیگاهرتز

**تقویت‌کننده کم‌نویز (LNA):** خنک‌شده با هلیوم مایع تا 25 کلوین → نویز حرارتی حداقل

### دمودولاتور (فصل‌های ۴ و ۵)

1. **حلقه کاستاس (Costas Loop - بخش ۵.۲):** بازیابی فاز حامل BPSK. باید با وجود شیفت دوپلر 280 کیلوهرتز، قفل کند.

2. **حلقه هم‌سازی سمبل (بخش ۵.۳):** تخمین زمان بهینه نمونه‌برداری با الگوریتم Gardner.

3. **فیلتر منطبق (بخش ۴.۲):** با پاسخ ضربه منطبق بر پالس Raised Cosine فرستنده.

4. **نمونه‌بردار:** در لحظه‌ای که ISI صفر است (طبق نایکوئیست).

5. **خروجی:** دنباله‌ای از مقادیر **LLR (Log-Likelihood Ratio)** برای هر بیت، نه صفر و یک قطعی. یعنی "بیت اول 60٪ احتمال دارد 1 باشد". این **Soft Decision** برای دیکدر حیاتی است.

### دیکدینگ (فصل ۸)

```text
┌─────────────┐    ┌─────────────┐    ┌─────────────┐    ┌─────────────┐
│ LLR ها      │───▶│ دیکدر       │───▶│ دی‌اینترلیور│───▶│ دیکدر       │
│ از دمودولاتور│   │ Viterbi     │    │ معکوس       │    │ Reed-Solomon│
└─────────────┘    └─────────────┘    └─────────────┘    └─────────────┘
```

1. **دیکدر ویتربی (کد کانولوشنال - بخش ۸.۲):** 48.5 میلیون بیت را می‌گیرد و با بیشترین احتمال، دنباله اصلی را پیدا می‌کند.

2. **دی‌اینترلیور:** ترتیب اصلی را برمی‌گرداند.

3. **دیکدر Reed-Solomon:** خطاهای بسته‌ای باقیمانده را تصحیح می‌کند.

4. **خروجی:** 21.2 میلیون بیت (2.65 مگابایت) داده فشرده.

**کدگشای منبع (فصل ۶):** فشرده‌سازی موجک را باز می‌کند → 26.5 مگابایت عکس اصلی.

---

## 🎉 نتیجه

عکس 4096×2160 رنگی از مریخ، **16 دقیقه** بعد از شروع ارسال، در آزمایشگاه JPL روی صفحه نمایش ظاهر می‌شود. دانشمندان نفس خود را حبس می‌کنند. اولین منظره واضح از دهانه جیزرو...

---

## 📊 تحلیل نهایی: پیوند تمام بخش‌های فصل ۱

| بخش از فصل ۱ | کاربرد در سناریوی مریخ |
|:------------|:----------------------|
| **۱.۱ - اجزای سیستم** | کل زنجیره: منبع ← کدینگ منبع ← کدینگ کانال ← مدولاسیون ← کانال ← دمدولاسیون ← دیکدینگ کانال ← دیکدینگ منبع |
| **۱.۲ - انواع کانال** | کانال فضای عمیق (بی‌سیم LOS) با نویز کیهانی + حرارتی |
| **۱.۳ - مدل‌های ریاضی** | مدل پایه: \( r = \alpha s + n \) ← مدل دقیق: فیلتر متغیر با زمان با محوشدگی رایان |
| **۱.۴ - تاریخچه** | نایکوئیست (پالس بدون ISI)، شانون (ظرفیت کانال)، همینگ، رید-سولومون، فورنی، ویتربی (کدهای الحاقی) |
| **۱.۵ - ساختار کتاب** | فصل ۳-۴-۵ (مدولاسیون و دمدولاسیون)، فصل ۶-۷-۸ (کدگذاری)، فصل ۱۳-۱۴ (محوشدگی) |

---

## 💎 درس نهایی

مخابرات دیجیتال، **هنر غلبه بر فاصله و نویز** است. از نقطه و خط مورس تا عکس 26 مگابایتی از مریخ، همه یک اصول ثابت دارد:

1. **فشرده‌سازی هوشمندانه** (کدگذاری منبع)
2. **محافظت با کدگذاری قوی** (کدگذاری کانال)
3. **سوار کردن بر موج مناسب** (مدولاسیون)
4. **عبور از کانال خصمانه** (مدل‌سازی فیزیکی)
5. **بازسازی با ریاضیات دقیق** (دیکدینگ نرم + کدگشایی)

هرچه SNR کمتر باشد، **نبوغ بیشتری** لازم است. این مهندسی مخابرات است.

---

## 🧭 نقشه راه خواندن کتاب

```text
فصل 1 (مقدمه) ← همین الان اینجا هستیم ✅
    ↓
فصل 2 (تحلیل سیگنال) ← ابزارهای ریاضی: توابع تصادفی، سری‌ها، تبدیلات
    ↓
فصل 3 (مدولاسیون) ← طراحی BPSK، QPSK، QAM، CPM
    ↓
فصل 4 (گیرنده بهینه AWGN) ← فیلتر منطبق، آشکارسازی ML
    ↓
فصل 5 (هم‌سازی) ← تخمین فاز و زمان، PLL، Costas Loop
    ↓
فصل 6 (نظریه اطلاعات) ← فشرده‌سازی، ظرفیت کانال (شانون)
    ↓
فصل 7 و 8 (کدگذاری کانال) ← Reed-Solomon، کانولوشنال، توربو، LDPC
    ↓
فصل 9 و 10 (یکسان‌سازی) ← مقابله با ISI، اکوالایزر تطبیقی
    ↓
فصل 11 (OFDM) ← Wi-Fi، 4G/5G
    ↓
فصل 12 (طیف گسترده) ← GPS، CDMA، مقاومت به تداخل
    ↓
فصل 13 و 14 (محوشدگی) ← کانال‌های سیار، رایلی، رایسی، کدگذاری
    ↓
فصل 15 (MIMO) ← چند آنتن، Alamouti، دایورسیتی فضایی
    ↓
فصل 16 (چندکاربره) ← CDMA، NOMA، شبکه‌های سلولی
```

---

> 🎯 **تبریک!** فصل ۱ را کامل فهمیدی. حالا آماده‌ای برای **فصل ۲: تحلیل سیگنال‌های معین و تصادفی**، جایی که ابزارهای ریاضی دقیق برای مدل‌سازی نویز، سیگنال‌های میان‌گذر، و فرایندهای تصادفی را یاد می‌گیری.

## 📋 بخش تکمیلی فصل ۱

---

## 📝 خلاصه یک‌صفحه‌ای فصل ۱ (برای مرور سریع)

| مفهوم | تعریف خلاصه |
|:------|:-----------|
| **مخابرات دیجیتال** | انتقال اطلاعات به شکل دیجیتال از منبع به مقصد |
| **کدگذاری منبع** | حذف افزونگی آماری داده (فشرده‌سازی) برای کاهش حجم |
| **کدگذاری کانال** | افزودن افزونگی ساختاریافته برای مقابله با نویز |
| **مدولاسیون** | تبدیل بیت به شکل‌موج قابل ارسال در کانال |
| **کانال AWGN** | کانال با نویز سفید گاوسی جمع‌شونده |
| **کانال فیلتر خطی** | کانال با ISI ناشی از پاشندگی (dispersion) |
| **کانال متغیر با زمان** | کانال چندمسیره با محوشدگی (fading) |
| **ظرفیت کانال (شانون)** | \( C = W \log_2(1 + \text{SNR}) \) - حداکثر نرخ قابل اطمینان |

---

## 🧠 اصطلاحات کلیدی فصل ۱ (برای تقویت حافظه)

<details>
<summary><strong>🔤 کشوی اصطلاحات (کلیک کن)</strong></summary>

| اصطلاح فارسی | اصطلاح انگلیسی | تعریف سریع |
|:------------|:---------------|:-----------|
| افزونگی | Redundancy | اطلاعات اضافی که یا حذف می‌شود (منبع) یا اضافه می‌شود (کانال) |
| نرخ کد | Code Rate | \( R = k/n \) - نسبت بیت‌های اطلاعات به بیت‌های کدگذاری‌شده |
| مدولاسیون M-تایی | M-ary Modulation | ارسال \( b = \log_2 M \) بیت با هر سمبل |
| نویز گرمایی | Thermal Noise | نویز گاوسی ناشی از حرکت الکترون‌ها در قطعات |
| ISI | Inter-Symbol Interference | تداخل یک سمبل با سمبل‌های مجاور |
| محوشدگی | Fading | نوسان شدید توان سیگنال ناشی از چندمسیره |
| کدگذاری الحاقی | Concatenated Coding | ترکیب دو یا چند کد برای تصحیح خطاهای تصادفی و بسته‌ای |
| دیکدینگ نرم | Soft Decoding | استفاده از احتمال/log-likelihood به جای تصمیم سخت 0/1 |

</details>

---

## 📖 راهنمای مطالعه: چگونه از فصل ۱ بیشترین بهره را ببریم؟

### برای درک عمیق‌تر:

1. **مثال‌های شخصی بسازید:** یک پیام واقعی (مثل "فردا امتحان دارم") را مراحل کدگذاری منبع، کدگذاری کانال و مدولاسیون را روی آن پیاده‌سازی کنید (حداقل روی کاغذ).

2. **کانال‌های اطرافتان را شناسایی کنید:**
   - وقتی وای‌فای خانه افت می‌کند، مشکل کدام کانال است؟ (ISI؟ محوشدگی؟ نویز؟)
   - چرا در تونل صدای رادیو قطع می‌شود؟ (کانال فیلتر متغیر با زمان + محوشدگی)

3. **ارقام تاریخی را به خاطر بسپارید:**
   - 1837: تلگراف مورس
   - 1924: نرخ نایکوئیست
   - 1948: قضیه شانون
   - 1993: کدهای توربو

### اشتباهات رایج (که نباید انجام دهید):

| اشتباه | توضیح |
|:-------|:------|
| ❌ قاطی کردن کدگذاری منبع و کانال | منبع = حذف افزونگی، کانال = اضافه کردن افزونگی |
| ❌ فکر کردن "نویز بیشتر = حتماً افزایش توان" | گاهی افزایش پهنای باند یا کدگذاری بهتر جواب می‌دهد (شانون) |
| ❌ نادیده گرفتن نقش اینترلیور | بدون اینترلیور، کدهای تصحیح خطا در برابر خطای بسته‌ای بی‌اثرند |

---

## 🧩 نقشه راه پیشنهادی برای ادامه

بر اساس علاقه شما در فصل ۱، مسیرهای زیر را پیشنهاد می‌کنم:

| اگر به این بخش علاقه داشتید | بروید سراغ |
|:---------------------------|:-----------|
| **کدگذاری منبع (فشرده‌سازی)** | فصل ۶ (نظریه اطلاعات) + مطالعه کد هافمن و LZW |
| **کدگذاری کانال** | فصل ۷ (کدهای بلوکی) و فصل ۸ (کدهای تریلیس و گراف) |
| **مدولاسیون و دمودولاسیون** | فصل ۳ و ۴ |
| **کانال‌های بی‌سیم و محوشدگی** | فصل ۱۳ و ۱۴ |
| **تاریخچه مخابرات** | منابع خارجی: کتاب "The Information" اثر James Gleick |

---

## 🤔 سوالات تفکری (برای امتحان یا پروژه)

1. اگر کدگذار منبع نداشته باشیم، چه اتفاقی برای پهنای باند مورد نیاز می‌افتد؟
2. اگر کدگذار کانال نداشته باشیم، چه بلایی سر BER می‌آید؟
3. چرا در کانال فضای عمیق از BPSK استفاده می‌کنیم نه 64-QAM؟
4. فرض کنید یک کانال با SNR = -10 dB و پهنای باند 1 MHz داریم. حداکثر نرخ ممکن چقدر است؟ (از فرمول شانون استفاده کنید)
5. تفاوت بین "تصحیح خطا" در کدگذاری کانال و "جبران ISI" در یکسان‌سازی چیست؟

---

## 🔗 منابع خارجی پیشنهادی برای مطالعه بیشتر

| منبع | توضیح | لینک (جستجو کنید) |
|:-----|:------|:------------------|
| **3Blue1Brown - بیت‌ها، بایت‌ها و کدگذاری** | ویدیوی عالی برای درک شهودی کدگذاری | YouTube |
| **شانون - مقاله A Mathematical Theory of Communication** | مقاله اصلی 1948 (خواندنی تاریخی) | Bell Labs |
| **Deep Space Network (NASA)** | نحوه ارتباط با فضاپیماها | nasa.gov/dsn |
| **Brian Kernighan - Understanding the Digital World** | کتاب مقدماتی عالی برای درک مفاهیم پایه | فروشگاه‌های آنلاین |

---

## 📌 نکات پایانی (برای موفقیت در ادامه مسیر)

> 💪 **تمرین عملی پیشنهادی:** یک نرم‌افزار ساده بنویسید (در پایتون یا MATLAB) که:
> - یک پیام متنی ساده دریافت کند
> - آن را با کدگذاری منبع (مثلاً حذف فاصله‌های تکراری) فشرده کند
> - با یک کد کانال ساده (مثل تکرار هر بیت 3 بار) محافظت کند
> - نویز تصادفی اضافه کند
> - در گیرنده خطاها را تصحیح کند
>  
> این کار باعث می‌شود تمام بلوک‌های فصل 1 را عملاً تجربه کنید!

---

## 🎯 سنجش یادگیری (خودارزیابی)

خودتان را ارزیابی کنید:

| سؤال | بله | تا حدی | خیر |
|:-----|:---:|:------:|:---:|
| می‌توانم تفاوت کدگذاری منبع و کانال را توضیح دهم؟ | ☐ | ☐ | ☐ |
| می‌توانم مدل‌های سه‌گانه کانال (AWGN، فیلتر خطی، متغیر با زمان) را نام ببرم؟ | ☐ | ☐ | ☐ |
| فرمول شانون را می‌دانم و معنی نمادهایش را توضیح می‌دهم؟ | ☐ | ☐ | ☐ |
| می‌توانم یک مثال واقعی برای هر نوع کانال بزنم؟ | ☐ | ☐ | ☐ |
| می‌دانم چرا اینترلیور برای کدهای تصحیح خطا مهم است؟ | ☐ | ☐ | ☐ |
| قهرمانان اصلی تاریخ مخابرات دیجیتال و کشفشان را به خاطر دارم؟ | ☐ | ☐ | ☐ |

**اگر 4 سؤال اول «بله» است، آماده‌ای برای فصل 2!** 🚀

---

## ⏭️ پیش‌نمایش فصل ۲

در **فصل ۲** خواهیم خواند:

- نمایش سیگنال‌های میان‌گذر و پایین‌گذر (چگونه سیگنال RF را به باند پایه می‌بریم؟)
- نمایش فضای سیگنال: هر شکل موج را می‌توان به یک نقطه در فضای برداری تبدیل کرد
- متغیرهای تصادفی مفید: گاوسی، رایلی، رایسی، و توزیع‌های دیگر
- فرایندهای تصادفی و بسط کارهونن-لوو
- کران‌های احتمالاتی و قضایای حدی

**نکته:** فصل 2 به ظاهر ریاضی‌تر است، اما تمام فصول بعدی به آن وابسته هستند. صبور باشید و مفاهیم را با مثال‌های شهودی دنبال کنید!

---

> 📢 **نظر شما:** آیا بخش خاصی از فصل ۱ برایتان مبهم بود؟ کدام مثال بیشتر به درکتان کمک کرد؟ این بازخوردها به من کمک می‌کند فصل ۲ را بهتر برایتان طراحی کنم.

---

**فصل ۱ - پایان** ✅

**فصل ۱ تموم شد. بریم سراغ فصل ۲!** 🚀
