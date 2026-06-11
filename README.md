Kiosk Mode Enterprise 🛡️
Kiosk Mode Enterprise is a robust, professional Android launcher designed for corporate and delivery devices. It transforms any Android smartphone into a strictly controlled, locked-down terminal, ensuring employees only access authorized applications.
Designed and engineered by Max Meloman aka Deadguf.
🌟 Key Features
•
Total Lockdown (Device Owner): Leveraging Android's DevicePolicyManager to take full control of the device security.
•
App Whitelisting: Granular control over which apps are visible and launchable.
•
Hidden Admin Entry: No visible "Settings" button. Access is granted via a secret "Z" gesture drawn on the home screen.
•
Maintenance Mode: A dedicated service mode (unlocked via Master Password) that temporarily lifts all restrictions for updates or troubleshooting.
•
Dual-Layer Security:
◦
Admin PIN: For daily app management.
◦
Master Password: Alphanumeric password for critical system-level toggles.
•
Smart Kiosk UI:
◦
Restricted status bar (notifications only, no settings).
◦
Customizable "Home" button behavior.
◦
Support for "Recent Apps" and "Quick Switching" between allowed tasks.
•
Multi-Language Support: Fully localized in English, Russian, German, and Armenian.
🚀 Installation & Setup
1. Initial Setup
1.
Install the APK on a fresh device (or a device with no accounts signed in).
2.
Enable USB Debugging in Developer Options.
2. Activate Device Owner Mode
Connect the device to your PC and run the following ADB command. This is required to enable the high-level lockdown features:
Shell Script
adb shell dpm set-device-owner com.maxmeloman.kioskmode/.KioskAdminReceiver
3. Configure the Kiosk
1.
Draw a "Z" gesture on the main screen.
2.
Enter the default Admin PIN: 1234.
3.
Go to Control Panel -> Home Screen to set the app as the default launcher.
4.
Use the Select Applications menu to whitelist your workflow apps.
🔧 Technical Specifications
•
Architecture: 100% Kotlin with Jetpack Compose.
•
Minimum SDK: Android 11 (API 30).
•
UI Framework: Material 3.
•
Storage: Secure local storage via encrypted/private SharedPreferences.
🔐 Default Credentials
•
Admin PIN: 1234 (Numeric)
•
Master Password: 5555 (Alphanumeric)
Note: It is highly recommended to change both passwords immediately after the first setup through the Control Panel.
