# project-analisis-data-python
# Instal berbagai library yang digunakan dengan beberapa perintah berikut.

conda activate main-ds
pip install streamlit babel

# Menyiapkan DataFrame

import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
import streamlit as st
from babel.numbers import format_currency
sns.set(style='dark')

# Membuat Komponen Filter
# Melengkapi Dashboard dengan Berbagai Visualisasi Data

streamlit run dashboard_bike_sharing.py
