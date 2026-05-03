from weasyprint import HTML

# Content for the README in Markdown-style within HTML
html_content = """
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <style>
        @page {
            size: A4;
            margin: 20mm;
            background-color: #fdfdfd;
        }
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #24292e;
            margin: 0;
            padding: 0;
        }
        .container {
            padding: 20px;
        }
        .header {
            border-bottom: 2px solid #e1e4e8;
            padding-bottom: 15px;
            margin-bottom: 25px;
            text-align: center;
        }
        h1 {
            color: #24292e;
            font-size: 26pt;
            margin: 0;
        }
        .subtitle {
            color: #586069;
            font-size: 12pt;
            margin-top: 5px;
        }
        h2 {
            color: #0366d6;
            font-size: 18pt;
            border-bottom: 1px solid #eaecef;
            padding-bottom: 5px;
            margin-top: 30px;
        }
        h3 {
            font-size: 14pt;
            color: #2f363d;
            margin-top: 20px;
        }
        p, li {
            font-size: 11pt;
        }
        .code-block {
            background-color: #f6f8fa;
            padding: 12px;
            border-radius: 6px;
            font-family: 'Courier New', Courier, monospace;
            font-size: 10pt;
            border: 1px solid #d1d5da;
            margin: 10px 0;
        }
        .file-card {
            background-color: #ffffff;
            border: 1px solid #e1e4e8;
            padding: 15px;
            border-radius: 8px;
            margin-bottom: 15px;
        }
        .badge-container {
            margin: 15px 0;
            text-align: center;
        }
        .badge {
            display: inline-block;
            background-color: #0366d6;
            color: white;
            padding: 4px 12px;
            border-radius: 15px;
            font-size: 9pt;
            font-weight: bold;
            margin: 0 4px;
        }
        .footer {
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid #eaecef;
            font-size: 10pt;
            color: #6a737d;
            text-align: center;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>📚 Repository Tugas Kuliah</h1>
            <div class="subtitle">Koleksi Implementasi Pemrograman & Analisis Data</div>
        </div>

        <div class="badge-container">
            <span class="badge">Python</span>
            <span class="badge">Jupyter Notebook</span>
            <span class="badge">Data Science</span>
            <span class="badge">Big Data</span>
        </div>

        <h2>📖 Deskripsi Project</h2>
        <p>Repository ini merupakan dokumentasi terstruktur untuk berbagai tugas akademik. Fokus utama mencakup pengolahan data menggunakan Python, teknik <i>scraping</i>, penggunaan API, hingga penyelesaian persoalan matematika komputasi.</p>

        <h2>📂 Struktur & Highlight File</h2>
        
        <div class="file-card">
            <h3>🚀 Analisis Big Data & Web Scraping</h3>
            <p>Berisi implementasi tingkat lanjut dalam pengambilan dan pengolahan data.</p>
            <ul>
                <li><code>UTS BIG DATA.ipynb</code>: Dokumentasi proses EDA, integrasi API, dan teknik Web Scraping.</li>
                <li><code>Tugas5_BigData_nopal.ipynb</code>: Studi kasus pengolahan dataset besar.</li>
            </ul>
        </div>

        <div class="file-card">
            <h3>📊 Statistika & Prediksi</h3>
            <p>Fokus pada pemodelan matematis dan analisis tren data.</p>
            <ul>
                <li><code>PrediksiKorelasiRegresi.ipynb</code>: Analisis hubungan antar variabel dan prediksi hasil.</li>
                <li><code>Tugas_Analisis_Dataset_Wine_Quality</code>: Implementasi machine learning untuk klasifikasi kualitas.</li>
                <li><code>Statistika Median, Mean...</code>: Dasar-dasar perhitungan statistik deskriptif.</li>
            </ul>
        </div>

        <div class="file-card">
            <h3>🧮 Matematika & Aljabar</h3>
            <p>Penyelesaian teori matematika menggunakan kode program.</p>
            <ul>
                <li><code>tugas_aljabar.ipynb</code>: Implementasi matriks dan operasi aljabar lainnya.</li>
            </ul>
        </div>

        <h2>🛠️ Cara Penggunaan</h2>
        <p>Untuk menjalankan notebook ini secara lokal, ikuti langkah berikut:</p>
        <div class="code-block">
            git clone https://github.com/yakaHan/Tugas-Kuliah.git<br>
            cd Tugas-Kuliah
        </div>
        <p>Gunakan lingkungan virtual dan instal dependensi standar:</p>
        <div class="code-block">
            pip install pandas numpy matplotlib scikit-learn beautifulsoup4
        </div>

        <div class="footer">
            <p>Dikelola dengan ❤️ oleh <strong>yakaHan</strong></p>
            <p>Link Repository: github.com/yakaHan/Tugas-Kuliah</p>
        </div>
    </div>
</body>
</html>
"""

# Output PDF path
output_pdf_path = "README_Tugas_Kuliah_v1.pdf"

# Generate PDF
HTML(string=html_content).write_pdf(output_pdf_path)

# Generate Markdown version for user to copy-paste
md_content = """# 📚 Repository Tugas Kuliah

Koleksi implementasi pemrograman, analisis data, dan proyek akademik yang disusun dalam format Jupyter Notebook.

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📝 Deskripsi
Repository ini berisi berbagai tugas perkuliahan yang mencakup bidang:
- **Analisis Data & Statistika**
- **Big Data & Machine Learning** (EDA, Web Scraping, API Integration)
- **Matematika Komputasi** (Aljabar Linear)

## 📂 Highlight File Utama

### 📊 Big Data & Scraping
- **UTS BIG DATA**: Implementasi komprehensif Exploratory Data Analysis (EDA), koneksi API, dan teknik pengambilan data via Scraping.
- **Tugas5 Big Data**: Latihan pengolahan dataset skala besar.

### 📈 Statistika & Prediksi
- **Prediksi Korelasi & Regresi**: Model matematis untuk melihat hubungan antar variabel dan prediksi masa depan.
- **Dataset Wine Quality**: Analisis klasifikasi kualitas berdasarkan fitur-fitur kimia.
- **Statistika Dasar**: Perhitungan Mean, Median, Modus, dan Mean Deviation.

### 🔢 Matematika
- **Tugas Aljabar**: Penyelesaian persoalan aljabar menggunakan pendekatan komputasi Python.

## 🚀 Cara Menjalankan
1. **Clone Repository**:
   ```bash
   git clone [https://github.com/yakaHan/Tugas-Kuliah.git](https://github.com/yakaHan/Tugas-Kuliah.git)
