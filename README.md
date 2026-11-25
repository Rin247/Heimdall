# Heimdall — File Manager, Archive Hub & Wireless Server Stack

Heimdall is a powerful, offline-first Android file manager, archive extractor, and local wireless server hub. Built with Kotlin, Jetpack Compose, Material 3, and native C++ `libarchive`, Heimdall combines dual-pane file management, cloud/network storage protocols, and local file servers (HTTP / SFTP / WebDAV) into a privacy-first mobile utility.

---

## 📂 Key Features & Subsystem Breakdown

### 📁 Multi-Tab & Dual-Pane File Explorer (`explorer`)
- **Current**: Storage Access Framework (SAF) integration, root file system access, multi-tab layout, batch copy/move/rename, and storage space analyzer.
- **Planned / Roadmap**: Dual-pane drag-and-drop side-by-side mode, file checksum calculator (MD5/SHA256), and file tagger.

### 📦 Native Archive Engine (`archive`)
- **Current**: In-place archive extraction, creation, and browsing for ZIP, TAR, GZ, BZ2, XZ, 7Z, and RAR formats via native `libarchive`.
- **Planned / Roadmap**: Encrypted archive creation (AES-256), split multi-part archive support, and archive repair tool.

### 🌐 Network Clients & Local Servers (`server`)
- **Current**: SMBv2/v3, SFTP, FTP, and WebDAV client connections; local HTTP file server and WebDAV server host.
- **Planned / Roadmap**: High-speed P2P Wi-Fi Direct file transfers, DLNA/UPnP media server, and background sync manager.

### 🔍 Built-In Preview & Viewers (`viewers`)
- **Current**: Syntax-highlighted code/text editor, hex viewer, image inspector with EXIF data, and PDF reader.
- **Planned / Roadmap**: Audio/Video stream player with subtitle support, Markdown live preview, and APK manifest inspector.

---

## 🏗️ Architecture & Technology Stack

- **Platform**: Android 13+ (minSdk 33, targetSdk 37).
- **UI & Layout**: Kotlin, Jetpack Compose, Material 3.
- **Native Core**: C++ NDK `libarchive` integration.
- **Network Stack**: SMBJ, SSHJ, NanoHTTPd, WebDAV server.
- **Licensing**: AGPL-3.0.

---

## 🛠️ Building & Running

```bash
./gradlew assembleDebug
./gradlew installDebug
```

---

## 📜 License

Heimdall is released under the **GNU Affero General Public License v3.0** (AGPL-3.0). See [`LICENSE`](LICENSE) for details.
