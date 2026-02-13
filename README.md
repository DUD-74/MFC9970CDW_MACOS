# Brother MFC-9970CDW PPD for macOS and Linux

This repository contains a functional **PPD (PostScript Printer Description)** file for the **Brother MFC-9970CDW** multi-function printer. 

While Brother has officially discontinued driver support for newer versions of macOS (including macOS 12 Monterey, 13 Ventura, 14 Sonoma, and 15 Sequoia), this PPD file allows you to continue using the printer via the standard CUPS interface or manual printer setup.

## 🚀 Features
- **Full Compatibility:** Works with macOS (Intel and Apple Silicon) and Linux.
- **Native Resolution:** Supports all standard DPI settings of the MFC-9970CDW.
- **Duplex Printing:** Full support for automatic double-sided printing.
- **Tray Management:** Correct mapping for multi-purpose and standard paper trays.

## 🛠 Installation (macOS)

1. **Download** the `BR9970_2.PPD` (or similar filename) from this repository.
2. Go to **System Settings** > **Printers & Scanners**.
3. Click **Add Printer, Scanner, or Fax...**.
4. Select the **Brother MFC-9970CDW** from the list (ensure it is connected via Network or USB).
5. In the **Use** dropdown menu, do not select "Auto Select". Instead, choose **"Other..."**.
6. Browse to and select the downloaded `.ppd` file.
7. Click **Add**.

## 🐧 Installation (Linux / CUPS)

Copy the PPD file to your local CUPS model directory:
```bash
sudo cp your-file.ppd /usr/share/cups/model/
sudo systemctl restart cups
