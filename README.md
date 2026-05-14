# 🌑 Жизнь на бис — Сайт Елены Дорохиной

Сайт для продажи книги «Жизнь на бис». Работает прямо с GitHub Pages — **бесплатно, без хостинга**.

---

## 🚀 КАК ЗАПУСТИТЬ НА GitHub Pages (шаг за шагом)

### Шаг 1 — Создайте аккаунт GitHub
Если нет — зарегистрируйтесь на [github.com](https://github.com)

### Шаг 2 — Создайте репозиторий
1. Нажмите кнопку **"New repository"** (зелёная, вверху)
2. Название: `zhizn-na-bis` (или любое другое)
3. Сделайте **Public** (обязательно для GitHub Pages бесплатного)
4. Нажмите **"Create repository"**

### Шаг 3 — Загрузите файлы
Самый простой способ — через браузер:
1. Нажмите **"uploading an existing file"** или **"Add file → Upload files"**
2. Перетащите **ВСЕ файлы** из папки проекта:
   - `index.html`
   - `admin/` (папку целиком)
   - `assets/` (папку целиком)
   - `_data/` (папку целиком)
   - `.nojekyll`
3. Нажмите **"Commit changes"**

### Шаг 4 — Включите GitHub Pages
1. В репозитории → **Settings** → **Pages** (слева)
2. Source: **"Deploy from a branch"**
3. Branch: **main** → **/root**
4. Нажмите **Save**

**Через 2-3 минуты сайт будет доступен по адресу:**
```
https://YOUR_USERNAME.github.io/zhizn-na-bis/
```

---

## 📸 КАК ДОБАВИТЬ ФОТОГРАФИИ

После того как сайт запущен, добавьте фото:

1. В репозитории перейдите в папку `assets/images/`
2. Нажмите **"Add file → Upload files"**
3. Загрузите фото с такими именами:

| Файл | Что это |
|------|---------|
| `elena.jpg` | Главное фото Елены (600×800px, вертикальное) |
| `about-photo.jpg` | Второе фото / силуэт (600×800px) |
| `page3.jpg` | 3-я страница книги |
| `back-cover.jpg` | Задняя обложка |
| `cert1.jpg` ... `cert5.jpg` | Сертификаты |

4. После загрузки — откройте `index.html` в репозитории
5. Нажмите карандаш (редактировать)
6. Найдите комментарии `📸 ФОТО` и замените плейсхолдеры на `<img>` теги

---

## 📲 КАК ВСТАВИТЬ ССЫЛКИ (Telegram, соцсети, цена)

Откройте `index.html` и найдите/замените:

| Что заменить | На что |
|---|---|
| `YOUR_TELEGRAM_BUY_URL` | Ссылка на Telegram для покупки книги |
| `YOUR_TELEGRAM_CHANNEL` | Ссылка на ваш Telegram канал/клуб |
| `YOUR_TELEGRAM_CLUB_PAY_URL` | Ссылка на оплату клуба |
| `YOUR_INSTAGRAM_URL` | Ваш Instagram |
| `YOUR_YOUTUBE_URL` | Ваш YouTube |
| `YOUR_LINKEDIN_URL` | Ваш LinkedIn |
| `YOUR_PHONE` | Номер для WhatsApp (только цифры) |
| `YOUR_EMAIL` | Ваш email |
| `5 500 ₽` | Реальная цена книги |
| `1 500 ₽` | Реальная цена клуба |

---

## ✏️ КАК РЕДАКТИРОВАТЬ ТЕКСТЫ САМОСТОЯТЕЛЬНО (CMS)

Сайт включает **Decap CMS** — удобная панель управления в браузере.

### Настройка CMS (один раз):

**Вариант А — через Netlify (рекомендуется, проще всего):**
1. Зарегистрируйтесь на [netlify.com](https://netlify.com) — бесплатно
2. New site → Import from Git → выберите ваш GitHub репозиторий
3. Netlify сам опубликует сайт
4. В Netlify: Site settings → Identity → Enable Identity
5. Registration: **Invite only**
6. Git Gateway → Enable Git Gateway
7. Identity → Invite users → введите свой email
8. Перейдите на `https://ВАШ-САЙТ.netlify.app/admin/`
9. Войдите через email — и редактируйте сайт!

**Вариант Б — через GitHub Pages (чуть сложнее):**
1. Откройте `admin/config.yml`
2. Замените `YOUR_GITHUB_USERNAME/YOUR_REPO_NAME` на реальные данные
3. OAuth proxy уже настроен (`sveltia-cms-auth.pages.dev`)
4. Откройте `https://ВАША-ССЫЛКА/admin/` — войдите через GitHub

---

## 📁 СТРУКТУРА ФАЙЛОВ

```
zhizn-na-bis/
├── index.html          ← Главная страница сайта
├── .nojekyll           ← Отключает Jekyll (нужен для GitHub Pages)
├── admin/
│   ├── index.html      ← CMS панель управления
│   └── config.yml      ← Настройки CMS (что редактировать)
├── assets/
│   └── images/         ← Все фотографии сюда
│       ├── cover.png   ← Обложка книги (уже есть!)
│       ├── elena.jpg   ← Добавить: фото автора
│       └── ...
└── _data/
    └── settings.json   ← Данные сайта
```

---

## 🎨 ЦВЕТОВАЯ ПАЛИТРА (для дизайнера)

```css
--bg:         #080706   /* Основной фон */
--gold:       #c8860a   /* Золотой */
--gold-bright:#f5c832   /* Яркое золото */
--orange:     #e8621a   /* Оранжевый */
--corona:     #ffd050   /* Корона затмения */
--cream:      #fff5e0   /* Текст */
```

---

## ❓ ПОДДЕРЖКА

Если что-то не работает — напишите разработчику.
