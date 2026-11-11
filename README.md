# Flutter Navigation Task

This project is a small Flutter application created for a navigation exercise. It contains two screens:

- **First Page** displays a **Next** button. Pressing it opens the second page.
- **Second Page** displays a **Return** button. Pressing it closes the second page and returns to the first page.

The app uses named routes in `MaterialApp`. `Navigator.pushNamed()` opens the second page, and `Navigator.pop()` returns to the previous page.

## Requirements

- Flutter SDK installed and available in `PATH`.
- For Android: Android SDK installed and Android licenses accepted.
- For Linux desktop: Flutter's Linux desktop build dependencies installed.
- For Android phone testing: USB debugging enabled and this computer authorized on the phone.

## Check available devices

From the project directory, run:

```bash
flutter devices
```

Example devices:

```text
SM S711B (mobile) • RZCX90XERJT • android-arm64 • Android 16 (API 36)
Linux (desktop)   • linux       • linux-x64     • Fedora Linux
```

## Run on Linux desktop

```bash
flutter run -d linux
```

## Run on an Android phone

Connect the phone by USB, enable **Developer options → USB debugging**, unlock it, and accept the **Allow USB debugging?** prompt. Confirm that `flutter devices` lists the phone, then run:

```bash
flutter run -d RZCX90XERJT
```

Replace `RZCX90XERJT` with the device ID shown by `flutter devices` if it differs. If `adb devices` shows `unauthorized`, accept the authorization prompt on the phone and check again.

## Run in a web browser

Start Flutter's web server:

```bash
flutter run -d web-server
```

Flutter prints a local URL in the terminal. Open that URL in a browser, such as Firefox. The `web-server` device has limited debugging support compared with Chrome, but it can be used to view and test the app.

To stop the running app, press `q` in the terminal where `flutter run` is running.
