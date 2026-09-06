# project2-python-handtrack-by-fidz
Welcome the handtrack project
# Retrolens - Filter & Portal Pelacak Tangan
Aplikasi filter kamera interaktif menggunakan gerakan tangan (hand tracking) dengan MediaPipe dan OpenCV. Anda dapat membuat "portal" dengan jari Anda yang akan menerapkan berbagai filter menarik (Mono, Dual-Tone, Pixelate, Invert, Sepia, Blur, Thermal, Sketch, Glitch, Neon, Galaxy).

# Persyaratan Sistem
-Python 3.7 atau lebih baru
-Webcam

# 1. Cara Install dan Menjalankan
## 1. Kloning Repositori
Pertama, clone repositori ini ke komputer Anda dan masuk ke foldernya (ganti URL dengan link repositori GitHub Anda):
'''git clone <URL_GITHUB_ANDA>
cd <NAMA_FOLDER_REPO>'''

## 2. Buat Lingkungan Virtual (Opsional tapi Sangat Disarankan)
Gunakan lingkungan virtual agar dependensi (perpustakaan) tidak bertabrakan dengan proyek Python lainnya di komputer Anda.
'''# Untuk Windows
python -m venv venv
venv\Scripts\activate

# Untuk macOS / Linux
python3 -m venv venv
source venv/bin/activate'''

## 3. Instal Dependensi
Instal semua perpustakaan Python yang dibutuhkan dengan menjalankan perintah berikut:
'''pip install -r requirements.txt'''
Atau jika Anda ingin menginstalnya secara manual satu per satu:
'''pip install opencv-python mediapipe numpy'''

## 4. Pastikan Model MediaPipe Tersedia
Aplikasi ini membutuhkan dua file model dari MediaPipe yang seharusnya sudah ada di dalam repositori ini:

hand_landmarker.task(Untuk mendeteksi titik di tangan)
selfie_segmenter.tflite(Untuk memfilter Galaxy / memisahkan latar belakang)
Jika file tersebut belum ada, pastikan untuk menempatkannya di dalam folder yang sama dengan file ''main.py.''
