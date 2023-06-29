# LGES2023_Sampling_and_XAI

### 실습 준비

0. 필요 패키지
```py
import zipfile
from google.colab import drive # Local PC로 실습하는 경우 실행 x
```
1. 구글 드라이브 연동(Local PC로 실습하는 경우 실행 x)
```py
drive.mount('/content/drive')
%cd /content/drive/MyDrive
```

2. git에서 가져오기
```py
!git clone https://github.com/Saerin-Lim/LGES2023_Sampling_and_XAI.git
```
3. time-series data 압축풀기
```py
# change directory # Local PC로 실습하는 경우 실행 x
%cd LGES2023_Sampling_and_XAI/

data_zip = zipfile.ZipFile('./data/time_series_data.zip')
data_zip.extractall('./data')
data_zip.close()
```
