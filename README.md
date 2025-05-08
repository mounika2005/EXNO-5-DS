# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
```
 import pandas as pd
 import numpy as np
 import seaborn as sns
 import matplotlib.pyplot as plt
```
```
x = [1, 2, 3, 4, 5]
y = [3, 6, 2, 7, 1]
plt.plot(x,y,label='line1')
```
![image](https://github.com/user-attachments/assets/ce99a0d4-ed69-433f-a25c-d6da7e39b6ce)
```
 x1 = [1,2,3]
 y1 = [2,4,1]
 x2 = [1,2,3]
 y2 = [4,1,3]
 plt.plot(x1,y1,label='line1')
 plt.plot(x2,y2,label='line2')
 plt.xlabel('x-axis')
 plt.ylabel('y-axis')
 plt.title('Two lines on same graph!')
 plt.legend()
 plt.show()
```
![image](https://github.com/user-attachments/assets/a7c0f485-41c3-4628-9f29-b985193ac5e4)
```
 import matplotlib.pyplot as plt
 x=[1,2,3,4,5,6]
 y=[2,4,1,5,2,6]
 plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
 plt.xlabel('x-axis')
 plt.ylabel('y-axis')
 plt.title('Some cool customizations!')
 plt.show()
```
![image](https://github.com/user-attachments/assets/7f6cab65-2af2-4a68-a67c-941134fe5753)
```
 yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
 plt.plot(yield_apples)
```
![image](https://github.com/user-attachments/assets/31ec1bc7-0b60-4a3d-b6d3-a59ea40c9f54)
```
 years=[2010,2011,2012,2013,2014,2015]
 yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
 plt.plot(years,yield_apples)
```
![image](https://github.com/user-attachments/assets/1b96270b-9af2-47cf-81e8-3ae27ea45c95)
```
 years=range(2000,2012)
 apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
 oranges=[0.926,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896, ]
 plt.plot(years, apples)
 plt.plot(years, oranges)
 plt.xlabel('Year')
 plt.ylabel('Yield (tons per hectare)')
 plt.title('Crop Yields in Kanto')
 plt.legend(['Apples','Oranges']);
```
![image](https://github.com/user-attachments/assets/64d5bbeb-88d3-422a-8faa-dbd246dd3a2e)
```
 plt.figure(figsize=(12,6))
 plt.plot(years,oranges,marker='o')
 plt.title("Yield of Oranges (tons per hectare)");
```
![image](https://github.com/user-attachments/assets/07465547-6b08-413b-a743-969b48b78a50)
```
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 x=np.arange(0,10)
 y=np.arange(11,21)
 x
```
![image](https://github.com/user-attachments/assets/f46870ec-9ad4-4810-b8eb-3aa6c9c523a7)
```
 plt.scatter(x,y,c='r')
 plt.xlabel('X-axis')
 plt.ylabel('Y-axis')
 plt.title('Graph in 2D')
 plt.savefig('Test.png')
```
![image](https://github.com/user-attachments/assets/6b3f9a99-41f7-49f3-93db-ba2121da2232)
```
 y=x*x
 y
```
 plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
 plt.xlabel('X axis')
 plt.ylabel('Y axis')
 plt.title('2d Diagram')
 plt.legend(['y-values']);
 ```
![image](https://github.com/user-attachments/assets/103dbb07-5fda-4ca0-8e86-8ccbf62e3dbe)
```
 x=np.arange(0,4*np.pi,0.1)
 y=np.sin(x)
 plt.title("sine wave form")
 plt.plot(x,y)
 plt.show()
 ```
![image](https://github.com/user-attachments/assets/4efe656f-6d20-4a5c-a4cc-8110da0e7c7b)
```
 import matplotlib.pyplot as plt
 import numpy as np
 x=[1,2,3,4,5]
 y1=[10,12,14,16,18]
 y2=[5,7,9,11,13]
 y3=[2,4,6,8,10]
 plt.fill_between(x,y1,color='blue')
 plt.fill_between(x,y2,color='green')
 ```
![image](https://github.com/user-attachments/assets/8c58af0d-2301-42f6-b49b-231cd63b97ea)
```
 import matplotlib.pyplot as plt
 import numpy as np
 x=[1,2,3,4,5]
 y1=[10,12,14,16,18]
 y2=[5,7,9,11,13]
 y3=[2,4,6,8,10]
 plt.fill_between(x,y1,color='blue')
 plt.fill_between(x,y2,color='green')
 plt.plot(x,y1,color='red')
 plt.plot(x,y2,color='black')
 plt.legend(['y1','y2'])
 plt.show()
 ```
![image](https://github.com/user-attachments/assets/a4f56123-d82c-413e-98d9-89350361ae87)
``` import matplotlib.pyplot as plt
 height=[10,24,36,40,5]
 names=['one','two','three','four','five']
 c1=['red','green']
 c2=['b','g']
 plt.bar(names,height,width=0.8,color=c1)
 plt.xlabel('x-axis')
 plt.ylabel('y-axis')
 plt.title('My bar chart!')
 plt.show()
```
![image](https://github.com/user-attachments/assets/e16acc71-f112-4c70-9810-987bb79d9bdf)
  ```
 x=[2,8,10]
 y=[11,16,9]
 x2=[3,9,11]
 y2=[6,15,7]
 plt.bar(x,y,color='r')
 plt.bar(x2,y2,color='g')
 plt.title('Bar graph')
 plt.ylabel('Y axis')
 plt.xlabel('X axis')
 plt.show()
```
![image](https://github.com/user-attachments/assets/ede06fb3-8e3f-4b16-bc86-1d6964ec4f47)
```
 import matplotlib.pyplot as plt
 ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
 range=(0,100)
 bins=10
 plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
 plt.xlabel('age')
 plt.ylabel('No. of people')
 plt.title('My histogram')
 plt.show()
```
![image](https://github.com/user-attachments/assets/c45b49d5-2b4a-46ec-836a-cd5d6d330f6d)
```
 import matplotlib.pyplot as plt
 import numpy as np
 np.random.seed(0)
 data=np.random.normal(loc=0,scale=1,size=100)
 data
 ```
![image](https://github.com/user-attachments/assets/2e5db36b-b3b3-4010-8e0f-d1eaf2e811f8)
```
 fig,ax=plt.subplots()
 ax.boxplot(data)
 ax.set_xlabel('Data')
 ax.set_ylabel('Values')
 ax.set_title('Box Plot')
 ```
![image](https://github.com/user-attachments/assets/fa0a1ccb-5c95-4d79-964a-c5ce0435f2c4)
```
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```
![image](https://github.com/user-attachments/assets/89fd4dc5-922b-45cc-9210-404aebd34dcb)
```
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
```
![image](https://github.com/user-attachments/assets/f3a67770-e94e-4fd6-87ff-4c7c6f51fd7d)







# Result:
        Thus Data Visualization using matplot python library for the given data is executed successfully.
