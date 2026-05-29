# Flash Game Launcher

En sevdiğiniz `.swf` uzantılı Flash oyunlarını düzenlemek ve oynamak için tasarlanmış modern, karanlık temalı bir masaüstü uygulamasıdır. Python ve PyQt6 ile geliştirilmiştir.

🌍 *[Read this in English](README.md)*

## Özellikler

- **Modern Arayüz**: Göz yormayan karanlık tema ve ekran boyutuna göre şekil alan duyarlı (responsive) ızgara tasarımı.
- **Otomatik Algılama**: `swf_files` klasöründeki tüm `.swf` oyunlarını otomatik olarak bulur ve listeler.
- **Oyun Kapak Resimleri**: Oyunlarınız için otomatik kapak resmi desteği. `.swf` dosyanızla tamamen aynı isme sahip bir resmi (örn. `.png`, `.jpg`, `.webp`) `swf_files` klasörüne atmanız yeterlidir.
- **Otomatik Güncelleme (In-App Updater)**: Program, GitHub üzerinden yeni bir sürüm olup olmadığını kontrol eder. Yeni sürüm varsa arka planda indirir, eski programın yerine yenisini koyar ve otomatik olarak yeniden başlar.
- **Taşınabilir (Standalone)**: PyInstaller kullanılarak tek bir `.exe` dosyası haline kolayca getirilebilir.

## Nasıl Kullanılır?

1. **İndirin**: [Releases](../../releases) sayfasından en son yayınlanan `.exe` dosyasını indirin.
2. **Oyunlarınızı Yükleyin**:
   - Uygulamayı bir kez çalıştırın. Bulunduğu dizine otomatik olarak `swf_files` klasörünü oluşturacaktır.
   - Oynamak istediğiniz Flash oyunlarını (`.swf`) bu klasörün içine atın.
   - (İsteğe bağlı) Kapak resimlerini de aynı isimle klasöre ekleyebilirsiniz (örnek: `ates_ve_su.swf` ve `ates_ve_su.png`).
3. **Oynayın**: Listedeki herhangi bir oyunun altındaki "Play" butonuna basarak anında oynamaya başlayabilirsiniz.

## Kaynak Koddan Derleme (Geliştiriciler İçin)

### Gereksinimler
- Python 3.10+
- `pip`

### Kurulum
1. Repoyu bilgisayarınıza klonlayın:
   ```bash
   git clone https://github.com/BartuAbiHD/FlashGameLauncher.git
   cd FlashGameLauncher
   ```
2. Gerekli kütüphaneleri yükleyin:
   ```bash
   pip install -r requirements.txt
   ```
3. Uygulamayı çalıştırın:
   ```bash
   python main.py
   ```

### Executable (.exe) Oluşturma
Windows için tek parça `.exe` dosyası oluşturmak istiyorsanız:
```bash
build.bat
```
Bu komut otomatik olarak bir sanal ortam (`.venv`) kuracak, gerekli paketleri indirecek ve `main.spec` dosyasını kullanarak uygulamanızı paketleyecektir.

## Telif Hakkı
© 2026 BartuAbiHD. Tüm hakları saklıdır.
