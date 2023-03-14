# Bkebi Pengantar

| **NAMA FILE/FOLDER**      | **PENJELASAN**       |
|:-----------------:|:------------:|
| BKEBI-ISFREE-NOT4SALE.LIC  | FILE LISENSI  |
| injector\.exe     | File Injektor Bkebi   |
| libstdimpact\.dll | File Utama Bkebi     |
| tp_files          | Folder Teleportasi       |
| themes            | Folder Tema         |
| cfg\.ini          | File Konfigurasi Injektor         |
| cfg\.json         | Konfigurasi Bkebi     |
| imgui\.ini        | Konfigurasi Ukuran GUI Bkebi |

Di sarankan untuk mencadangakan file `cfg.json` File ini tidak hanya berisikan konfigurasi Bkebi, tetapi juga penanda yang sudah selesai. Anda dapat membuat file `BAT` yang ada di bawah ini untuk membuat salinan `cfg.json` anda. Beri nama "start.bat" dan jalankan program di dalam folder Bkebi

```cmd
@echo off
set rootPath=%cd%
echo %date%%time%

copy /Y cfg.json.backup cfg.json.backup2
copy /Y cfg.json cfg.json.backup
start injector.exe
```
