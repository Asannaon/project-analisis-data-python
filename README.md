# project-analisis-data-python

Tutorial streamlit

Impor Perpustakaan:

ular piton

Salin kode
import streamlit as st

import ssl 
import pandas as pd
import plotly.express as px
import plotly.graph_objects as go
Skrip

Memuat Data:

Salin kode
@st.cache_resource
def load_data():
    data = pd.read_csv(
  
"Bike-sharing-dataset/hour.csv")
    return data

data = load_data()
Fungsi load_datadigunakan untuk memst.cache_resourceuntuk meningkatkan kinerja.

Judul Dasbor dan Bilah Sisi:

Skrip menetapkan judul dashboard
Membuat dan menampilkan informasi di sidebar seperti nam
Memberikan opsi untuk menang
Visualisasi:

Membuat dua kolomst.columns.
Visualisasi
Visualisasi
Visu
Tentang Bagian:

Laki-laki
Jalankan Dasbor:

Untuk menjalankan dstreamlit runpada terminal, terpisah
Arduino

Salin kode
streamlit run dashboard_bike_sharing.py
