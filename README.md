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

این مخزن با فرمت [Agent Skills](https://agentskills.io/specification) سازگار است و از طریق [`npx skills`](https://github.com/vercel-labs/skills) قابل نصب است:

```bash
# مشاهده Skills موجود در این مخزن
npx skills add forough-ghasemzadeh/skills --list

# نصب همه Skills
npx skills add forough-ghasemzadeh/skills

# نصب فقط یک Skill مشخص
npx skills add forough-ghasemzadeh/skills --skill resignation
npx skills add forough-ghasemzadeh/skills --skill private-joint-stock

# نصب برای یک ابزار مشخص (مثلاً Claude Code)
npx skills add forough-ghasemzadeh/skills -a claude-code
```

`npx skills` در حال حاضر ابزارهایی مانند Claude Code، Cursor، Codex و OpenCode را پشتیبانی می‌کند. برای **ChatGPT** که هنوز به این CLI متصل نیست، محتوای فایل `SKILL.md` مربوطه (به‌همراه فایل‌های `references/`) را در Custom GPT Instructions یا Project Instructions کپی کنید.

## استفاده

پس از نصب، Skill مناسب را در محیط AI خود فعال یا معرفی کنید و درخواست خود را به زبان طبیعی وارد کنید.

برای مثال:

```text
من مدیرعامل و شریک یک شرکت با مسئولیت محدود هستم و
می‌خواهم فقط از سمت مدیرعاملی استعفا بدهم و همچنان
شریک شرکت باقی بمانم.
```
