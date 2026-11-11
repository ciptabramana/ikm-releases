# IKM releases

Installer packages for **IKM** (Survei Indeks Kepuasan Masyarakat, PermenPANRB 14/2017): respondents answer the 9 service-element questions on registered tablets, and the admin page shows the IKM per period and per loket (service counter), with print and CSV export. IKM runs on one server PC in your own network.

This repository holds no source code. Download a package from **Releases**.

## Which file

| File | Server PC |
|---|---|
| `ikm-<version>-windows.zip` | Windows 10/11 |
| `ikm-<version>-linux.zip` | Linux |

## Install or update

1. Install Docker (Docker Desktop on Windows).
2. Unzip into a folder named `ikm`. An update unzipped over it keeps the server's own `.env`.
3. Run `install.bat` (Windows) or `install.sh` (Linux).
4. Open `http://<server>:8880/#/admin` and activate the license with the key from your supplier.

`SERVER_GUIDE.md` and `USER_GUIDE.md` in the zip explain the rest (Bahasa Indonesia: `SERVER_GUIDE.id.md`, `USER_GUIDE.id.md`).

## License

IKM is proprietary software. Copyright (c) 2026 Cipta Bramana. All rights reserved.

Each installation needs a license key for its server PC and number of tablets, from the Licensor or an authorized supplier. Use is governed by the [IKM Software License Agreement](LICENSE) (Bahasa Indonesia and English; the Indonesian text prevails). In short: you may run IKM on the licensed server and its connected devices for your own service units' satisfaction surveys; you may not copy, modify, reverse engineer, resell, or redistribute it, or bypass the license check. Open-source components keep their own licenses, listed in [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).

Support, installation and license renewals: contact your IKM supplier.
