# Kiosk Mode Enterprise 🛡️

**Kiosk Mode Enterprise** is a robust, professional Android launcher designed for corporate and delivery devices. It transforms any Android smartphone into a strictly controlled, locked-down terminal, ensuring employees only access authorized applications.

> 💖 **100% Free & Ad-Free Forever**  
> This project is completely free, contains absolutely no ads, and will remain this way forever. If you find this tool useful and want to support its development, you can do so here:  
> 👉 [Support the project on DonationAlerts](https://www.donationalerts.com/r/maxmeloman)

*Designed and engineered by Max Meloman aka Deadguf.*

---

### 🌟 Key Features
- **Total Lockdown (Device Owner):** Leverages Android's `DevicePolicyManager` to take full control of device security.
- **App Whitelisting:** Granular control over which apps are visible and launchable.
- **Hidden Admin Entry:** No visible "Settings" button. Access is granted via a secret **"Z"** gesture drawn on the home screen.
- **Maintenance Mode:** A dedicated service mode (unlocked via Master Password) that temporarily lifts all restrictions for updates or troubleshooting.
- **Dual-Layer Security:**
  - **Admin PIN:** For daily app management.
  - **Master Password:** Alphanumeric password for critical system-level toggles.
- **Smart Kiosk UI:**
  - Restricted status bar (notifications only, no settings).
  - Customizable "Home" button behavior.
  - Support for "Recent Apps" and "Quick Switching" between allowed tasks.
- **Multi-Language Support:** Fully localized in English, Russian, German, and Armenian.

---

### 🚀 Installation & Setup

#### 1. Initial Setup
1. Install the APK on a fresh device (or a device with no accounts signed in).
2. Enable **USB Debugging** in Developer Options.

#### 2. Activate Device Owner Mode
Connect the device to your PC and run the following ADB command. This is required to enable the high-level lockdown features:
```shell
adb shell dpm set-device-owner com.maxmeloman.kioskmode/.KioskAdminReceiver
```

#### 3. Configure the Kiosk
1. Draw a **"Z"** gesture on the main screen.
2. Enter the default Admin PIN: `1234`.
3. Go to **Control Panel -> Home Screen** to set the app as the default launcher.
4. Use the **Select Applications** menu to whitelist your workflow apps.

---

### 🔧 Technical Specifications
- **Architecture:** 100% Kotlin with Jetpack Compose.
- **Minimum SDK:** Android 11 (API 30).
- **UI Framework:** Material 3.
- **Storage:** Secure local storage via encrypted/private `SharedPreferences`.

---

### 🔐 Default Credentials
- **Admin PIN:** `1234` (Numeric)
- **Master Password:** `5555` (Alphanumeric)

> ⚠️ **Note:** It is highly recommended to change both passwords immediately after the first setup through the Control Panel.

---

### 👨‍💻 Author
Engineered by **Max Meloman** aka **Deadguf**  
*Enterprise Kiosk Solutions © 2026*

# Kiosk Mode Enterprise 🛡️

**Kiosk Mode Enterprise** — это надежный и профессиональный лаунчер для Android, разработанный для корпоративных и курьерских устройств. Он превращает любой смартфон на Android в строго контролируемый, заблокированный терминал, гарантируя, что сотрудники имеют доступ только к авторизованным приложениям.

> 💖 **100% Бесплатно и без рекламы навсегда**  
> Этот проект полностью бесплатный, не содержит абсолютно никакой рекламы и останется таким навсегда. Если этот инструмент оказался для вас полезным и вы хотите поддержать его разработку, вы можете сделать это здесь:  
> 👉 [Поддержать проект на DonationAlerts](https://www.donationalerts.com/r/maxmeloman)

*Разработано и создано Max Meloman (aka Deadguf).*

---

### 🌟 Ключевые особенности
- **Полная блокировка (Device Owner):** Использует `DevicePolicyManager` Android для получения полного контроля над безопасностью устройства.
- **Белый список приложений:** Тонкая настройка того, какие приложения видны и могут быть запущены.
- **Скрытый вход для администратора:** Никаких видимых кнопок «Настройки». Доступ предоставляется через секретный жест **«Z»**, нарисованный на главном экране.
- **Режим обслуживания:** Специальный сервисный режим (разблокируется через Мастер-пароль), который временно снимает все ограничения для обновлений или устранения неполадок.
- **Двухуровневая защита:**
  - **PIN-код администратора:** Для ежедневного управления приложениями.
  - **Мастер-пароль:** Буквенно-цифровой пароль для критических системных переключателей.
- **Умный интерфейс киоска:**
  - Ограниченная строка состояния (только уведомления, без настроек).
  - Настраиваемое поведение кнопки «Домой».
  - Поддержка «Недавних приложений» и «Быстрого переключения» между разрешенными задачами.
- **Многоязычная поддержка:** Полная локализация на английский, русский, немецкий и армянский языки.

---

### 🚀 Установка и настройка

#### 1. Начальная подготовка
1. Установите APK на чистое устройство (или на устройство, в котором не выполнен вход в аккаунты).
2. Включите **Отладку по USB** в меню «Для разработчиков».

#### 2. Активация режима Device Owner
Подключите устройство к ПК и выполните следующую команду ADB. Это необходимо для включения функций блокировки высокого уровня:
```shell
adb shell dpm set-device-owner com.maxmeloman.kioskmode/.KioskAdminReceiver
```

#### 3. Настройка киоска
1. Нарисуйте жест **«Z»** на главном экране.
2. Введите PIN-код администратора по умолчанию: `1234`.
3. Перейдите в **Панель управления -> Главный экран**, чтобы установить приложение в качестве лаунчера по умолчанию.
4. Используйте меню **Выбор приложений**, чтобы добавить необходимые рабочие приложения в белый список.

---

### 🔧 Технические характеристики
- **Архитектура:** 100% Kotlin с использованием Jetpack Compose.
- **Минимальный SDK:** Android 11 (API 30).
- **UI-фреймворк:** Material 3.
- **Хранение данных:** Безопасное локальное хранилище через зашифрованные/приватные `SharedPreferences`.

---

### 🔐 Учетные данные по умолчанию
- **PIN-код администратора:** `1234` (числовой)
- **Мастер-пароль:** `5555` (буквенно-цифровой)

> ⚠️ **Примечание:** Настоятельно рекомендуется изменить оба пароля сразу после первой настройки через Панель управления.

---

### 👨‍💻 Автор
Разработано **Max Meloman** (aka **Deadguf**)  
*Enterprise Kiosk Solutions © 2026*
