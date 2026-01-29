<div align="center">

# 📰 News Platform

### منصة إخبارية احترافية متعددة اللغات

<p align="center">
  <img src="https://img.shields.io/badge/Laravel-11-FF2D20?style=for-the-badge&logo=laravel&logoColor=white" alt="Laravel 11">
  <img src="https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React 18">
  <img src="https://img.shields.io/badge/PostgreSQL-15-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL">
  <img src="https://img.shields.io/badge/TypeScript-5-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript">
  <img src="https://img.shields.io/badge/Vite-5-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/TailwindCSS-3-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white" alt="Tailwind">
  <img src="https://img.shields.io/badge/Redis-Cache-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis">
  <img src="https://img.shields.io/badge/Cloudflare-CDN-F38020?style=flat-square&logo=cloudflare&logoColor=white" alt="Cloudflare">
  <img src="https://img.shields.io/badge/AI-Powered-00D9FF?style=flat-square&logo=openai&logoColor=white" alt="AI">
</p>

---

</div>

## ✨ نظرة عامة

منصة إخبارية شاملة ومتطورة مبنية باستخدام أحدث التقنيات، تدعم تعدد اللغات (RTL/LTR)، نظام إعلانات متقدم، وتكامل الذكاء الاصطناعي لتحسين جودة المحتوى.

### 🎯 المزايا الرئيسية

- 🌍 **تعدد اللغات** - دعم كامل للعربية والإنجليزية مع RTL/LTR
- 🤖 **ذكاء اصطناعي** - تلخيص تلقائي، تحسين SEO، واقتراح عناوين
- 📊 **نظام إعلانات متقدم** - إدارة شاملة للإعلانات مع جدولة وتتبع
- 🔐 **صلاحيات متعددة** - Super Admin, Admin, Editor, Ads Manager
- 🎨 **Dark/Light Mode** - واجهة قابلة للتخصيص
- 📱 **Responsive Design** - تصميم متجاوب بالكامل
- ⚡ **أداء عالي** - Redis Cache, CDN, Lazy Loading
- 🔍 **بحث متقدم** - Full-text search مع PostgreSQL

---

## 🏗️ البنية التقنية

### Backend Stack

```
🔧 Laravel 11           - PHP Framework
🗄️ PostgreSQL          - Database (JSON Fields, Full-text Search)
🔒 Sanctum              - SPA Authentication
⚡ Redis                - Caching & Queues
📦 AWS S3/DO Spaces     - Media Storage
🤖 OpenAI API           - AI Integration
📧 Firebase Auth        - Phone Verification
```

### Frontend Stack

```
⚛️ React 18             - UI Library
📘 TypeScript           - Type Safety
⚡ Vite 5               - Build Tool
🎨 TailwindCSS          - Styling
🔄 Redux Toolkit        - State Management
🌐 React Router         - Navigation
🎭 React Query          - Data Fetching
🌍 i18next              - Internationalization
```

### DevOps & Infrastructure

```
🌐 Nginx                - Web Server
🔐 Let's Encrypt        - SSL Certificate
☁️ Cloudflare           - CDN & Security
🚀 GitHub Actions       - CI/CD
📊 Sentry/Bugsnag       - Error Tracking
👷 Supervisor           - Queue Management
```

---

## 📂 هيكلة المشروع

<details>
<summary><b>📁 Backend Structure (Laravel)</b></summary>

```
app/
├── Actions/              # Business Logic Actions
├── DTOs/                 # Data Transfer Objects
├── Services/             # Service Layer
│   ├── ArticleService/
│   ├── CategoryService/
│   ├── AdService/
│   └── AIService/
├── Repositories/         # Data Access Layer
│   └── Interfaces/
├── Http/
│   ├── Controllers/
│   │   ├── API/V1/
│   │   │   ├── Auth/
│   │   │   ├── Admin/
│   │   │   └── Public/
│   ├── Requests/         # Form Validation
│   ├── Resources/        # API Resources
│   └── Middleware/
├── Policies/             # Authorization
├── Jobs/                 # Queue Jobs
├── Events/               # Domain Events
├── Listeners/            # Event Handlers
├── Exceptions/           # Custom Exceptions
└── Models/
```

</details>

<details>
<summary><b>⚛️ Frontend Structure (React)</b></summary>

```
resources/js/
├── app/                  # App Entry
├── components/           # Reusable Components
│   ├── ui/              # UI Components
│   ├── common/          # Common Components
│   └── layouts/         # Layout Components
├── features/            # Feature Modules
│   ├── articles/
│   ├── categories/
│   ├── ads/
│   └── auth/
├── pages/               # Page Components
│   ├── HomePage.jsx
│   ├── ArticleDetailsPage.jsx
│   ├── CategoryPage.jsx
│   └── admin/
│       ├── DashboardPage.jsx
│       ├── ManageArticlesPage.jsx
│       └── ManageAdsPage.jsx
├── services/            # API Services
│   ├── api.js
│   ├── articleService.js
│   └── authService.js
├── hooks/               # Custom Hooks
├── store/               # Redux Store
├── utils/               # Utilities
├── i18n/                # Translations
└── styles/              # Global Styles
```

</details>

---

## 🗄️ قاعدة البيانات

### الجداول الرئيسية

| الجدول | الوصف |
|--------|-------|
| `users` | المستخدمين والصلاحيات |
| `articles` | الأخبار والمقالات |
| `categories` | الأقسام (قابلة للتفعيل/التعطيل/الترتيب) |
| `tags` | الوسوم |
| `comments` | التعليقات مع Moderation |
| `ads` | الإعلانات المتقدمة |
| `ad_positions` | مواضع الإعلانات |
| `media` | الملفات والصور |
| `languages` | اللغات المدعومة |
| `settings` | إعدادات النظام |
| `views` | إحصائيات المشاهدات |
| `logs` | السجلات والتتبع |

<details>
<summary><b>📊 عرض Schema الكامل</b></summary>

```sql
-- Users & Permissions
users (id, name, email, phone, role_id, is_active, ...)
roles (id, name, slug, permissions JSONB, ...)
permissions (id, name, slug, group, ...)

-- Content Management
articles (
  id, title JSONB, slug, content JSONB, excerpt JSONB,
  category_id, user_id, status, is_featured, is_breaking,
  published_at, views_count, meta JSONB, ...
)

categories (
  id, name JSONB, slug, parent_id, position,
  is_active, show_in_header, show_in_homepage,
  layout_type, meta JSONB, ...
)

tags (id, name JSONB, slug, usage_count, ...)
article_tag (article_id, tag_id)

-- Comments System
comments (
  id, article_id, user_id, content,
  parent_id, is_approved, is_flagged, ...
)

-- Advanced Ads System
ads (
  id, title, type, content JSONB,
  position_id, priority, is_active,
  start_date, end_date, 
  target_languages JSONB, target_devices JSONB,
  target_pages JSONB, impressions, clicks, ...
)

ad_positions (
  id, name, slug, location,
  max_ads, dimensions JSONB, ...
)

-- Media & Assets
media (
  id, filename, path, type, size,
  alt_text JSONB, is_public, user_id, ...
)

-- System
languages (id, name, code, direction, is_active, ...)
settings (key, value JSONB, type, group, ...)
views (article_id, ip, user_id, viewed_at, ...)
logs (level, message, context JSONB, created_at, ...)
```

**مزايا JSONB:**
- ✅ تخزين محتوى متعدد اللغات بكفاءة
- ✅ Metadata مرنة
- ✅ Indexing سريع
- ✅ Querying متقدم

</details>

---

## 🚀 البدء السريع

### المتطلبات

```bash
PHP >= 8.3
Composer
Node.js >= 20
PostgreSQL >= 15
Redis
```

### التثبيت

<details>
<summary><b>1️⃣ استنساخ المشروع</b></summary>

```bash
git clone https://github.com/hamzatal/news-platform.git
cd news-platform
```

</details>

<details>
<summary><b>2️⃣ Backend Setup</b></summary>

```bash
# Install dependencies
composer install

# Copy environment file
cp .env.example .env

# Generate app key
php artisan key:generate

# Configure database in .env
DB_CONNECTION=pgsql
DB_HOST=127.0.0.1
DB_PORT=5432
DB_DATABASE=news_platform
DB_USERNAME=postgres
DB_PASSWORD=your_password

# Run migrations
php artisan migrate

# Seed database (optional)
php artisan db:seed

# Link storage
php artisan storage:link
```

</details>

<details>
<summary><b>3️⃣ Frontend Setup</b></summary>

```bash
# Install dependencies
npm install

# Run development server
npm run dev
```

</details>

<details>
<summary><b>4️⃣ تشغيل المشروع</b></summary>

```bash
# Terminal 1: Laravel
php artisan serve

# Terminal 2: Vite
npm run dev

# Terminal 3: Queue Worker
php artisan queue:work

# Terminal 4: Redis (if not running as service)
redis-server
```

</details>

**🌐 الوصول للتطبيق:**
- Frontend: `http://localhost:5173`
- API: `http://localhost:8000/api/v1`

---

## 🔐 المصادقة والصلاحيات

### نظام الأدوار

| الدور | الصلاحيات |
|------|-----------|
| **Super Admin** | تحكم كامل بالنظام، الإعدادات، المستخدمين |
| **Admin** | إدارة المحتوى، الأقسام، التعليقات |
| **Editor** | كتابة ونشر الأخبار |
| **Ads Manager** | إدارة الإعلانات فقط |

### المصادقة

```javascript
// Login
POST /api/v1/auth/login
{
  "email": "user@example.com",
  "password": "password"
}

// Register
POST /api/v1/auth/register
{
  "name": "User Name",
  "email": "user@example.com",
  "password": "password",
  "password_confirmation": "password"
}

// Email Verification
GET /api/v1/auth/verify-email/{id}/{hash}

// Phone Verification (Firebase)
POST /api/v1/auth/verify-phone
{
  "phone": "+962XXXXXXXXX",
  "verification_code": "123456"
}
```

---

## 📱 نظام الإعلانات

### أنواع الإعلانات

- 🎯 **Header Banner** - أعلى الصفحة
- 📰 **Between Articles** - بين الأخبار
- 📌 **Sidebar Ads** - الشريط الجانبي
- 📑 **In-Article** - داخل المقال
- 🚀 **Popup** - نافذة منبثقة
- 🎬 **Fullscreen** - ملء الشاشة
- ⭐ **Sponsored Articles** - مقالات ممولة

### مزايا الإعلانات

```javascript
✅ تفعيل/تعطيل
✅ جدولة (تاريخ بداية ونهاية)
✅ أولوية العرض
✅ استهداف حسب:
   - اللغة
   - الجهاز (Mobile/Desktop)
   - الصفحات
✅ تتبع (المشاهدات والنقرات)
```

---

## 🤖 تكامل الذكاء الاصطناعي

### المزايا المدعومة

| الميزة | الوصف |
|-------|-------|
| 📝 **تلخيص تلقائي** | إنشاء ملخص للخبر |
| 💡 **اقتراح عناوين** | عناوين جذابة وفعالة |
| 🔍 **تحسين SEO** | Meta tags, keywords |
| 🔄 **كشف التكرار** | تجنب الأخبار المكررة |
| 🏷️ **تصنيف تلقائي** | اقتراح الفئة المناسبة |
| #️⃣ **اقتراح وسوم** | Tags ذكية |
| ✍️ **تدقيق لغوي** | عربي وإنجليزي |

### مثال استخدام

```php
// في ArticleService
public function enhanceWithAI(Article $article): array
{
    return [
        'summary' => $this->aiService->generateSummary($article->content),
        'seo_title' => $this->aiService->suggestSEOTitle($article->title),
        'keywords' => $this->aiService->extractKeywords($article->content),
        'category' => $this->aiService->suggestCategory($article->content),
        'tags' => $this->aiService->suggestTags($article->content),
    ];
}
```

---

## 🔍 البحث المتقدم

```sql
-- PostgreSQL Full-Text Search
SELECT * FROM articles
WHERE to_tsvector('arabic', title->>'ar') @@ plainto_tsquery('arabic', 'كلمة البحث')
   OR to_tsvector('english', title->>'en') @@ plainto_tsquery('english', 'search term');
```

**البحث حسب:**
- 📰 العنوان
- 📝 المحتوى
- 🏷️ الوسوم
- 📂 القسم
- 📅 التاريخ
- ⭐ الكاتب

---

## 🎨 الواجهات

### الصفحة الرئيسية

```
┌─────────────────────────────────────────┐
│  Header (Navigation + Breaking News)   │
├─────────────────────────────────────────┤
│                                         │
│  Hero Section (Main News + Slider)     │
│                                         │
├─────────────────────────────────────────┤
│  Categories Grid / List                │
├─────────────────────────────────────────┤
│  Latest News + Sidebar Ads             │
├─────────────────────────────────────────┤
│  Most Viewed | Trending                │
├─────────────────────────────────────────┤
│  Footer (Links + Social + Newsletter)  │
└─────────────────────────────────────────┘
```

### لوحة التحكم

- 📊 **Dashboard** - إحصائيات شاملة
- 📰 **إدارة الأخبار** - CRUD كامل
- 📂 **إدارة الأقسام** - ترتيب وتفعيل
- 💬 **إدارة التعليقات** - Moderation
- 📱 **إدارة الإعلانات** - Ads Manager
- 👥 **إدارة المستخدمين** - Roles & Permissions
- ⚙️ **الإعدادات** - System Settings

---

## 🌍 تعدد اللغات

### اللغات المدعومة

- 🇸🇦 العربية (RTL)
- 🇬🇧 English (LTR)

### التطبيق

```javascript
// React Component
import { useTranslation } from 'react-i18next';

function Component() {
  const { t, i18n } = useTranslation();
  
  return (
    <div dir={i18n.dir()}>
      <h1>{t('home.welcome')}</h1>
    </div>
  );
}
```

```php
// Laravel Blade
{{ __('messages.welcome') }}
```

---

## 🔧 APIs الخارجية

### 🌤️ Weat API

```javascript
// OpenWeatherMap Integration
const weather = await fetch(
  `https://api.openweathermap.org/data/2.5/weather?q=${city}&appid=${API_KEY}`
);
```

### 📰 World News

```javascript
// NewsAPI Integration
const news = await fetch(
  `https://newsapi.org/v2/top-headlines?country=us&apiKey=${API_KEY}`
);
```

**Cache Strategy:**
- ⏱️ تحديث كل 15-30 دقيقة
- 💾 Redis Cache
- 🔄 Background Jobs

---

## 🚀 النشر (Deployment)

### Production Stack

```
Domain: Namecheap/GoDaddy
Server: DigitalOcean Droplet (2GB RAM)
OS: Ubuntu 22.04 LTS
Web Server: Nginx
SSL: Let's Encrypt
CDN: Cloudflare
```

### خطوات النشر

<details>
<summary><b>1️⃣ إعداد السيرفر</b></summary>

```bash
# Update system
sudo apt update && sudo apt upgrade -y

# Install Nginx
sudo apt install nginx -y

# Install PHP 8.3
sudo apt install php8.3-fpm php8.3-pgsql php8.3-redis php8.3-mbstring php8.3-xml php8.3-curl -y

# Install PostgreSQL
sudo apt install postgresql postgresql-contrib -y

# Install Redis
sudo apt install redis-server -y

# Install Supervisor
sudo apt install supervisor -y
```

</details>

<details>
<summary><b>2️⃣ Deploy Code</b></summary>

```bash
# Clone repository
git clone https://github.com/hamzatal/news-platform.git /var/www/news-platform
cd /var/www/news-platform

# Install dependencies
composer install --optimize-autoloader --no-dev
npm install && npm run build

# Set permissions
sudo chown -R www-data:www-data /var/www/news-platform
sudo chmod -R 755 /var/www/news-platform/storage

# Run migrations
php artisan migrate --force

# Optimize
php artisan config:cache
php artisan route:cache
php artisan view:cache
```

</details>

<details>
<summary><b>3️⃣ Configure Nginx</b></summary>

```nginx
server {
    listen 80;
    server_name example.com;
    root /var/www/news-platform/public;

    add_header X-Frame-Options "SAMEORIGIN";
    add_header X-Content-Type-Options "nosniff";

    index index.php;

    charset utf-8;

    location / {
        try_files $uri $uri/ /index.php?$query_string;
    }

    location ~ \.php$ {
        fastcgi_pass unix:/var/run/php/php8.3-fpm.sock;
        fastcgi_param SCRIPT_FILENAME $realpath_root$fastcgi_script_name;
        include fastcgi_params;
    }

    location ~ /\.(?!well-known).* {
        deny all;
    }
}
```

</details>

<details>
<summary><b>4️⃣ SSL Setup</b></summary>

```bash
# Install Certbot
sudo apt install certbot python3-certbot-nginx -y

# Get SSL certificate
sudo certbot --nginx -d example.com -d www.example.com

# Auto-renewal
sudo certbot renew --dry-run
```

</details>

<details>
<summary><b>5️⃣ Queue Worker</b></summary>

```ini
# /etc/supervisor/conf.d/laravel-worker.conf
[program:laravel-worker]
process_name=%(program_name)s_%(process_num)02d
command=php /var/www/news-platform/artisan queue:work --sleep=3 --tries=3
autostart=true
autorestart=true
user=www-data
numprocs=2
redirect_stderr=true
stdout_logfile=/var/www/news-platform/storage/logs/worker.log
```

```bash
sudo supervisorctl reread
sudo supervisorctl update
sudo supervisorctl start laravel-worker:*
```

</details>

---

## 📊 الأداء والتحسين

### استراتيجيات Cache

```php
// Cache Categories
Cache::remember('categories.active', 3600, function () {
    return Category::where('is_active', true)
        ->orderBy('position')
        ->get();
});

// Cache Articles
Cache::tags(['articles'])->remember("article.{$id}", 3600, function () use ($id) {
    return Article::with('category', 'tags', 'media')->find($id);
});
```

### Database Optimization

```sql
-- Indexes
CREATE INDEX idx_articles_published ON articles(published_at DESC);
CREATE INDEX idx_articles_category ON articles(category_id);
CREATE INDEX idx_articles_status ON articles(status);

-- Full-Text Search
CREATE INDEX idx_articles_title_ar ON articles USING gin(to_tsvector('arabic', title->>'ar'));
CREATE INDEX idx_articles_title_en ON articles USING gin(to_tsvector('english', title->>'en'));
```

### Frontend Optimization

- ⚡ **Code Splitting** - React.lazy()
- 🖼️ **Lazy Loading** - للصور والمكونات
- 📦 **Bundle Optimization** - Vite Tree-shaking
- 🗜️ **Compression** - Gzip/Brotli
- 🌐 **CDN** - Cloudflare للأصول الثابتة

---

## 🧪 الاختبار

```bash
# Backend Tests
php artisan test

# Frontend Tests
npm run test

# E2E Tests
npm run test:e2e

# Coverage
php artisan test --coverage
```

---

## 📈 المراقبة والأخطاء

### Error Tracking

```php
// Sentry Integration
if (app()->bound('sentry')) {
    app('sentry')->captureException($exception);
}
```

### Logs

```bash
storage/logs/
├── laravel.log          # Application logs
├── worker.log           # Queue worker logs
├── nginx-access.log     # Web server access
└── nginx-error.log      # Web server errors
```

---

## 🛡️ الأمان

### Best Practices

- ✅ **HTTPS Only** - SSL إلزامي
- ✅ **CSRF Protection** - Laravel built-in
- ✅ **XSS Prevention** - Input sanitization
- ✅ **SQL Injection** - Eloquent ORM
- ✅ **Rate Limiting** - API throttling
- ✅ **File Upload Validation** - Type & size checks
- ✅ **Password Hashing** - Bcrypt
- ✅ **2FA** - Phone verification

### Cloudflare Security

```
✓ DDoS Protection
✓ Web Application Firewall
✓ Bot Management
✓ SSL/TLS Encryption
✓ Rate Limiting
```

---

## 🤝 المساهمة

نرحب بالمساهمات! يرجى اتباع الخطوات:

1. Fork المشروع
2. إنشاء فرع للميزة (`git checkout -b feature/AmazingFeature`)
3. Commit التغييرات (`git commit -m 'Add some AmazingFeature'`)
4. Push للفرع (`git push origin feature/AmazingFeature`)
5. فتح Pull Request

### معايير الكود

- ✅ PSR-12 للـ PHP
- ✅ ESLint للـ JavaScript/TypeScript
- ✅ مسح الاختبارات
- ✅ توثيق واضح

---

## 📝 الترخيص

هذا المشروع مرخص تحت [MIT License](LICENSE)

---

## 👥 الفريق

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/hamzatal">
        <img src="https://github.com/hamzatal.png" width="100px;" alt=""/>
        <br />
        <sub><b>Your Name</b></sub>
      </a>
      <br />
      <sub>Lead Developer</sub>
    </td>
    <!-- Add more team members -->
  </tr>
</table>

---

## 📞 التواصل

- 📧 Email: contact@newsplatform.com
- 🌐 Website: https://newsplatform.com
- 💬 Discord: [Join our server](https://discord.gg/newsplatform)

---

## 🙏 شكر وتقدير

- [Laravel](https://laravel.com) - PHP Framework
- [React](https://react.dev) - UI Library
- [PostgreSQL](https://postgresql.org) - Database
- [TailwindCSS](https://tailwindcss.com) - CSS Framework
- [OpenAI](https://openai.com) - AI Integration
- [Cloudflare](https://cloudflare.com) - CDN & Security

---

<div align="center">

### صُنع بـ ❤️ للصحافة العربية

**[⬆ العودة للأعلى](#-news-platform)**

</div>
