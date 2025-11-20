# Kickly — Advanced Kick.com Stream Overlay 🚀

![Kickly Banner](assets/kicklyLogo.png)

[![Release](https://img.shields.io/github/v/release/OWNER/REPO?label=release&style=for-the-badge)](https://github.com/OWNER/REPO/releases)
[![Actions](https://img.shields.io/github/actions/workflow/status/OWNER/REPO/release.yml?branch=main&style=for-the-badge)](https://github.com/OWNER/REPO/actions)
[![License](https://img.shields.io/github/license/OWNER/REPO?style=for-the-badge)](LICENSE)

Kickly is a lightweight, standalone stream overlay tailored for Kick.com streamers. It provides a transparent, click-through chat overlay with features such as Gift Leaderboards, Interactive Mode, and hot-reload configuration.

Kickly, Kick.com yayıncıları için özel tasarlanmış, hafif ve bağımsız bir yayın katmanıdır. Şeffaf, tıklama geçişli (click-through) sohbet penceresi, Hediye Lider Tablosu, Etkileşim Modu ve anlık yapılandırma (hot-reload) gibi özellikler sunar.

---

## Table of contents / İçindekiler
- Features / Özellikler
- Quick demo / Hızlı demo
- Installation / Kurulum
- Usage / Kullanım
- Components / Bileşenler
- Configuration & Themes / Yapılandırma ve Temalar
- Hotkeys / Kısayollar
- Releases / Sürüm Yayınlama
- Troubleshooting / Sorun Giderme
- Contributing / Katkıda Bulunma
- Changelog / Değişiklikler
- License / Lisans

---

## 🌟 Features / Özellikler

- Transparent overlay — Chat floats over the game without blocking view.  
  Şeffaf overlay — Sohbet oyununuzun üzerinde, görüşü engellemeden görünür.
- Click-through — Clicks pass through to the game window.  
  Tıklama geçişi — Tıklamalar doğrudan oyuna iletilir.
- Interactive Mode (Alt+N) — Enable to type messages or interact with controls.  
  Etkileşim Modu (Alt+N) — Sohbet yazmak veya kontrollerle etkileşim için.
- Gift Leaderboard — Highlights top gifters in real time.  
  Hediye Lider Tablosu — En çok hediye gönderenleri canlı olarak vurgular.
- Hot-reload configuration — Changes apply instantly without restarting the overlay.  
  Canlı ayarlar — Değişiklikler overlay'i yeniden başlatmadan anında uygulanır.
- Theme support via `.qss` files — Fully customizable appearance.  
  `.qss` tema desteği — Görünüm tamamen özelleştirilebilir.

---

## 📺 Quick demo / Hızlı demo

![demo gif](docs/demo.gif)

---

## 📦 Installation / Kurulum

1. Download the official release assets from the GitHub Releases page.  
   Resmi sürüm paketlerini GitHub Releases sayfasından indirin.
2. Extract the ZIP file to a folder (e.g., Desktop).  
   ZIP dosyasını bir klasöre çıkarın (örn. Masaüstü).
3. Run the executables in this order:
   - Kickly Backend.exe — start FIRST (a browser window may open for authentication).  
     Backend.exe — ÖNCE çalıştırın (giriş için tarayıcı penceresi açılabilir).
   - Kickly Overlay.exe — start SECOND (after backend connection).  
     Overlay.exe — BACKEND bağlandıktan SONRA çalıştırın.
   - Kickly Config.exe — optional, can be opened anytime to edit themes and settings.  
     Config.exe — İsteğe bağlı, temaları ve ayarları düzenlemek için her zaman açılabilir.

Note: Distribute releases with versioned filenames (e.g., `kickly-v1.2.0-windows.zip`) and include checksums for integrity when possible.

---

## 🚀 Usage / Kullanım

1. Run Kickly Backend.exe and authenticate on Kick.com if prompted.  
   Backend’i başlatın ve gerekiyorsa Kick.com ile kimlik doğrulaması yapın.
2. Run Kickly Overlay.exe once the backend is connected; ensure the game is in Windowed or Borderless Windowed mode.  
   Backend bağlıyken Overlay’i başlatın; oyunun Pencereli veya Çerçevesiz Pencereli modda olduğundan emin olun.
3. Toggle Interactive Mode with Alt + N to type messages or click controls.  
   Etkileşim Modunu açıp kapatmak için Alt + N tuşunu kullanın.

---

## 🔧 Components / Bileşenler

- Kickly Backend.exe — Connects to Kick.com and streams chat events.  
  Kickly Backend — Kick.com ile bağlantı kurup sohbet verilerini alır.
- Kickly Overlay.exe — Renders the transparent chat overlay and leaderboard.  
  Kickly Overlay — Şeffaf sohbet katmanını ve lider tablosunu gösterir.
- Kickly Config.exe — Theme and settings manager with hot-reload.  
  Kickly Config — Tema ve ayar yöneticisi (anında uygulama).

---

## 🎨 Configuration & Themes / Yapılandırma ve Temalar

- Themes are stored as `.qss` files in `/themes`. Edit and save to apply changes live.  
  Temalar `/themes` içinde `.qss` dosyaları olarak bulunur. Düzenleyip kaydedildiğinde değişiklikler anında uygulanır.
- Keep font sizes and contrast accessible for viewers.

---

## ⌨️ Hotkeys / Kısayollar

- Alt + N — Toggle Interactive Mode (type messages, click controls).  
  Alt + N — Etkileşim Modu aç/kapat.
- Additional hotkeys can be customized via Kickly Config.exe.  
  Ek kısayollar Kickly Config.exe üzerinden özelleştirilebilir.

---


## ⚠️ Troubleshooting / Sorun Giderme

- Anti-Virus false positives: Packaged Python apps (PyInstaller) can trigger AV heuristics. Add the Kickly folder to AV exclusions if a false positive occurs.  
  Antivirüs uyarıları: PyInstaller ile paketlenmiş Python uygulamaları bazen AV tarafından işaretlenir. Yanlış pozitif durumunda Kickly klasörünü dışlamalara ekleyin.
- Overlay not visible: Ensure the game runs in Windowed or Borderless Windowed mode; exclusive fullscreen may hide overlays.  
  Overlay görünmüyorsa: Oyunu Pencereli veya Çerçevesiz Pencereli modda çalıştırın; Tam Ekran modu overlay'i gizleyebilir.
- Backend connection lost: Restart Kickly Backend.exe and verify network connectivity.  
  Backend bağlantısı kesildiyse: Backend.exe'yi yeniden başlatın ve ağ bağlantısını kontrol edin.

---

## 🤝 Contributing / Katkıda Bulunma

Contributions are welcome. Suggested workflow:
1. Fork the repository.  
2. Create a branch: `git checkout -b feat/your-feature`.  
3. Use Conventional Commits (feat:, fix:, chore:) and include clear PR descriptions.  
4. Open a Pull Request for review.

---

## 🧾 Changelog / Değişiklikler

Maintain a `CHANGELOG.md` using `standard-version` or `semantic-release` conventions to keep release notes structured and readable.

---

## License / Lisans

MIT License — Free to use, modify, and distribute.  
MIT Lisansı — Kullanımı, değiştirilmesi ve dağıtımı serbesttir.

---
