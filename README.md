# Sistem Monitoring & Kontrol IoT (Node-RED REST API, WebSocket & SQLite)

Implementasi praktikum REST API Node-RED beserta seluruh tugas pengembangan:

- **Simulasi ESP32 (`simulasi_esp32.py`)**: Mengirim data suhu dan kelembaban via MQTT (`iot/sensor`) serta menerima perintah kontrol (`iot/kontrol`) dan peringatan threshold (`iot/alert`).
- **Endpoint Threshold (`PUT /api/threshold`)**: Mengatur batas maksimal suhu dan memicu notifikasi real-time jika suhu melewati batas.
- **Grafik Real-Time (Chart.js)**: Visualisasi pergerakan suhu dan kelembaban langsung pada web dashboard.
- **Autentikasi `X-API-Key`**: Validasi header `X-API-Key` pada seluruh endpoint `/api/*`.
- **WebSocket (`/ws/sensor`)**: Komunikasi dua arah real-time dari Node-RED ke dashboard tanpa polling.
- **Penyimpanan SQLite (`iot_data.db`)**: Menyimpan riwayat pembacaan sensor secara permanen ke database SQLite.
