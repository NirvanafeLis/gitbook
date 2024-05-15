# python 实验题

输出1-1000里的素数

```
# -*- coding: UTF-8 -*-
 
num=[];
i=2
for i in range(2,1000):
   j=2
   for j in range(2,i):
      if(i%j==0):
         break
   else:
      num.append(i)
print(num)
```
