# codes for excel
import pandas as pd

pd.__version__

pd.read_excel('exl.xlsx')

pd.read_excel('exl.xlsx',index_col=0)

h3 = pd.read_excel('exl.xlsx')
h3 = h3.head(3)
print(h3)

pd.read_excel('exl.xlsx',index_col=0,header=0)

pd.read_excel('exl.xlsx',index_col=0,usecols='A:C')

pd.read_excel('exl.xlsx',index_col=0,usecols='A:C',names=["name","place","desh"])

pd.read_excel('exl.xlsx',index_col=0,header=0,usecols=[0,1,2],sheet_name=1)

pd.read_excel('exl.xlsx',index_col=0,usecols=[0,2,3])

pd.read_excel('exl.xlsx',index_col=0,header=0,usecols=[0,1,2],sheet_name='teacher')

pd.read_excel('exl.xlsx',index_col=0,header=0,usecols=[0,1,2],sheet_name=1,skiprows=[0,1])

teacher = pd.read_excel('exl.xlsx',index_col=0,header=0,usecols=[0,1,2],sheet_name=1)
print(teacher)

teacher.info()

teacher.head()
 head() function displays first few rows and tail() displays last few rows

 teacher.to_csv("newCSV.csv")
