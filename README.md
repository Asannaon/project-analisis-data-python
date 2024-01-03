# project-analisis-data-python
# setup environment nootbook
import pandas as pd: Ini mengimpor library pandas dan memberinya alias pd. pandas adalah library Python yang digunakan untuk manipulasi dan analisis data. Dengan menggunakan alias pd, kita dapat menggunakan fungsi-fungsi dari pandas dengan cara yang lebih ringkas.

import pandas as pd

# Membuat DataFrame
df = pd.DataFrame({'A': [1, 2, 3], 'B': [4, 5, 6]})

# Menampilkan DataFrame
print(df)

import plotly.express as px: Ini mengimpor modul express dari library plotly dan memberikannya alias px. plotly adalah library yang digunakan untuk membuat visualisasi data interaktif. plotly.express adalah antarmuka tingkat tinggi yang mempermudah pembuatan grafik

import plotly.express as px

# Membuat scatter plot dengan plotly express
df = px.data.iris()
fig = px.scatter(df, x='sepal_width', y='sepal_length', color='species')
fig.show()

import warnings: Ini mengimpor modul warnings, yang digunakan untuk mengelola peringatan (warnings) yang dihasilkan oleh interpreter Python. Dengan mengimpor warnings, Anda dapat mengontrol tampilan atau penanganan peringatan selama eksekusi program.

import warnings

# Menonaktifkan peringatan
warnings.filterwarnings('ignore')

Dengan mengimpor library-library tersebut, Anda dapat memanfaatkan fungsionalitas dan fitur-fitur yang disediakan oleh pandas untuk manipulasi data, serta menggunakan plotly untuk membuat visualisasi data yang interaktif. Peringatan (warnings) dapat membantu Anda mengelola tampilan pesan peringatan selama eksekusi program.

# setup environment Streamlit
# Instal berbagai library yang digunakan dengan beberapa perintah berikut.

conda create --name main-ds python=3.12.1
conda activate main-ds
pip install numpy pandas scipy matplotlib seaborn jupyter streamlit babel

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
