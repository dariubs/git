<div dir="rtl">

# راهنمای گیت

یک کتاب کوچک فارسی برای یادگیری گیت — از پایه تا پیشرفته.

🌐 **نسخه آنلاین:** [dariubs.github.io/git](https://dariubs.github.io/git/)

---

## درباره پروژه

این پروژه یک راهنمای فارسی برای یادگیری سیستم کنترل نسخه **Git** است. مطالب به‌صورت کتابی ساختاریافته نوشته شده‌اند و تمام مفاهیم پایه تا پیشرفته گیت را به زبان ساده توضیح می‌دهند.

### سرفصل‌ها

- مدیریت کد منبع و معرفی گیت
- نصب و پیکربندی
- `init` و `clone`
- `add`, `commit`, `status`, `diff`
- `log` و `.gitignore`
- `branch` و `merge`
- `remote` و میزبان‌های گیت
- بازگرداندن تغییرات
- `tag`, `stash`, `rebase`
- `cherry-pick` و `blame`
- نکات و ترفندها

---

## پیش‌نیازها

- [Hugo](https://gohugo.io/installation/) (نسخه extended)
- [Node.js](https://nodejs.org/) (برای Tailwind CSS)

---

## اجرای محلی

```bash
git clone https://github.com/dariubs/git.git
cd git
npm install
npm run build:css
hugo server
```

سایت روی آدرس `http://localhost:1313` در دسترس خواهد بود.

برای توسعه همزمان CSS و Hugo:

```bash
npm run dev:css

# in another terminal
hugo server
```

---

## مشارکت

خوشحال می‌شیم که در بهبود این کتاب مشارکت کنید — چه ویرایش محتوا، چه اضافه کردن فصل جدید، چه رفع اشتباهات تایپی.

### مراحل مشارکت

1. مخزن را Fork کنید
2. یک branch جدید بسازید:
   ```bash
   git checkout -b fix/typo-in-branch-chapter
   ```
3. تغییرات خود را اعمال کنید
4. Commit بزنید:
   ```bash
   git commit -m "fix: اصلاح اشتباه تایپی در فصل branch"
   ```
5. Push کنید و یک Pull Request باز کنید

### افزودن فصل جدید

فایل‌های محتوا در پوشه `content/book/` قرار دارند. برای اضافه کردن فصل جدید:

```bash
# مثال: فصل ۲۳
touch content/book/23.new-topic.md
```

ساختار هر فایل:

```markdown
---
title: "عنوان فصل"
weight: 23
---

محتوای فصل...
```

### نکات مشارکت

- متن را به فارسی روان و ساده بنویسید
- از مثال‌های عملی و کاربردی استفاده کنید
- برای کدها از کد بلوک‌های مناسب استفاده کنید

---

## ساختار پروژه

```
.
├── content/
│   └── book/          # فصل‌های کتاب (فایل‌های Markdown)
├── themes/
│   └── gitbook-fa/    # تم اختصاصی سایت
├── assets/
│   └── css/           # فایل‌های CSS (Tailwind)
├── static/            # فایل‌های استاتیک
└── hugo.toml          # تنظیمات Hugo
```

---

## لایسنس

این پروژه تحت لایسنس [MIT](LICENSE) منتشر شده است.

---

نوشته شده با ❤️ توسط [داریوش عباسی](https://dariush.in)

</div>
