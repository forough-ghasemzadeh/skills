# Iranian Corporate Resignation Legal Skills

مجموعه‌ای از AI Skills تخصصی برای **تحلیل و تنظیم اسناد مرتبط با استعفای مدیران شرکت‌ها در حقوق ایران**.

این مجموعه در حال حاضر بر دو قالب شرکت تمرکز دارد:

- شرکت با مسئولیت محدود
- شرکت سهامی خاص

## قابلیت‌ها

این Skills می‌توانند در موارد زیر کمک کنند:

- تحلیل وضعیت حقوقی استعفا
- تفکیک استعفا از سمت و عضویت
- بررسی آثار استعفا
- بررسی جانشینی مدیران
- بررسی الزامات ثبت تغییرات
- بررسی آثار ثبتی و رسمی تغییر سمت
- شناسایی ریسک‌های حقوقی
- تنظیم استعفانامه، اظهارنامه و صورتجلسات مرتبط

> این پروژه یک ابزار کمک‌حقوقی است و جایگزین بررسی و نظر حقوقی متخصص واجد صلاحیت نیست.

## نصب

این مخزن با فرمت استاندارد [Agent Skills](https://agentskills.io/specification) سازگار است و هر Skill شامل یک `SKILL.md` با frontmatter معتبر است. بسته به ابزاری که استفاده می‌کنید، یکی از روش‌های زیر را انتخاب کنید.

### روش ۱: در Claude.ai و Claude Desktop (توصیه‌شده)

Claude.ai و Claude Desktop (پلن‌های Pro، Max، Team و Enterprise) امکان آپلود مستقیم Skills سفارشی را دارند — بدون نیاز به هیچ دانش فنی:

1. پوشهٔ Skill مورد نظر را به‌صورت zip فشرده کنید، طوری که `SKILL.md` مستقیماً در ریشهٔ فایل zip قرار بگیرد (نه داخل یک پوشهٔ میانی):

   ```bash
   cd companies/private-joint-stock/resignation && zip -r ../../../private-joint-stock-resignation-skill.zip . && cd -
   cd companies/limited-liability/resignation && zip -r ../../../limited-liability-resignation-skill.zip . && cd -
   ```

   (اگر با خط فرمان راحت نیستید، می‌توانید از یک همکار فنی بخواهید این مرحله را برایتان انجام دهد.)

2. در Claude.ai یا Claude Desktop به مسیر **Settings → Capabilities → Skills** (یا Customize → Skills) بروید.
3. روی «+ Create skill» کلیک کرده و فایل zip را آپلود کنید.
4. در گفتگوی جدید، Skill را فعال کنید و پرسش خود را به زبان فارسی و طبیعی مطرح کنید.

### روش ۲: در ChatGPT (به‌صورت دستی)

ChatGPT هنوز امکان آپلود مستقیم فایل Skill را ندارد. برای استفاده در یک Custom GPT یا Project:

1. محتوای فایل `SKILL.md` Skill مورد نظر (و در صورت وجود، فایل‌های داخل `references/`) را باز کنید.
2. کل متن را در بخش Instructions مربوط به Custom GPT یا Project کپی کنید.

### روش ۳: با ابزارهای برنامه‌نویسی (اختیاری، برای کاربران فنی)

اگر تیم شما از ابزارهایی مانند Claude Code یا Hermes Agent استفاده می‌کند، می‌توان این Skills را با [`npx skills`](https://github.com/vercel-labs/skills) نیز نصب کرد:

```bash
npx skills add forough-ghasemzadeh/skills
```

### روش ۴: به‌صورت Plugin در Claude Code

این مخزن یک [Claude Code plugin marketplace](https://code.claude.com/docs/en/plugin-marketplaces) نیز هست و هر دو Skill را در یک پلاگین واحد (`iranian-corporate-resignation`) عرضه می‌کند. در Claude Code:

```
/plugin marketplace add forough-ghasemzadeh/skills
/plugin install iranian-corporate-resignation@ghasemzadeh-skills
```

پس از نصب، در صورت نیاز `/reload-plugins` را اجرا کنید. Skillها به‌صورت `iranian-corporate-resignation:limited-liability-resignation` و `iranian-corporate-resignation:private-joint-stock-resignation` در دسترس‌اند و همچنان بر اساس محتوای گفتگو به‌صورت خودکار توسط مدل نیز فعال می‌شوند.

> توجه: این روش برای **Claude Code** (ابزار خط‌فرمان) است. برنامهٔ Claude Desktop در حال حاضر مفهوم «Plugin» ندارد و Skills سفارشی را فقط به‌صورت فایل zip (روش ۱) می‌پذیرد.

## استفاده

پس از نصب، Skill مناسب را در محیط AI خود فعال یا معرفی کنید و درخواست خود را به زبان طبیعی وارد کنید.

برای مثال:

```text
من مدیرعامل و شریک یک شرکت با مسئولیت محدود هستم و
می‌خواهم فقط از سمت مدیرعاملی استعفا بدهم و همچنان
شریک شرکت باقی بمانم.
```
