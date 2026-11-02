<p align="center">
  <a href="https://github.com/renzetx/RNGram">
    <img src="https://raw.githubusercontent.com/pyrogram/artwork/master/artwork/pyrogram-logo.png" alt="RNGram Logo" width="130">
  </a>
</p>

<h1 align="center">⚡ RNGram ⚡</h1>

<p align="center">
  <b>Modern, Ultra-Fast & Feature-Complete Telegram MTProto Framework for Python</b>
</p>

<p align="center">
  <a href="https://github.com/renzetx/RNGram">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=18&duration=2400&pause=800&color=0088CC&center=true&vCenter=true&width=620&lines=%E2%9A%A1+MTProto+Layer+232+Protocol+Support;%F0%9F%92%AC+Built-in+Pyromod+Conversation+Flow;%F0%9F%92%8E+Native+TON+Wallet+%26+Telegram+Stars;%F0%9F%8E%A8+Expandable+Quotes+%26+Message+Effects;%F0%9F%9B%A1%EF%B8%8F+Leak-Proof+LRU+Memory+%26+Async+Safety" alt="RNGram Feature Highlights" />
  </a>
</p>

<p align="center">
  <a href="https://pypi.org/project/RNGram"><img src="https://img.shields.io/pypi/v/RNGram.svg?style=for-the-badge&color=0088CC&logo=pypi&logoColor=white" alt="PyPI Version"></a>
  <a href="https://pypi.org/project/RNGram"><img src="https://img.shields.io/pypi/pyversions/RNGram.svg?style=for-the-badge&color=3776AB&logo=python&logoColor=white" alt="Python Versions"></a>
  <a href="#"><img src="https://img.shields.io/badge/MTProto-Layer%20232-FF69B4?style=for-the-badge&logo=telegram&logoColor=white" alt="MTProto Layer 232"></a>
  <a href="https://github.com/renzetx/RNGram/blob/main/COPYING.lesser"><img src="https://img.shields.io/badge/License-LGPLv3-2EA44F.svg?style=for-the-badge" alt="License"></a>
  <a href="https://t.me/Renboyz"><img src="https://img.shields.io/badge/Telegram-Channel-0088CC?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram Channel"></a>
</p>

---

<p align="center">
  <a href="#-fitur-unggulan">✨ Fitur Unggulan</a> •
  <a href="#-instalasi">📦 Instalasi</a> •
  <a href="#-panduan-cepat-quick-start">🚀 Panduan Cepat</a> •
  <a href="#-fitur-modern-telegram--ton">💎 Telegram Modern & TON</a> •
  <a href="#-matriks-perbandingan">📊 Matriks Perbandingan</a> •
  <a href="#-komunitas--dukungan">🤝 Komunitas</a>
</p>

---

## 📖 Tentang RNGram

**RNGram** adalah framework Telegram MTProto API asinkron berperforma tinggi yang dibangun di atas fondasi **Pyrogram** dengan dukungan **MTProto Layer 232** terbaru. Dirancang secara khusus untuk membangun bot modern, userbot, serta sistem otomasi berskala besar dengan stabilitas maksimal.

RNGram menyatukan fitur-fitur tercanggih protokol Telegram dengan ekstensi pengembang terbaik—seperti alur percakapan interaktif (*Pyromod*), pembuat keyboard ringkas (*Smart Keyboards*), integrasi TON Blockchain, dan mitigasi *memory leak* berbasis *Bounded LRU Cache*—semuanya tersedia langsung (*battery-included*) tanpa dependensi pihak ketiga yang rumit.

---

## ✨ Fitur Unggulan

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>🚀 MTProto Layer 232</h3>
      <p>Dukungan terlengkap untuk fitur Telegram modern: Telegram Stars, Hadiah (Gifts), Paid Media, Stories, Business Connections, dan Efek Animasi Pesan.</p>
    </td>
    <td width="50%" valign="top">
      <h3>💬 Alur Interaktif (Pyromod)</h3>
      <p>Buat dialog tanya-jawab multi-langkah yang elegan dengan <code>listen()</code>, <code>ask()</code>, dan <code>wait_for_click()</code> langsung dari objek <code>Message</code>, <code>Chat</code>, atau <code>User</code>.</p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>💎 Integrasi TON Wallet</h3>
      <p>Kelola dan kueri alamat TON blockchain pengguna secara langsung melalui API Telegram (<code>get_address_ton_wallet</code>, <code>get_user_ton_wallet_addresses</code>).</p>
    </td>
    <td width="50%" valign="top">
      <h3>🎨 Rich Text & Formatting Modern</h3>
      <p>Dukungan kutipan yang dapat diciutkan (<i>Expandable Blockquote</i>), format waktu dinamis (<code>&lt;tg-time&gt;</code>), spoiler, dan custom emoji.</p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>🛡️ Zero-Leak & Task Safety</h3>
      <p>Dilengkapi <b>Bounded LRU Caches</b>, pembersihan listener otomatis saat timeout, serta pelacakan referensi kuat pada task asyncio guna mencegah interupsi Garbage Collector.</p>
    </td>
    <td width="50%" valign="top">
      <h3>⚡ Akselerasi C Ekstra Cepat</h3>
      <p>Dukungan modul C opsional (<code>tgcrypto</code>) untuk kecepatan enkripsi/dekripsi MTProto instan dengan efisiensi CPU maksimal.</p>
    </td>
  </tr>
</table>

---

## 📦 Instalasi

Pilih manajer paket favorit Anda:

### Menggunakan `pip`
```bash
# Instal versi standar
pip install -U RNGram

# Instal versi performa tinggi (dengan akselerasi C tgcrypto) [Sangat Disarankan]
pip install -U "RNGram[fast]"
```

### Menggunakan `uv` (Ultra Cepat)
```bash
uv add "RNGram[fast]"
```

### Menggunakan `poetry`
```bash
poetry add RNGram -E fast
```

> [!TIP]
> **Kompatibilitas Python:** Mendukung penuh Python 3.10, 3.11, 3.12, 3.13, hingga 3.14.

---

## 🚀 Panduan Cepat (Quick Start)

### 1. Bot Sederhana dengan Expandable Blockquote & Rich Text

```python
from pyrogram import Client, filters, enums

app = Client(
    "my_bot",
    api_id=12345,
    api_hash="0123456789abcdef0123456789abcdef",
    bot_token="123456:ABC-DEF1234ghIkl-zyx57W2v1u123ew11"
)

@app.on_message(filters.command("start") & filters.private)
async def start_handler(client: Client, message):
    text = (
        f"{client.bold('Halo, ' + message.from_user.first_name)}! 👋\n\n"
        f"{client.expandable_blockquote('Ini adalah teks kutipan panjang yang bisa dibuka dan ditutup langsung di aplikasi Telegram modern.')}\n\n"
        f"📅 Waktu server: <tg-time unix='1730000000' format='r'>baru saja</tg-time>"
    )
    await message.reply_text(text, parse_mode=enums.ParseMode.HTML)

app.run()
```

---

### 2. Dialog Formulir Interaktif (Built-in Pyromod)

Buat alur tanya-jawab multi-langkah tanpa memerlukan modul FSM (Finite State Machine) eksternal:

```python
from pyrogram import Client, filters

app = Client("my_bot")

@app.on_message(filters.command("daftar") & filters.private)
async def register_dialog(client: Client, message):
    # Ajukan pertanyaan dan tunggu balasan dari pengguna
    nama = await message.chat.ask(
        "📝 Silakan masukkan nama lengkap Anda:",
        timeout=60
    )

    # Ajukan pertanyaan tahap kedua
    usia = await message.chat.ask(
        f"Senang berkenalan denganmu, {nama.text}! Berapa usia Anda?",
        timeout=60
    )

    await message.reply_text(
        f"✅ <b>Pendaftaran Berhasil!</b>\n"
        f"• Nama: {nama.text}\n"
        f"• Usia: {usia.text} tahun"
    )

app.run()
```

---

### 3. Smart Keyboards (`ikb` & `btn`)

Menyusun keyboard inline dengan sintaks yang bersih dan mudah dibaca:

```python
from pyrogram import Client, filters
from pyrogram.helpers import ikb, btn

app = Client("my_bot")

@app.on_message(filters.command("menu"))
async def show_menu(client: Client, message):
    keyboard = ikb([
        [btn("📢 Saluran Resmi", "https://t.me/Renboyz", type="url")],
        [btn("⚡ Beli VIP", "buy_vip"), btn("ℹ️ Bantuan", "help_menu")],
        [btn("❌ Tutup Menu", "close_menu")]
    ])

    await message.reply_text(
        "Silakan pilih salah satu opsi di bawah ini:",
        reply_markup=keyboard
    )

app.run()
```

---

## 💎 Fitur Modern Telegram & TON

### 1. Telegram Stars & Paid Media (Konten Berbayar)

Kirim konten foto/video eksklusif yang hanya dapat dibuka setelah pengguna membayar dengan Telegram Stars:

```python
from pyrogram.types import InputMediaPhoto

await app.send_paid_media(
    chat_id=chat_id,
    stars_amount=25,
    media=[InputMediaPhoto("foto_premium.jpg")],
    caption="⭐ Buka foto resolusi tinggi ini menggunakan 25 Telegram Stars!"
)
```

### 2. Animasi Efek Pesan Layar Penuh (Message Effects)

Kirim pesan dengan efek visual bawaan Telegram (kembang api, api membara, hati, dll.):

```python
await app.send_message(
    chat_id=chat_id,
    text="🎉 Selamat! Transaksi Anda telah berhasil dikonfirmasi.",
    effect_id=5104841245755180586  # ID Efek animasi resmi Telegram
)
```

### 3. Kueri TON Wallet Pengguna (Layer 232)

Periksa alamat dompet TON terhubung milik pengguna secara langsung:

```python
# Mendapatkan informasi alamat dompet TON pengguna
wallet_info = await app.get_user_ton_wallet_addresses("username_atau_id")

for wallet in wallet_info:
    print(f"User ID: {wallet.user_id}")
    print(f"Alamat TON: {wallet.address}")
```

---

## 📊 Matriks Perbandingan

Perbandingan komprehensif antara **RNGram** dengan pustaka Telegram berbasis MTProto lainnya:

| Fitur / Kapabilitas | Pyrogram Legacy | Fork Standar | **⚡ RNGram (v2.2.26)** |
| :--- | :---: | :---: | :---: |
| **MTProto Layer** | Layer 158 *(Usang)* | Layer 220+ | **Layer 232 (Terbaru)** |
| **Integrasi TON Wallet** | ❌ | ❌ / Parsial | **✅ Lengkap (Native API)** |
| **Telegram Stars & Paid Media** | ❌ | ⚠️ Terbatas | **✅ Lengkap** |
| **Sticker & Emoji Set Management** | ⚠️ Terbatas | ⚠️ Terbatas | **✅ Lengkap (30+ Metode)** |
| **Expandable Blockquote & Time Tags** | ❌ | ⚠️ Manual Parse | **✅ Bawaan (`<tg-time>`, Blockquote)** |
| **Message Effects (`effect_id`)** | ❌ | ❌ / Parsial | **✅ Lengkap** |
| **Built-in Pyromod (`ask` / `listen`)** | ❌ Butuh plugin luar | ❌ Tidak ada | **✅ Terpasang Langsung** |
| **Helper Formatter Teks (`client.bold`)** | ❌ | ❌ | **✅ Terintegrasi** |
| **Smart Inline Keyboard (`ikb`, `btn`)** | ❌ | ❌ | **✅ Terintegrasi** |
| **Proteksi Kebocoran Memori (LRU)** | ❌ Rentan Leak | ⚠️ Parsial | **✅ Teruji & Stabil** |
| **Tracked Asyncio Tasks** | ❌ Rentan GC Drop | ⚠️ Parsial | **✅ Aman dari GC Interrupt** |

---

## ⚙️ Konfigurasi Lanjutan

### Mengatur Timeout Pyromod Secara Global
Anda dapat mengatur konfigurasi default percakapan melalui `PyromodConfig`:

```python
from pyrogram.utils import PyromodConfig

# Mengubah pesan default saat batas waktu interaksi terlampaui
PyromodConfig.timeout_handler = None  # Atau pasang callback khusus
```

---

## 🤝 Komunitas & Dukungan

Jangan ragu untuk bergabung dengan komunitas pengembang kami:

* 📢 **Kanal Pembaruan:** [@Renboyz](https://t.me/Renboyz)
* 💬 **Grup Diskusi:** [@RNMarkets](https://t.me/RNMarkets)
* 🐛 **Pelaporan Masalah / Bug:** [GitHub Issues](https://github.com/renzetx/RNGram/issues)
* 📖 **Referensi Dokumentasi Asli:** [Pyrogram Documentation](https://docs.pyrogram.org)

---

## 📜 Lisensi & Atribusi

**RNGram** dilisensikan di bawah ketentuan **[GNU Lesser General Public License v3.0 or later (LGPLv3+)](COPYING.lesser)**.

```
Copyright (C) 2017-present Dan <https://github.com/delivrance>
Copyright (C) 2024-present KurimuzonAkuma <https://github.com/KurimuzonAkuma>
Copyright (C) 2024-present Renboys <https://github.com/renzetx>
```

<p align="center">
  Dikelola dengan ❤️ oleh <b><a href="https://t.me/Renboyz">Renboys</a></b> bersama Komunitas Open Source.
</p>
