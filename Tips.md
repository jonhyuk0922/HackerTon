1.zip파일 풀어서 tmp 디렉토리에 저장해주기

```python
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
