copy paste kode di bawah ini... ganti nama file yang di folder Dataset_Kecil
misalnya 
-https://github.com/RianHadi096/MachineLearning/blob/main/Dataset_Kecil/Global_Music_Streaming_Listener_Preferences.csv?raw=true
jadi
-https://github.com/RianHadi096/MachineLearning/blob/main/Dataset_Kecil/file_yang_ada_di_folder_dataset_kecil.csv?raw=true

jangan dirubah kode yang paling akhir yang seperti ini '?raw=true'

import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

try:
    url = "https://github.com/RianHadi096/MachineLearning/blob/main/Dataset_Kecil/Global_Music_Streaming_Listener_Preferences.csv?raw=true"
    df = pd.read_csv(url)
    print(df)
except Exception as e:
    print(f"Error loading data: {e}")
