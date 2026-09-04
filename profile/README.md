<div align="center">
  <img src="https://raw.githubusercontent.com/AERoutee/AERoute-FE/main/src/assets/aeroute-logo.png" alt="AERoute" width="180" />

# AERoute

### A clearer route for every breath.

[![Live Demo](https://img.shields.io/badge/Live_Demo-aeroute.my.id-0B7A53?style=for-the-badge&logo=googlechrome&logoColor=white)](https://aeroute.my.id)
[![Frontend](https://img.shields.io/badge/GitHub-AERoute--FE-181717?style=for-the-badge&logo=github)](https://github.com/AERoutee/AERoute-FE)
[![Backend](https://img.shields.io/badge/GitHub-AERoute--BE-181717?style=for-the-badge&logo=github)](https://github.com/AERoutee/AERoute-BE)
[![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)](https://github.com/AERoutee/AERoute-FE/blob/main/LICENSE)

**Submission for ITECHNO CUP 2026 - Web Development**

**By Team singular you**

</div>

---

## 📋 Daftar Isi

- [Tim Developer](#-tim-developer)
- [Tentang Proyek](#-tentang-proyek)
- [Fitur Unggulan](#-fitur-unggulan)
- [Demo & Screenshot](#-demo--screenshot)
- [Teknologi](#-teknologi)
- [Arsitektur Sistem](#-arsitektur-sistem)
- [Instalasi & Setup](#-instalasi--setup)
- [Penggunaan](#-penggunaan)
- [API Documentation](#-api-documentation)
- [Testing](#-testing)
- [Lisensi](#-lisensi)

---

## 👥 Tim Developer

| Nama                    | Peran                                    | GitHub                                   |
| ----------------------- | ---------------------------------------- | ---------------------------------------- |
| **Andrian Pratama**     | Project Lead & Lead Full-Stack Developer | [@Yanzz231](https://github.com/Yanzz231) |
| **Jeremy Auriel Zhang** | Full-Stack Developer                     | [@jeremzhg](https://github.com/jeremzhg) |
| **Calvin Wu**           | Product Manager                          | [@5calvinw](https://github.com/5calvinw) |

---

## 🎯 Tentang Proyek

### Latar Belakang

![Latar Belakang AERoute](assets/LatarBelakang.png)

### Solusi yang Ditawarkan

![Mockup AERoute](assets/mockups.png)
![Solusi yang Ditawarkan](assets/Solusi.png)

### Tujuan Projek

![Solusi yang Ditawarkan](assets/tujuan.png)

---

## ✨ Fitur Unggulan

### Fitur Utama

| Fitur                                | Deskripsi                                                                                                                                                                                                                                                                                 | Keunggulan                                                                                                                                    |
| ------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| **Perbandingan Rute Multimoda**      | Pengguna dapat memilih satu hingga tiga mode dari **Walk, Cycle, Bus, Train, dan Subway**. AERoute membandingkan rute aktif secara terpisah atau menyusun perjalanan terintegrasi seperti Cycle → Transit → Walk sesuai kombinasi yang tersedia.                                          | Satu planner dapat membantu pengguna membandingkan perjalanan aktif dan transportasi umum tanpa berpindah aplikasi.                           |
| **Analisis Paparan PM2.5**           | Setiap alternatif menampilkan estimasi PM2.5 untuk keberangkatan saat ini, +30 menit, dan +60 menit. Kondisi per segmen divisualisasikan langsung pada garis rute dengan warna hijau, kuning, merah, atau abu-abu ketika data tidak tersedia.                                             | Pengguna dapat melihat perubahan kualitas udara sepanjang perjalanan dan mempertimbangkan waktu keberangkatan, bukan hanya jarak atau durasi. |
| **Rekomendasi Rute yang Transparan** | AERoute menampilkan label rekomendasi, alasan pemilihan, trade-off, keterbatasan data, dan **evidence completeness** untuk setiap hasil. Prioritas aktif tersedia dalam mode **Balanced** dan **Lower exposure**, sedangkan transit menyediakan **Less walking** dan **Fewer transfers**. | Hasil tidak diberikan sebagai skor misterius; pengguna dapat memahami faktor yang membuat satu rute lebih sesuai daripada alternatif lain.    |
| **Konteks Cuaca, Panas, dan UV**     | Checkpoint cuaca mengikuti perkiraan waktu pengguna mencapai bagian tertentu dari rute. Ringkasan suhu, peluang hujan, angin, UV, serta rekomendasi waktu istirahat ditampilkan bersama hasil perjalanan.                                                                                 | Membantu pengguna menilai kenyamanan perjalanan berdasarkan kondisi yang mungkin ditemui di sepanjang rute.                                   |
| **Rest Stop dan Informasi Transit**  | Kandidat tempat istirahat dan titik transit muncul sebagai marker interaktif. Popup menampilkan alamat, status buka, toilet, parkir, tempat duduk, informasi aksesibilitas yang tersedia, maksimal tiga foto beratribusi, dan **View 360°** ketika Street View tersedia.                  | Informasi pendukung perjalanan dapat diperiksa langsung dari peta tanpa menutupi konteks rute yang sedang dipilih.                            |
| **Community Road Reports**           | Pengguna dapat membuat laporan hazard, jalan terhalang, kecelakaan, konstruksi, atau masalah peta dengan deskripsi dan maksimal tiga foto. Pengguna lain dapat **Confirm**, **Dispute**, atau menarik verifikasi, sedangkan pemilik dapat menyelesaikan laporannya.                       | Kondisi lapangan yang belum tercakup provider peta dapat menjadi sinyal tambahan dalam evaluasi rute.                                         |
| **Live Location dan Route Guidance** | Lokasi serta arah pengguna diperbarui melalui browser geolocation. Setelah memperoleh lokasi yang masih baru, akurat, dan dekat titik awal, pengguna dapat memulai tampilan panduan rute; rute non-transit juga mendukung pembaruan ketika pengguna menyimpang.                           | Memberikan pengalaman map-first dari tahap perencanaan hingga perjalanan dimulai.                                                             |
| **Insights Perjalanan**              | Perjalanan yang dikonfirmasi dapat dicatat sebagai **modeled trip impact**. Halaman Insights merangkum jumlah perjalanan, jarak dan durasi aktif, estimasi pengurangan exposure index, serta lebih sedikitnya sinyal laporan terkonfirmasi.                                               | Pengguna memperoleh ringkasan dampak pilihan rute berdasarkan hasil perencanaan yang tersimpan.                                               |

### Fitur Tambahan

- **Peta Interaktif** - alternatif dapat dipilih melalui kartu hasil maupun garis rute; layer cuaca, aksesibilitas, rest stop, dan laporan komunitas dapat dikontrol dari dashboard.
- **Reduced-exertion Approximation** - menyediakan alternatif berdasarkan data usaha perjalanan yang tersedia tanpa mengklaim rute wheelchair-safe atau sepenuhnya step-free.
- **PWA Offline Summary** - menyimpan ringkasan terbatas dari rute terakhir selama maksimal 24 jam tanpa koordinat dan identitas pengguna.
- **Autentikasi dan Pemulihan Akun** - mendukung email/password, Google OAuth, OTP enam digit, reset password, dan pencabutan sesi lama.
- **Pengelolaan Profil** - pengguna dapat memperbarui nama dan foto profil; gambar diproses sebelum disimpan pada object storage privat.
- **Dashboard Responsif** - planner, hasil rute, report flow, popup peta, dan navigasi disesuaikan untuk desktop maupun perangkat mobile.

---

## 📸 Demo & Screenshot

### Live Demo

| Layanan      | URL                                                                      |
| ------------ | ------------------------------------------------------------------------ |
| Live Website | [https://aeroute.my.id](https://aeroute.my.id)                           |
| API          | [https://api.aeroute.my.id](https://api.aeroute.my.id)                   |
| Swagger UI   | [https://api.aeroute.my.id/api/docs](https://api.aeroute.my.id/api/docs) |

### Screenshot Aplikasi

![Screenshot AERoute](assets/screenshots.png)

### Video Demo

## Link Video Demo: https://www.youtube.com/watch?v=qeQefV2TFRI

[![Watch the demo](assets/thumbnail.png)](https://www.youtube.com/watch?v=qeQefV2TFRI)

---

## 🛠️ Teknologi

### Tech Stack

#### Frontend

```text
Framework      : React 19 + Vite 8 + TypeScript
UI             : Tailwind CSS 4
Routing        : React Router
Server State   : TanStack Query + Axios
Authentication : Better Auth React Client
Maps & Places  : Google Maps JavaScript API + Places
PWA            : Web App Manifest + Service Worker + reduced offline summary
Testing        : Jest + React Testing Library
```

#### Backend

```text
Runtime        : Node.js + TypeScript ESM
Framework      : Express 5
Database / ORM : PostgreSQL + Prisma 7
Authentication : Better Auth
Validation     : Zod
Google APIs    : Routes, Air Quality, Weather, Places
Media          : Multer + Sharp + private S3-compatible storage
Documentation  : OpenAPI 3.1 + Swagger UI
```

#### DevOps & Tools

```text
Deployment     : Railway
Website        : aeroute.my.id
API            : api.aeroute.my.id
CI/CD          : Railway GitHub Integration
Quality Gates  : tests, coverage, lint, typecheck, build, Prisma validation/migrations
Monitoring     : LogRocket frontend; redacted Railway/backend logs
```

### Provider & Asset Attribution

| Sumber                         | Penggunaan                                                                       |
| ------------------------------ | -------------------------------------------------------------------------------- |
| **Google Maps JavaScript API** | Map rendering dan interaksi browser                                              |
| **Google Places API**          | Place search/autocomplete dan rest-stop candidates sepanjang rute                |
| **Google Routes API**          | Geometry, alternatif, durasi, jarak, transit legs, serta provider labels         |
| **Google Air Quality API**     | Current conditions untuk offset 0 dan hourly forecast buckets untuk +30/+60      |
| **Google Weather API**         | Hourly forecast terdekat dengan target waktu tiap checkpoint                     |
| **AERoute Community Reports**  | Sinyal laporan aktif dalam 100 meter dari geometry; bukan verifikasi keselamatan |
| **Icons8 Color Icons**         | Ikon warna antarmuka; attribution: [Icons8](https://icons8.com/icons/color)      |

Google provider data dapat tidak lengkap atau tidak tersedia menurut wilayah, waktu, konfigurasi API, dan cakupan layanan. Custom ranking dan modeled metrics dihitung AERoute, bukan skor keselamatan dari Google.

---

## 🏗️ Arsitektur Sistem

### System Architecture

![AERoute System Architecture](https://raw.githubusercontent.com/AERoutee/AERoute-FE/main/assets/Architecture.png)

### Database Schema

![AERoute Entity Relationship Diagram](https://raw.githubusercontent.com/AERoutee/AERoute-FE/main/assets/ERD.png)

### Folder Structure

```text
AERoute/
├── AERoute-FE/
│   ├── public/               # manifest, service worker, offline page
│   ├── src/api/              # auth, routes, reports, insights
│   ├── src/components/       # map, layout, feature UI
│   ├── src/pages/            # dashboard, insights, profile, public pages
│   └── tests/
├── AERoute-BE/
│   ├── prisma/               # schema and migrations
│   ├── src/modules/          # route comparison, reports, insights, auth/recovery/profile
│   └── tests/
└── .github/profile/
```

---

## ⚙️ Instalasi & Setup

### Prerequisites

- Node.js 24 atau versi LTS modern yang didukung toolchain.
- npm, PostgreSQL, dan Git.
- Google Cloud project dengan **Maps JavaScript API, Places API, Routes API, Air Quality API, dan Weather API** aktif serta billing/credentials yang sesuai.
- Browser key yang dibatasi untuk frontend dan server key yang dibatasi untuk backend.
- SMTP account dan private S3-compatible bucket untuk recovery serta images.

### 1️⃣ Clone Repository

```bash
git clone https://github.com/AERoutee/AERoute-FE.git
git clone https://github.com/AERoutee/AERoute-BE.git
```

### 2️⃣ Setup Backend

```bash
cd AERoute-BE
npm ci
copy .env.example .env
npm run db:migrate
npm run dev
```

Backend berjalan di `http://localhost:3000`. `npm run db:migrate` menjalankan `prisma migrate deploy`, termasuk migration `20260901000100`, `20260901000200`, dan `20260902000100` pada database yang belum memilikinya.

### 3️⃣ Setup Frontend

```bash
cd AERoute-FE
npm ci
copy .env.example .env
npm run dev
```

Frontend berjalan di `http://localhost:5173`.

### 4️⃣ Environment Variables

Frontend:

```env
VITE_API_BASE_URL="http://localhost:3000"
VITE_GOOGLE_MAPS_BROWSER_KEY="replace-with-browser-restricted-key"
VITE_LOGROCKET_APP_ID="your-workspace/your-app"
VITE_APP_VERSION="0.1.0"
```

Backend groups:

```text
Application : NODE_ENV, PORT, FRONTEND_ORIGIN, CORS_ORIGINS, TRUST_PROXY
Auth        : BETTER_AUTH_URL, BETTER_AUTH_SECRET, GOOGLE_CLIENT_ID, GOOGLE_CLIENT_SECRET
Database    : DATABASE_URL
Providers   : GOOGLE_MAPS_SERVER_KEY, PROVIDER_TIMEOUT_MS
Email       : SMTP_HOST, SMTP_PORT, SMTP_SECURE, SMTP_USER, SMTP_PASSWORD
Storage     : S3_ENDPOINT, S3_REGION, S3_BUCKET, S3_PUBLIC_BASE_URL, S3_ACCESS_KEY_ID, S3_SECRET_ACCESS_KEY
```

Jangan commit `.env`; server secrets tidak boleh memakai prefix `VITE_`.

### Railway Deployment & CI/CD

- Railway Railpack menjalankan dependency install dan production build.
- Backend menjalankan `npm run db:migrate` sebagai **pre-deploy command** sebelum aplikasi baru aktif.
- Backend health check memakai `/api/health`; frontend memakai `/`.
- Railway Variables menyimpan production configuration; push ke branch terhubung memicu build, migration predeploy, health check, dan deploy.

---

## 🚀 Penggunaan

### Menjalankan Aplikasi

Frontend:

```bash
npm run dev
npm test
npm run test:coverage
npm run lint
npm run typecheck
npm run build
```

Backend:

```bash
npm run dev
npm test
npm run test:coverage
npm run lint
npm run typecheck
npm run build
npm run db:migrate
npx prisma validate
```

### User Guide

#### Membandingkan Rute

1. Buka [AERoute](https://aeroute.my.id), masuk, lalu buka dashboard map.
2. Pilih origin dan destination melalui Places atau map.
3. Aktifkan satu sampai maksimal tiga mode dari **Walk, Cycle, Bus, Train, dan Subway** sebagai preferensi/kandidat. Walk + Cycle tanpa transit membandingkan dua alternatif aktif terpisah. Cycle + satu atau lebih transit menjalankan itinerary komposit Cycle → transit → Walk bersama fallback transit native; parkir sepeda pada transit pertama tidak diverifikasi.
4. Untuk Walk/Cycle tanpa transit atur **Balanced** atau **Lower exposure**. Jika itinerary memuat Bus/Train/Subway, atur hanya **Less walking** atau **Fewer transfers** untuk seluruh itinerary transit.
5. Opsional: aktifkan sensitive-user, reduced-exertion approximation, report preference, dan layer rest-stop candidates.
6. Tekan **Compare routes** untuk melihat current, +30, dan +60, lalu periksa explanation, trade-offs, evidence completeness, hazard signals, Break/heat/UV, PM2.5 segment legend, dan limitations.
7. Pilih route card/polyline. **Start route guidance** aktif hanya dengan live fix yang fresh, akurat, dan dekat origin; transit/composite tidak melakukan auto reroute dan fitur ini bukan turn-by-turn guidance.

![Tutorial melihat dan memilih rute AERoute](assets/Guide1.png)

#### Community Report

1. Tekan **Report**, pilih kategori, isi deskripsi, dan tambahkan maksimal tiga JPG/PNG/WebP berukuran maksimal 3 MB per file.
2. Report aktif hingga 24 jam kecuali diselesaikan lebih awal oleh pemilik.
3. Pengguna lain dapat **Confirm**, **Dispute**, atau menarik verification; pemilik dapat resolve report miliknya.
4. Evidence score menggabungkan recency, foto, dan confirmation balance; skor bukan bukti kebenaran atau keselamatan.

![Tutorial membuat Community Report AERoute](assets/Guide2.png)

#### Mengelola Akun

1. Buka menu akun pada dashboard, lalu pilih **Profile**.
2. Ubah foto profil melalui tombol edit pada avatar.
3. Ubah nama melalui **Edit name**, lalu simpan perubahan.
4. Akun Google dapat menambahkan password setelah verifikasi email.

![Tutorial mengelola akun AERoute](assets/Guide3.png)

#### Insights dan Offline

1. Setelah perjalanan, konfirmasi pencatatan modeled trip impact dari persisted route result; **Recorded trips** adalah planned/model estimate, bukan GPS trace.
2. Buka route **`/insights`** melalui menu **Insights** untuk melihat modeled impact summary. Insights saat ini hanya memodelkan impact; Saved Commute tetap kompatibel di backend, tetapi UI pembuatan, pengelolaan, dan watch telah dihapus.
3. Saat offline, PWA hanya menampilkan reduced summary terakhir hingga 24 jam; koordinat dan identitas pengguna tidak disimpan pada summary tersebut.

---

## 📚 API Documentation

### Base URL

```text
Development : http://localhost:3000
Production  : https://api.aeroute.my.id
Swagger UI  : https://api.aeroute.my.id/api/docs
OpenAPI JSON: https://api.aeroute.my.id/api/openapi.json
```

### Health, Authentication, Recovery, dan Profile

```http
GET    /api/health
POST   /api/auth/sign-up/email
POST   /api/auth/sign-in/email
POST   /api/auth/sign-in/social
GET    /api/auth/get-session
POST   /api/auth/sign-out
POST   /api/auth/update-user
POST   /api/auth/change-password
GET    /api/auth/list-accounts
POST   /api/v1/recovery-challenges
GET    /api/v1/recovery-challenges/:id
POST   /api/v1/recovery-challenges/:id/resend
POST   /api/v1/recovery-challenges/:id/verify
POST   /api/v1/recovery-challenges/:id/reset
GET    /api/v1/profile/avatar/:userId
PUT    /api/v1/profile/avatar
DELETE /api/v1/profile/avatar
```

### Authenticated Route Comparison

```http
POST /api/v1/route-comparisons
GET  /api/v1/place-photos?name=...
```

Request menerima mode aktif/transit, transit modes/preference, optional Cycle-to-transit access plan, accessibility mode, departure offsets `0/30/60`, hazard policy, dan rest-stop option. Walk normal meminta rest stops; composite Cycle + transit memakai offset `0`, tanpa rest stops, dan selalu disertai request fallback transit native. Response memuat current routes, future departure comparisons, compact/full itinerary segments, explanation/evidence completeness, report signals, Break/weather/heat/UV, serta Places candidates dengan Place ID/association ID yang dipersistenkan bila tersedia, maksimal tiga foto beserta Google Maps/report URI, facility/accessibility facts, source disclosure, dan warnings. Detail transit mengirim `routeResultId`, ordinal, dan role hanya ketika association context tersedia.

### Community Road Reports

```http
GET    /api/v1/road-reports
GET    /api/v1/road-reports/mine
POST   /api/v1/road-reports
PUT    /api/v1/road-reports/:id/verification
DELETE /api/v1/road-reports/:id/verification
PATCH  /api/v1/road-reports/:id
GET    /api/v1/road-report-images/:id
```

`GET nearby` dan image read bersifat public sesuai lifecycle report; create, mine, verification, retract, dan owner resolution membutuhkan session.

### Saved Commute & Trip Impact

```http
GET    /api/v1/saved-commutes
POST   /api/v1/saved-commutes
PATCH  /api/v1/saved-commutes/:id
DELETE /api/v1/saved-commutes/:id
POST   /api/v1/trip-impacts
GET    /api/v1/trip-impacts/summary
```

Seluruh endpoint saved commute dan trip impact membutuhkan authentication. Endpoint Saved Commute dipertahankan untuk kompatibilitas backend dan record lama; frontend tidak lagi menyediakan UI pembuatan atau pengelolaan. Insights saat ini hanya menyajikan modeled trip impact. Kontrak request/response, multipart upload, cookie security, examples, dan status codes tersedia di Swagger UI.

---

## 🧪 Testing

### Perintah Verifikasi

```bash
# Jalankan di masing-masing repository
npm test
npm run test:coverage
npm run lint
npm run typecheck
npm run build

# Backend database contract
npx prisma validate
npm run db:migrate
```

Tidak ada klaim perintah E2E karena package frontend maupun backend tidak menyediakan script E2E.

### Hasil Terverifikasi

| Repository   | Suites | Tests | Statements | Branches | Functions |  Lines | Status                                       |
| ------------ | -----: | ----: | ---------: | -------: | --------: | -----: | -------------------------------------------- |
| **Frontend** |     33 |   210 |     93.75% |   83.36% |    91.42% | 97.74% | tests, coverage, lint, typecheck, build pass |
| **Backend**  |     20 |   344 |     95.47% |   87.27% |    95.48% | 98.17% | tests, coverage, lint, typecheck, build pass |

`prisma validate` dan migration deploy pass. Coverage thresholds:

| Repository           | Statements | Branches | Functions | Lines |
| -------------------- | ---------: | -------: | --------: | ----: |
| **Frontend minimum** |        80% |      70% |       80% |   80% |
| **Backend minimum**  |        95% |      85% |       95% |   95% |

Provider behavior yang bergantung pada Google coverage, browser geolocation, SMTP, dan object storage tetap memerlukan integration/manual QA dengan credentials dan environment yang sesuai; angka coverage tidak diklaim sebagai cakupan provider eksternal end-to-end.

---

## 📄 Lisensi

Proyek ini dilisensikan di bawah [MIT License](https://github.com/AERoutee/AERoute-FE/blob/main/LICENSE).

---

<div align="center">

**Made with ❤️ by Team singular you for ITECHNO CUP 2026**

</div>
