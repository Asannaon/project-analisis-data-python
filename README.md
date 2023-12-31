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

import streamlit as st

#Create a filter for selecting a specific city
city = st.selectbox('Select City', df['City'].unique())


# Melengkapi Dashboard dengan Berbagai Visualisasi Data

import matplotlib.pyplot as plt
import seaborn as sns

#Filter data based on user selection
filtered_data = df[df['City'] == city]

#Create visualizations (e.g., bar chart, line chart, etc.)
st.bar_chart(filtered_data['Column_Name'])

# Add other visualizations as needed


streamlit run dashboard_bike_sharing.py
