![image](https://github.com/user-attachments/assets/6ce3a9be-5ddc-4ebb-a970-0bf387df4cde)# skill_assesment 1

```
import pandas as pd
data={
    'Name' : ['John', 'Sarah', 'Mike', 'Emily', 'David'],
    'Age': [25, 31, 29, 35, 27],
    'Gender': ['M', 'F', 'M', 'F', 'M'],
    'Salary': [50000, 70000, 60000, 80000, 55000]
}
df=pd.DataFrame(data)
print(df.head(3))
```
![image](https://github.com/user-attachments/assets/00fa15b1-23b1-4fc3-afeb-76ef9349c295)
```
data={
    'name' : ['John', 'Sarah', 'Mike', 'Emily', 'David'],
    'age': [25, 31, 29, 35, 27],
    'Gender': ['M', 'F', 'M', 'F', 'M'],
    'Salary': [50000, 70000, 60000, 80000, 55000]
}
df=pd.DataFrame(data)
print(df.tail())
```
![image](https://github.com/user-attachments/assets/cc9baca8-c289-4629-bbdd-2593e6f24f09)

```
data={
    'Name' : ['John', 'Sarah', 'Mike', 'Emily', 'David'],
    'Age': [25, 31, 29, 35, 27],
    'Gender': ['M', 'F', 'M', 'F', 'M'],
    'Salary': [50000, 70000, 60000, 80000, 55000]
}
df=pd.DataFrame(data)
print(df.info)
```
![image](https://github.com/user-attachments/assets/3118ae9e-90af-4c77-bf53-3d6182055de8)

```
data={
    'Name' : ['John', 'Sarah', 'Mike', 'Emily', 'David'],
    'Age': [25, 31, 29, 35, 27],
    'Gender': ['M', 'F', 'M', 'F', 'M'],
    'Salary': [50000, 70000, 60000, 80000, 55000]
}
df=pd.DataFrame(data)
print(df.describe())
```
![image](https://github.com/user-attachments/assets/35716d16-2a28-4bd7-8fae-ca6091a40fc3)
```
data={
    'Name' : ['Alice','Bob','Charlie','Dave'],
    'Age': [25,30,35,40],
    'score' : [90,80,85,95]
}
df=pd.DataFrame(data)
df_sorted=df.sort_values(by='Age',ascending =False)
print(df_sorted)
```
![image](https://github.com/user-attachments/assets/62356c54-42ad-4e70-b0a6-6ad3d4b01917)
```
data={
    'Name' : ['Alice','Bob','Charlie','Dave','Emily','Frank'],
    'gender' : ['F','M','M','M','F','M'],
    'age': [25,35,40,28,30,45],
    'salary' : [50000,70000,60000,80000,65000,90000]
}
df=pd.DataFrame(data)
print(df.groupby('gender')['salary'].mean())
```
![image](https://github.com/user-attachments/assets/a3aa7215-30dd-4abd-9d67-abdc202a35f0)
```
data={
    'Name' : ['Alice','Bob','Charlie','Dave','Emily','Frank'],
    'gender' : ['F','M','M','M','F','M'],
    'age': [25,35,40,28,30,45],
    'salary' : [50000,70000,60000,80000,65000,90000]
}
df=pd.DataFrame(data)
print(df.groupby('gender').count())
```
![image](https://github.com/user-attachments/assets/1f57cd60-f7eb-43c7-a072-c5dd329f8977)
```
import pandas as pd
data={
    'name' : ['Alice','Bob','Charlie','Dave','Eve'],
    'age': [25,32,None,41,28],
    'salary' : [50000,None,70000,90000,65000]
}
df=pd.DataFrame(data)
df
```
![image](https://github.com/user-attachments/assets/28fb2be1-3cb2-478d-ad1b-250c1f844ad6)
```
df_cleaned=df.dropna(subset='salary')
print(df_cleaned)
```
![image](https://github.com/user-attachments/assets/be4cebe0-772a-49ac-899d-58e54168ecf1)
```
df_cleaned_all=df.dropna(how='all')
print(df_cleaned_all)
```
![image](https://github.com/user-attachments/assets/cd65a68b-b1e2-406e-a1c2-5b1a4cb20a3e)
```
df_cleaned_any=df.dropna(how='any')
print(df_cleaned)
```
![image](https://github.com/user-attachments/assets/74002e2b-9b60-4f66-8175-8b90d73730b0)
```
import pandas as pd
import numpy as np
data={
    'name': ['Alice ','Bob','Charlie','Dave','Eve','Bob','Charlie'],
    'age' : [25,np.nan,35,41,np.nan,np.nan,85],
    'salary' : [50000,np.nan ,70000,np.nan,60000,np.nan,70000]
}
df=pd.DataFrame(data)
~df.duplicated()
```
![image](https://github.com/user-attachments/assets/cbf7a8b8-ebcb-49bb-84fb-4b7d206562d5)
```
import pandas as pd
import numpy as np
data={
    'name': ['Alice ','Bob','Charlie','Dave','Eve'],
    'age' : [25,np.nan,35,41,np.nan],
    'salary' : [50000,np.nan ,70000,np.nan,60000]
}
df=pd.DataFrame(data)
print(df.fillna(0))
```
![image](https://github.com/user-attachments/assets/72afe1dc-ace7-4605-8dbd-335239eaec9b)
```
import pandas as pd
import numpy as np
data={
    'name': ['Alice ','Bob','Charlie','Dave','Eve'],
    'age' : [25,np.nan,35,41,np.nan],
    'salary' : [50000,np.nan ,70000,np.nan,60000]
}
df=pd.DataFrame(data)
print(df.fillna(method='ffill'))
```
![image](https://github.com/user-attachments/assets/e961ba74-b2b3-458d-a6e6-1b9aacbde36d)
```
import pandas as pd
import numpy as np
data={
    'name': ['Alice ','Bob','Charlie','Dave','Eve'],
    'age' : [25,np.nan,35,41,np.nan],
    'salary' : [50000,np.nan ,70000,np.nan,60000]
}
df=pd.DataFrame(data)
print(df.fillna(method='bfill'))
```

![image](https://github.com/user-attachments/assets/cba8e1cf-5eff-484f-9b70-09c33e61742f)
```
import pandas as pd
import numpy as np
data={
    'name': ['Alice ','Bob','Charlie','Dave','Eve'],
    'age' : [25,np.nan,35,41,np.nan],
    'salary' : [50000,np.nan ,70000,np.nan,60000]
}
df=pd.DataFrame(data)
print(df.fillna(df.mean(numeric_only=True)))
```
![image](https://github.com/user-attachments/assets/e71d5208-2a3e-4f4c-b515-719fe76db269)
```
import pandas as pd
import numpy as np
data={
    'name': ['Alice ','Bob','Charlie','Dave','Eve'],
    'age' : [25,np.nan,35,41,np.nan],
    'salary' : [50000,np.nan ,70000,np.nan,60000]
}
df=pd.DataFrame(data)
~df.duplicated()
```
![image](https://github.com/user-attachments/assets/506497df-763b-41a9-970f-567390bd72fe)
```
import pandas as pd
import numpy as np
data={
    'name': ['Alice ','Bob','Charlie','Dave'],
    'age' : [25,32,18,47],
    'gender' : ['F','M','M','M'],
    'height' : [1.62, 1.78, 1.65, 1.83]
}
df=pd.DataFrame(data)
df_filter=df[(df['gender']=='M') & (df['height']>1.7)]
print(df_filter)
```
![image](https://github.com/user-attachments/assets/ba9a36b7-fce6-42d2-b1d0-377ffea56adc)


