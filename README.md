# Kickly v0.4 - Standalone Release & New Features / Bağımsız Sürüm ve Yeni Özellikler 🚀

[![Release](https://img.shields.io/github/v/release/YourAnonELF/Kickly?label=Release&style=for-the-badge)](https://github.com/YourAnonELF/Kickly/releases)
[![Actions](https://img.shields.io/github/actions/workflow/status/YourAnonELF/Kickly/release.yml?branch=main&label=Actions&style=for-the-badge)](https://github.com/YourAnonELF/Kickly/actions)
[![License](https://img.shields.io/github/license/YourAnonELF/Kickly?label=License&style=for-the-badge)](LICENSE)

We are excited to announce **Kickly v0.4**! This release transforms Kickly into a fully standalone application, meaning you no longer need to install Python to run it. We've also added powerful new features like the Gift Leaderboard and Interactive Mode.

**Kickly v0.4** sürümünü duyurmaktan heyecan duyuyoruz! Bu sürümle Kickly tamamen bağımsız bir uygulamaya dönüştü; artık çalıştırmak için Python yüklemenize gerek yok. Ayrıca Hediye Lider Tablosu ve Etkileşim Modu gibi güçlü yeni özellikler ekledik.

---

## ✨ New Features / Yeni Özellikler

### 📦 Standalone Executables / Bağımsız Uygulamalar
Kickly is now packaged into 3 easy-to-run files. No coding knowledge required!
Kickly artık çalıştırılması kolay 3 dosya halinde paketlendi. Kodlama bilgisi gerekmez!
- **Kickly Backend.exe**: Connects to Kick.
- **Kickly Overlay.exe**: The transparent chat overlay.
- **Kickly Config.exe**: Settings manager.

### 👑 Gift Leaderboard / Hediye Lider Tablosu
- **Top Gifter Display**: The overlay now automatically detects and displays the top gifter of the session in **Gold** text in the header.
- **En Çok Hediye Gönderen**: Overlay artık oturumun en çok hediye gönderenini (Top Gifter) otomatik olarak algılar ve başlıkta **Altın** rengiyle gösterir.

### 🎮 Interactive Mode / Etkileşim Modu (`Alt + N`)
- **Toggle Interaction**: Press `Alt + N` to switch between "Click-Through" (Game Mode) and "Interactive Mode".
- **Features**: In Interactive Mode, you can type in chat, click buttons, and scroll through message history.
- **Etkileşim Geçişi**: "Tıklama Geçişi" (Oyun Modu) ve "Etkileşim Modu" arasında geçiş yapmak için `Alt + N` tuşlarına basın.
- **Özellikler**: Etkileşim modunda sohbete yazı yazabilir, butonlara tıklayabilir ve mesaj geçmişini kaydırabilirsiniz.

### ⚡ Config Hot-Reload / Anında Ayar Yenileme
- **Instant Updates**: Change your theme, opacity, window size, or position using `Kickly Config.exe`, and the Overlay will update **instantly** without restarting.
- **Anında Güncelleme**: `Kickly Config.exe` kullanarak temanızı, opaklığı, pencere boyutunu veya konumunu değiştirin; Overlay yeniden başlatmaya gerek kalmadan **anında** güncellenir.

---

## 🛠️ Technical Improvements / Teknik İyileştirmeler

- **PyInstaller Support**: Fixed compatibility issues with `rich` and `colorama` libraries to ensure smooth packaging. / Paketleme sorunlarını gidermek için `rich` ve `colorama` kütüphaneleriyle ilgili uyumluluk sorunları çözüldü.
- **Websockets Fix**: Downgraded to `websockets==12.0` to resolve build errors. / Derleme hatalarını çözmek için `websockets` sürümü `12.0`'a düşürüldü.
- **Refactoring**: Centralized channel logic for better stability. / Daha iyi kararlılık için kanal mantığı merkezileştirildi.

---

## 📥 How to Update / Nasıl Güncellenir?

1.  Download the `v0.4` ZIP file from Releases. / Releases kısmından `v0.4` ZIP dosyasını indirin.
2.  Extract to a folder. / Bir klasöre çıkartın.
3.  Run `Kickly Backend.exe` first, then `Kickly Overlay.exe`. / Önce `Kickly Backend.exe`, sonra `Kickly Overlay.exe` çalıştırın.
