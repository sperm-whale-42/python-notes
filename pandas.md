## 读取Excel

```python
# 导入相关库
import pandas as pd

# 超参数
data_path = 'D:\0000\0001.xlsx' # 数据地址

# 读取excel数据
## 设置读取的文件路径
io = pd.io.excel.ExcelFile(r''+data_path) # r"+path防转义
## 按工作簿读取数据
sheet1_data = pd.read_excel(io,sheet_name='sheet1')
sheet2_data = pd.read_excel(io,sheet_name='sheet2')
io.close()
## 导入数据类型为dataframe，参考runoob.com/pandas/pandas-dataframe.html
```



