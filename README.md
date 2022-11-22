# rtx1200_exporter
RTX1200 prometheus exporter

upload by sftp
```bash
sftp -o "batchmode no" -b upload.bat ${host}
```

upload.bat
```bash
put rtx1200_exporter.lua /rtx1200_exporter.lua
quit
```

make exporter enable on rtx1200
```
schedule at 1 startup * lua /rtx1200_exporter.lua
```
