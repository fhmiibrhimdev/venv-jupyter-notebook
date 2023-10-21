# Cara Membuat Lingkungan Virtual Environment untuk Jupyter Notebook di Windows

Panduan ini akan membantu kamu mengatur lingkungan virtual di Jupyter Notebook di Windows. Lingkungan virtual memungkinkan kamu untuk menjaga proyek-proyek Python-mu tetap terpisah, sehingga tidak ada konflik antar dependensi.

## Langkah 1: Instalasi Python
Pastikan kamu memiliki Python terpasang di komputermu. Jika belum, unduh versi terbaru dari python.org dan ikuti panduan instalasinya.

## Langkah 2: Instalasi Jupyter Notebook
Jika belum memiliki Jupyter Notebook, pasang dengan mudah menggunakan perintah berikut di Command Prompt atau PowerShell:
```
pip install jupyter
```

## Langkah 3: Instalasi Virtual Environment (Opsional)
Kalau ingin menggunakan lingkungan virtual (virtual environment), pastikan kamu sudah memasang virtualenv. Kalau belum, instalasi bisa dilakukan dengan perintah:
```
pip install virtualenv
```

## Langkah 4: Buat Lingkungan Virtual
Buka Command Prompt atau PowerShell, dan arahkan ke folder proyekmu. Lalu, buat lingkungan virtual dengan perintah berikut (gantilah myenv dengan nama sesuai keinginanmu):
```
virtualenv myenv
```

## Langkah 5: Aktifkan Lingkungan Virtual
Aktifkan lingkungan virtual yang telah kamu buat dengan perintah berikut di Command Prompt atau PowerShell:
```
myenv\Scripts\activate
```
Jika kamu menggunakan PowerShell, mungkin perlu mengizinkan skrip PowerShell dengan perintah `Set-ExecutionPolicy RemoteSigned`.

## Langkah 6: Instalasi Kernel Jupyter Notebook di Lingkungan Virtual
Pastikan kamu menginstal kernel Jupyter Notebook di lingkungan virtualmu dengan perintah berikut:
```
pip install ipykernel
python -m ipykernel install --user --name=myenv --display-name="My Virtual Environment"
```
Gantilah myenv dengan nama lingkungan virtualmu, dan sesuaikan nama tampilan sesuai keinginan.

## Langkah 7: Buka Jupyter Notebook
Sekarang kamu bisa mulai Jupyter Notebook dengan perintah berikut:
```
jupyter notebook
```
Jupyter Notebook akan terbuka di browsermu. Buat notebook baru dan pilih kernel lingkungan virtual yang tadi telah kamu buat.

## Langkah 8: Menonaktifkan Lingkungan Virtual
Kalau sudah selesai menggunakan Jupyter Notebook, kamu bisa menonaktifkan lingkungan virtual dengan perintah berikut di Command Prompt atau PowerShell:
```
deactivate
```
Sekarang, kamu bisa menggunakan lingkungan virtual di Jupyter Notebook di Windows. Kamu bisa mengikuti langkah ini untuk setiap proyek yang berbeda, menjaga proyekmu tetap terpisah dan menghindari masalah dengan dependensi.
