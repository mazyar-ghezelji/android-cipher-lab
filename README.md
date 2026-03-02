## Android Cipher Lab

An Android app demonstrating classic symmetric cryptography algorithms and modes of operation. The app lets you experiment with:

- **Algorithms**: DES, 3DES (DESede), AES
- **Block modes**: CBC, CFB, ECB

It provides simple screens for **encryption** and **decryption**, so you can see how different algorithm/mode combinations behave in practice.

---

## Project structure

- **`app/`**: Main Android app module
- **`app/src/main/java/mazyar/crypto/`**
  - `MainActivity.java` – landing screen where you choose to encrypt or decrypt
  - `encrypt.java` – encryption screen that lets you pick the algorithm and mode, enter plaintext, and generate ciphertext
  - `decrypt.java` – decryption screen that uses the previously generated key and parameters to recover the plaintext

---

## Getting started

**Prerequisites**

- Android Studio (Arctic Fox or newer recommended)
- Android SDK and build tools installed

**Open the project**

1. Start Android Studio.
2. Choose **“Open an existing project”**.
3. Select the repository root directory.
4. Let Gradle sync and download any required dependencies.

**Run on a device or emulator**

1. Connect an Android device with USB debugging enabled, or start an emulator.
2. In Android Studio, select the `app` configuration.
3. Click **Run** to build and install the app.

---

## Using the app

- **Main screen**
  - Navigate to **Encrypt** or **Decrypt**.

- **Encrypt screen**
  - Choose an **algorithm** (DES / 3DES / AES).
  - Choose a **mode** (CBC / CFB / ECB).
  - Enter the plaintext you want to encrypt.
  - Tap **Encrypt** to generate ciphertext.

- **Decrypt screen**
  - Reuse the same algorithm/mode selection and key that were used for encryption.
  - Tap **Decrypt** to recover and view the plaintext.

> **Note**: This app is intended for learning and experimentation, not for production‑grade security.

---

## Development notes

- Java source code is in `app/src/main/java/mazyar/crypto/`.
- Layout XML files are in `app/src/main/res/layout/`.
- Common Android build artifacts (`build/`, `.gradle`, `.idea`, etc.) are ignored via `.gitignore`.

If you update Gradle, Android Gradle Plugin, or target SDK versions, make sure the project still builds cleanly on a fresh checkout.


