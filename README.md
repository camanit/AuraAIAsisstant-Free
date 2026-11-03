# 🌌 Aura AI Assistant — Web, Voice & Meeting Copilot

![Version](https://img.shields.io/badge/version-1.5.0-indigo)
![Manifest](https://img.shields.io/badge/Chrome-Manifest%20V3-success)
![License](https://img.shields.io/badge/license-MIT-blue)

**Aura AI Assistant** adalah ekstensi peramban modern berbasis **Chrome Manifest V3 (`sidePanel` API)** yang dirancang untuk merangkum halaman web secara mendalam, menerjemahkan artikel utuh (1:1), membuat opsi balasan cerdas dwibahasa (*Bilingual Smart Reply*), serta menjadi asisten *real-time* saat rapat di **Zoom Web, Google Meet, maupun Live Stream (YouTube, Facebook, TikTok, Twitch)**.

---

## ✨ Fitur Utama

### 🟢 Aura Free (Gratis Selamanya)
- **📄 Ringkasan Eksekutif Mendalam:** Merangkum artikel panjang, berita, postingan LinkedIn Pulse, dan repositori GitHub menjadi *Executive Summary*, *Key Takeaways*, dan *Kesimpulan*.
- **🌐 Terjemahan Utuh 1:1 (Full Page Translation):** Menerjemahkan seluruh isi artikel paragraf demi paragraf dari atas sampai bawah tanpa dipotong atau diringkas.
- **💬 Bilingual Smart Reply + 1-Click Insert:** Membuat 3 opsi balasan yang otomatis menyesuaikan **bahasa asli halaman/lawan bicara** (lengkap dengan terjemahan artinya dalam bahasa Anda) dan menyuntikkannya langsung ke kotak komentar LinkedIn/Gmail/Chat dengan 1 klik.
- **🎙️ Voice Copilot (Speech-to-Text & Text-to-Speech):** Mendukung perintah suara via mikrofon dan pembacaan hasil analisis dengan suara AI natural.
- **🌍 5 Bahasa Antarmuka Global (Full UI Localization):** Seluruh tombol dan menu otomatis berubah mengikuti bahasa pilihan Anda: 🇮🇩 Bahasa Indonesia, 🇬🇧 English, 🇯🇵 日本語, 🇸🇦 العربية, dan 🇨🇳 中文.
- **🔒 Keamanan Lokal (BYOK + Free Instant Engine):** Langsung berfungsi tanpa API Key menggunakan *Built-in Instant Engine*, atau hubungkan API Key **Google Gemini (`gemini-3.0-flash`)**, **OpenAI**, atau **Groq** yang disimpan aman di `chrome.storage.local`.

### 👑 Aura PRO (Khusus Mode Rapat Web & Video Live Stream)
- **🔴 Live Meeting & Stream Copilot:** Mendeteksi otomatis **Zoom Web, Google Meet, Microsoft Teams, YouTube Live, Facebook Live, TikTok Live, dan Twitch**.
- **📡 Auto-Sync Live Captions (CC):** Memantau *subtitle/closed captions* dan *live chat* secara *real-time* menggunakan `MutationObserver`.
- **🗣️ Bilingual Teleprompter:** Menampilkan maksud pembicara dalam bahasa ibu Anda sekaligus menyiapkan kalimat respons dalam bahasa lawan bicara untuk langsung diucapkan di depan kamera.
- **📋 Generator Notulensi Rapat (Auto MoM):** Menyusun rekaman percakapan rapat menjadi dokumen *Minutes of Meeting* rapi yang siap diunduh ke format Markdown (`.md`).

---

## 🛠️ Cara Instalasi (Developer / Load Unpacked)

1. Unduh atau *clone* repositori ini:
   ```bash
   git clone https://github.com/camanit/AuraAIAsisstant.git
   ```
2. Buka browser berbasis Chromium (Google Chrome, Microsoft Edge, Brave, Arc) dan kunjungi `chrome://extensions/`.
3. Aktifkan sakelar **Developer mode** di pojok kanan atas.
4. Klik tombol **Load unpacked** di pojok kiri atas, lalu pilih folder proyek `Aura AI Assistant`.
5. Klik ikon **✦ Aura AI** di toolbar browser untuk membuka **Side Panel**.

---

## 📁 Struktur Proyek

- `manifest.json` — Konfigurasi Chrome Extension Manifest V3.
- `background.js` — Service Worker untuk manajemen Side Panel & menu klik kanan (*Context Menus*).
- `content.js` — Ekstraktor konten halaman cerdas, *Auto-Sync Live Caption Observer*, dan *1-Click Chat Inserter*.
- `sidepanel.html` & `sidepanel.css` — Antarmuka SaaS modern dengan dukungan *Dark/Light Mode*.
- `sidepanel.js` — Pengendali utama lokalisasi 5 bahasa, multi-provider AI (Gemini/OpenAI/Groq), *Free Instant Engine*, serta fitur suara & MoM.
- `ROADMAP.md` — Peta jalan pengembangan produk (Fase 1 – Fase 5).
- `PRIVACY_POLICY.md` — Kebijakan privasi resmi untuk publikasi Chrome Web Store.
- `LAUNCH_KIT_LINKEDIN.md` — Panduan publikasi Chrome Web Store & draf konten *Build in Public* LinkedIn.

