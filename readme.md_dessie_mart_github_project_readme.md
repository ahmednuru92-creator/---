# 🇪🇹 ደሴ ማርት (Dessie Mart / ሙጋድ ገበያ)

> **የደሴ ከተማ እና የደቡብ ወሎ ዘመናዊ የሞባይል ኢ-ኮሜርስ፣ የኪራይ/ሽያጭ፣ የተገላቢጦሽ ጨረታ (Reverse Bidding / RFQ) እና የዲጂታል ክፍያ መድረክ**

[![Flutter](https://img.shields.io/badge/Flutter-3.19.x-02569B?logo=flutter)](https://flutter.dev)
[![Node.js](https://img.shields.io/badge/Node.js-20.x-339933?logo=node.js)](https://nodejs.org)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16.0-4169E1?logo=postgresql)](https://postgresql.org)
[![Telebirr](https://img.shields.io/badge/Telebirr-SuperApp_API-007ACC)](https://telebirr.et)
[![CBE Birr](https://img.shields.io/badge/CBE_Birr-WebPay_API-800080)](https://cbe.com.et)
[![Telegram Bot](https://img.shields.io/badge/@DessieMarket-Automated_Bot-26A5E4?logo=telegram)](https://t.me/DessieMarket)
[![License](https://img.shields.io/badge/License-Proprietary-red.svg)](#)

---

## 📌 1. ስለ ፕሮጀክቱ አጠቃላይ እይታ (About Dessie Mart)

**ደሴ ማርት (Dessie Mart / ሙጋድ ገበያ)** በታሪካዊቷ ደሴ ከተማ እና በደቡብ ወሎ ዙሪያ ያሉ ነጋዴዎችን፣ ድርጅቶችን፣ ተከራዮችን፣ ገዢዎችን እና አቅራቢዎችን የሚያስተሳስር ዘመናዊ መድረክ ነው። 

መተግበሪያው በተለይ ለኢትዮጵያ ገበያ ምቹ በሆነ **100% የአማርኛ በይነገጽ**፣ በኢትዮ ቴሌኮም **ቴሌብር (Telebirr)** እና በ**ኢትዮጵያ ንግድ ባንክ (CBE Birr)** ቀጥታ ኤፒአይ ትስስር፣ በውስጠ-መተግበሪያ ዲጂታል ዋሌት (In-App Wallet) እና አውቶሜትድ በሆነ የቴሌግራም ቻናል ስርጭት (**`@DessieMarket`**) የተገነባ ነው።

### 🌟 ቁልፍ ባህሪያት (Core Features)
* **🏪 ሁለንተናዊ የገበያ ካታሎግ (Classifieds Marketplace):** ሽያጭ እና ኪራይ (ቤት፣ ሱቅ፣ መኪና፣ ማሽን፣ ኤሌክትሮኒክስ፣ አልባሳት ወዘተ)።
* **📑 የተገላቢጦሽ ጨረታ (Buyer Demand / Reverse Bidding RFQ):** ገዢዎች የሚፈልጉትን ዕቃ በምስል፣ በጽሁፍ እና በቪዲዮ የሚለጥፉበት፤ አቅራቢዎች ተወዳዳሪ ዋጋ የሚያቀርቡበት ክፍት መድረክ።
* **💳 ሁለንተናዊ የክፍያ ስነ-ምህዳር (Unified Payments & Multi-Gateway Fallback):**
  * **50.00 ብር** — የጨረታ ሰነድ መክፈቻና ማቅረቢያ
  * **100.00 ብር** — መደበኛ የማስታወቂያ ህትመት ክፍያ
  * **300.00 / 1,500.00 / 5,000.00 ብር** — ልዩ ተመራጭ፣ ፕሪሚየም ባነር እና የቪአይፒ ኮርፖሬት ስፖንሰርሺፕ
  * ክፍያ ሲቋረጥ ሳይቆለፍ ሁሉንም አማራጮች ክፍት የሚያደርግ (Telebirr, CBE Birr, Awash, In-App Wallet)።
* **⚡ አውቶሜትድ ማህበራዊ ሚዲያ ቦት:** ክፍያው ሲጠናቀቅ ማስታወቂያው በ 3 ሰከንድ ውስጥ ወደ **`@DessieMarket`** ቴሌግራም ቻናል ይሰራጫል።
* **💬 የቀጥታ ውይይት እና የዋጋ ድርድር (In-App Chat & Counter Offer):** ገዢና ሻጭ በቀጥታ የሚደራደሩበት፣ የስልክ ጥሪ (Click-to-Call) የሚያደርጉበት።
* **🛡️ ማህበረሰባዊ ደህንነት እና ጥቆማ (Trust & Safety):** አጭበርባሪዎችን በ 1 ንክኪ መጠቆሚያ (Report Scam) እና የሻጮች የኮከብ ደረጃ ምዘና (★ 4.9)።

---

## 🏗️ 2. የቴክኖሎጂ ቁልል (Technology Stack)

| ንብርብር (Layer) | ቴክኖሎጂ (Technology) | ዝርዝር መግለጫ (Description) |
|---|---|---|
| **Frontend Mobile** | **Flutter (Dart 3.x)** | Clean Architecture (Feature-First), Riverpod / Bloc State Management |
| **Backend API** | **Node.js (Express / NestJS)** | RESTful API, WebSocket (ለቀጥታ ውይይት), Idempotency Middleware |
| **Database** | **PostgreSQL 16 + Prisma ORM** | የተጠቃሚዎች፣ ማስታወቂያዎች፣ ጨረታዎች እና የክፍያ ግብይቶች ዳታቤዝ |
| **Caching & Pub/Sub** | **Redis Cluster** | የኦቲፒ ገደብ ቁጥጥር (Rate limiting) እና የውይይት ማስተላለፊያ |
| **Payment Gateways** | **Telebirr H5 / WebPay + CBE Birr WebPay** | 256-Bit SSL HMAC-SHA256 የተመሰጠረ የክፍያ ማረጋገጫ |
| **Social Automation** | **Telegraf (Telegram Bot API)** | ወደ `@DessieMarket` ቻናል ፎቶ እና ማጠቃለያ መላኪያ |
| **CI/CD & DevOps** | **Docker + GitHub Actions** | አውቶሜትድ አንድሮይድ APK/AAB ግንባታ እና የክላውድ ማሰማሪያ |

---

## 📂 3. የሪፖዚቶሪ ፎልደር መዋቅር (Repository Directory Tree)

```plaintext
dessie-mart/
├── .github/workflows/          # CI/CD pipelines (Android APK/AAB build, Backend deploy)
├── android/                    # Android Native configuration (build.gradle, ProGuard, App Icon)
├── ios/                        # iOS Native configuration (Info.plist, Runner)
├── lib/                        # Flutter Frontend (Clean Architecture)
│   ├── core/                   # Theme (Colors #1254d6 & #f97316), Constants, API Client
│   ├── features/               # Home, Auth, Listings, Payments, Tenders RFQ, Chat, Wallet
│   └── shared_widgets/         # Unified BottomNavBar (5 keys), TopAppBar, CustomToast
├── server/                     # Node.js Express Backend
│   ├── src/controllers/        # paymentWebhookController, listingController, tenderController
│   ├── src/services/           # telebirrService, cbeBirrService, telegramBotService
│   └── src/db/prisma/          # schema.prisma, PostgreSQL Migrations
├── scripts/                    # Keystore generation, Webhook simulation, Database backup
├── assets/                     # Official Logo (SVG/PNG), App Icon (Squircle), Promo Poster
├── docs/                       # Official Go-Live, Sandbox Guide, Build & Lifecycle Runbooks
├── docker-compose.yml          # Local full-stack development environment
└── README.md                   # Main Project Documentation
```

---

## 🚀 4. አሰራር እና አጀማመር (Quick Start Guide)

### 4.1 ቅድመ-ሁኔታዎች (Prerequisites)
- [Flutter SDK](https://docs.flutter.dev/get-started/install) (`v3.19.x` ወይም ከዚያ በላይ)
- [Node.js](https://nodejs.org) (`v20.x` LTS)
- [Docker](https://www.docker.com) & Docker Compose
- Android Studio / Xcode

---

### 4.2 የፕሮጀክቱ ማውረጃና ማስጀመሪያ (Installation)

```bash
# 1. ሪፖዚቶሪውን ክሎን ያድርጉ
git clone https://github.com/dessie-mart/dessie-mart.git
cd dessie-mart

# 2. የባክ-ኤንድ ሰርቨር እና ዳታቤዝ ማስጀመር (Docker)
docker-compose up -d

# 3. የባክ-ኤንድ ዲፔንደንሲዎችን መጫን እና ዳታቤዝ ማዘጋጀት
cd server
npm install
npx prisma migrate dev --name init
npm run dev

# 4. የሞባይል አፑን ማስጀመር (በሌላ ተርሚናል)
cd ../
flutter pub get
flutter run
```

---

## 🧪 5. የሙከራ ትዕዛዞች እና ሳንድቦክስ (Testing & Webhook Simulation)

የቴሌብር እና የሲቢኢ ብር ክፍያዎችን በሳንድቦክስ ለመፈተሽ የተዘጋጁ ስክሪፕቶችን መጠቀም ይችላሉ፡

```bash
# የ 50.00 ብር የቴሌብር ስኬታማ ክፍያ መሞከሪያ
npm run test:webhook:telebirr

# ወይም በቀጥታ በ cURL፡
curl -X POST http://localhost:4000/api/v1/payments/telebirr/webhook \
  -H "Content-Type: application/json" \
  -H "x-gateway-provider: TELEBIRR" \
  -d '{
    "outTradeNo": "DM-TD-TEST-8849",
    "totalAmount": "50.00",
    "tradeStatus": "SUCCESS",
    "transactionNo": "TB202508942019",
    "subjectPayload": {
      "tenderId": "tnd_industrial_generator_50kva"
    }
  }'
```

---

## 📱 6. የሞባይል አፕ ግንባታ ትዕዛዞች (Build Commands)

### ሀ. ለቀጥታ ጭነት የሚሆን ኤፒኬ (Release APK)
```bash
flutter build apk --release
# የሚገኝበት አድራሻ፡ build/app/outputs/flutter-apk/app-release.apk
```

### ለ. ለ Google Play Store የሚቀርብ ይፋዊ ጥቅል (AAB Bundle)
```bash
flutter build appbundle --release --obfuscate --split-debug-info=./build/symbols
# የሚገኝበት አድራሻ፡ build/app/outputs/bundle/release/app-release.aab
```

---

## 📑 7. ይፋዊ ሰነዶች ማውጫ (Documentation Links)

* 📖 [ይፋዊ የፕሮዳክሽን ማሰማሪያ ፍኖተ-ካርታ (GO_LIVE_RUNBOOK.md)](docs/GO_LIVE_RUNBOOK.md)
* 🧪 [የቴሌብር እና ሲቢኢ ብር ሳንድቦክስ ፍተሻ መመሪያ (SANDBOX_TESTING_GUIDE.md)](docs/SANDBOX_TESTING_GUIDE.md)
* 💳 [የክፍያ እና የጨረታ ህይወት ኡደት ማጠቃለያ (PAYMENT_TENDER_LIFECYCLE.md)](docs/PAYMENT_TENDER_LIFECYCLE.md)
* 📱 [የአንድሮይድ APK/AAB ግንባታ የተሟላ መመሪያ (APK_AAB_BUILD_GUIDE.md)](docs/APK_AAB_BUILD_GUIDE.md)

---

## 👥 8. አበርካቾች እና የድጋፍ መስመሮች (Team & Support)

* **ይፋዊ ቴሌግራም ቻናል:** [@DessieMarket](https://t.me/DessieMarket)
* **የደንበኞች ድጋፍ መስመር:** 📞 **127** / **+251 942 188 492**
* **መገኛ:** ሙጋድ የንግድ አዳራሽ፣ ፒያሳ፣ ደሴ፣ ደቡብ ወሎ፣ ኢትዮጵያ

---

<p align="center">
  <b>ደሴ ማርት (ሙጋድ ገበያ) — በኩራት በደሴ ከተማ የተሰራ! 💚💛❤️</b><br>
  <i>Empowering Commerce & Tenders Across South Wollo</i>
</p>