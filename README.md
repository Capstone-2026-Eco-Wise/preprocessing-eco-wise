# Eco-Wise Dataset Preprocessing Pipeline

Repositori ini berisi berkas dan skrip pendukung untuk melakukan *data preprocessing* dan eksplorasi statistik pada dataset limbah **Eco-Wise**. Tahap Preprocessing digunakan untuk memastikan citra sampah memiliki dimensi yang seragam, bersih dari anomali, dan siap diolah oleh model MobileNetV2.

## 📊 Dataset Overview
Dataset yang digunakan mencakup **17.620 gambar** yang dikelompokkan ke dalam 4 kategori utama:
* **Anorganik**: Kaleng, plastik (PET, HDPEM), kertas, kardus, kaca, kain, bungkus makanan.
* **B3 (Bahan Berbahaya & Beracun)**: Baterai, botol obat/kimia, wadah kosmetik, kaleng aerosol.
* **Organik**: Sisa makanan, kulit telur, daun, tisu.
* **Non-Waste**: Objek acak yang tidak mendefinisikan Objek Sampah.

## 📦 File di dalam Repositori
1. `Preprocessing_Eco_Wise_Final.ipynb`: Notebook utama proses pembersihan data, resizing gambar ke $224 \times 224$, penanganan *DecompressionBombWarning*, augmentasi data, dan analisis kecerahan.
2. `dataset_manifest.csv`: Berkas manifes yang memetakan jalur file, label kelas, resolusi asli, *aspect ratio*, hingga partisi data (*train, test, validation*).
3. `eco_wise_data_dictionary.csv`: Kamus data terstruktur yang berisi ringkasan statistik dan distribusi sampel per material kelas.

## 📥 Dataset Download
Karena ukuran dataset berupa citra gambar terlalu besar untuk diunggah langsung ke GitHub, Anda dapat mengunduh berkas kompresi dataset mentah asli melalui tautan Google Drive berikut:
🔗 [Unduh Eco-Wise Dataset ZIP (Google Drive)](https://drive.google.com/file/d/1aq95F8fq4XIeQeZGrIqm-_Va2L8PTJM-/view?usp=drive_link)

> **Petunjuk:** Setelah mengunduh berkas `ecowise_dataset.zip`, ekstrak ke direktori kerja Anda atau sesuaikan jalur *path* yang ada di dalam Notebook.

## 🚀 Cara Penggunaan

1. **Kloning Repositori ini:**
   ```bash
   git clone [https://github.com/USERNAME_ANDA/Preprocessing.git](https://github.com/USERNAME_ANDA/Preprocessing.git)
   cd Preprocessing

2. **Install Library:**
   pip install -r requirements.txt

3. **Run Preprocessing:**
   Buka file Preprocessing_Eco_Wise_Final.ipynb menggunakan Jupyter Notebook, JupyterLab, atau Google Colab untuk mengeksekusi pipeline        pengolahan citra dari awal hingga akhir.
