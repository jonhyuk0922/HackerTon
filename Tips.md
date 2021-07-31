1.zip파일 풀어서 tmp 디렉토리에 저장해주기

```python
import zipfile

local_zip = 'PATH'
zip_ref = zipfile.ZipFile(local_zip,'r')
zip_ref.extractall('/tmp')
zip_ref.close()
```

2.판다스 숫자 출력 포맷 변경

```python
pd.options.display.float_format = '{:.1f}'.format

#원래대로 복원
pd.reset_option('display.float_format')
```

3.train data 상관관계 시각화

```python
import seaborn as sns
sns.heatmap(train.corr(),annot=True)
```

4. NAN 결측치 처리하는 방법

```python
import pandas as pd
#dataFrame = df
df.fillna(value='NAN')
#만약 A열의 NAN을 A의 평균으로 채움, inplace는 df에 바로 값 채움
df['A'].fillna(value=df['A'].mean(), inplace = True)
```

5. Colab에서 파일 저장하는 법

```python
from google.colab import files
files.download('파일 경로')
#팝업 해제해줘야함
```

6. 학습한 모델 불러오는 법

```python
import tensorflow as tf

tf.keras.models.save_model('path')
model = tf.keras.models.load_model('path')
```
