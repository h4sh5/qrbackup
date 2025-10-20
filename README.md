# QRBackup

Backup and restore data on paper using base45 encoding for maximum efficiency. Browser only web app using WebAssembly; no server-side processing required.

Stores about 65KB of data per A4 page.

## Usage

### Backup

Use the github page URL, or serve this on a server and browse to index.html (opening of the html file directly without serving may not work due to CORS, so serve on localhost using something like `python3 -m http.server`). Select the file to backup and then print the page out on a laser printer at around 600 dpi.

### Restore

Scan all pages containing the QR codes using at least 600 dpi and preferably in color to PNG files (other image types may also work). Browse to restore.html and select those scanned images, type in the filename you wish to save it to, then hit restore and wait a few seconds; it may take longer on large files.

## Credits

fast_qr for QR code generation: https://github.com/erwanvivien/fast_qr

zbar-wasm for QR code scanning: https://github.com/undecaf/zbar-wasm
