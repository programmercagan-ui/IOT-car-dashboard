# 🚗 ESP32 OBD Dashboard & Shift Light

ESP32 tabanlı **akıllı araç dashboard ve shift light sistemi**.  
OBD üzerinden gerçek zamanlı motor verilerini okuyarak **TFT ekranda gösterir** ve **WS2812 LED shift light** ile vites değiştirme uyarısı verir.

Proje ayrıca **WiFi üzerinden ayarlanabilen bir web paneli** içerir.

Bu cihaz **universal olarak tasarlanmıştır** ve OBD-II destekleyen çoğu araç ile çalışabilir.

---

# 📸 Features

### 🏎️ Dashboard

4 farklı ekran modu içerir:

- Minimal Dashboard
- Classic Dashboard
- Race Dashboard
- Telemetry Screen

Gerçek zamanlı gösterilen veriler:

- RPM
- Speed
- Gear (calculated)
- Boost

Session verileri:

- Max RPM
- Max Speed
- Max Boost

---

# 📊 Telemetry Data

OBD üzerinden okunan gelişmiş araç verileri:

- Engine Load
- Throttle Position
- MAF Flow
- Battery Voltage
- Coolant Temperature
- Intake Temperature
- Ambient Temperature
- Fuel Level
- DPF Load
- Engine Runtime

---

# 💡 Shift Light System

WS2812 LED strip ile **yarış tipi vites uyarı sistemi**.

Desteklenen modlar:

- Gunluk Mode
- Linear Mode
- Cadde Mode
- Sport Mode
- Reverse Mode
- Aero Strobe
- Knight Rider
- Demo Rainbow
- Heartbeat
- Cyberpunk Glitch
- Rain Drop

LED parlaklığı ve RPM aralıkları **web panelinden ayarlanabilir**.

---

# 🌐 Web Control Panel

ESP32 WiFi üzerinden **web paneli açar**.

Panelden ayarlanabilen özellikler:

- Shift light modu
- RPM başlangıç değeri
- Yeşil / Sarı / Kırmızı RPM aralıkları
- LED parlaklığı
- Strobe hızı
- Fake RPM test mode

Eğer araç OBD bağlantısı kurulamazsa **20 saniye sonra otomatik Access Point açılır.**

WiFi adı:

EGEA_SHIFT_LIGHT

Şifre:

12345678

---

# 🧠 Technologies Used

- ESP32
- ELM327 / V-LINK OBD Adapter
- TFT_eSPI
- FastLED
- FreeRTOS Tasks
- ESP32 WebServer
- EEPROM storage

---

# 🔌 Hardware

Gerekli parçalar:

- ESP32
- 320x240 TFT Display (ILI9341)
- WS2812 LED strip (8 LED)
- OBD Adapter (ELM327 / V-LINK)
- Button (dashboard değiştirmek için)

---

# ⚙️ Pin Configuration

| Component | Pin |
|-----------|-----|
| LED Strip | GPIO 5 |
| Button | GPIO 4 |
| TFT | TFT_eSPI config |

---

# 🎮 Controls

### Button Controls

| Action | Function |
|-------|----------|
| Single Click | Dashboard change |
| Double Click | LED mode change |
| Hold 5 seconds | Brightness toggle |

---

# 🧪 Test Mode

Web panelinden **Fake RPM** aktif edilebilir.

Bu mod:

- Araç bağlı değilken
- LED ve ekran test etmek için kullanılır.

---

# 👨‍💻 Developer

Cagan Derindere

MIS Student  
Embedded Systems & Software Developer

---

# ⚠️ Note

Bu proje **OBD-II destekleyen araçlarla çalışacak şekilde universal tasarlanmıştır.**

Bazı araçlarda belirli OBD PID değerleri farklı olabilir.

---

# ⭐ Support

Projeyi beğendiysen **GitHub Star ⭐ vermeyi unutma.**
