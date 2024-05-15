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

判断式

```
#条件判断
# age=15
# if age>=18:
# print("You are Adult,Pls Come in!")
# else:
# print("You are not Adult,Pls Go away")
#改进版，年龄由用户输入
# age=int(input("请输入你的年龄："))
# if age>=18:
# print("You are Adult,Pls Come in!")
# else:
# print("You are not Adult,Pls Go away")
#
# print("我不在条件选择语句内，永远会执行")

#判断人的年纪是否合法
# #0-120
# age=int(input("请输入年龄"))
# if age>=0 and age<=120:
# print("合法年纪")
# else:
# print("非法年纪")
#节日案例 节日 端午节 吃粽子 中秋节 吃月饼 元宵节 吃元宵
# holiday=input("输入节日：")
# if holiday=="端午节":
# print("吃粽子")
# elif holiday=="中秋节":
# print("吃月饼")
# elif holiday=="元宵节":
# print("吃元宵")
# else:
# print("你想吃啥都行")
#判断成绩等级
# score=float(input("请输入成绩："))
# if score>=80 and score<=100:
# print("优秀")
# elif score >=70:
# print("良好")
# elif score >=60:
# print("及格")
# else:
# print("不及格")
#猜数游戏
import random
# data=random.randint(1,100)
# userdata=int(input("请输入一个1-100中的数字："))
# if userdata > data:
# print("你猜大了")
# elif userdata < data:
# print("你猜小了")
# else:
# print("你猜对了")
```

循环体

```
#计算1-100的累加和
#while循环实现
# i=1
# sum=0
# while i<=100:
# sum+=i
# i+=1
# print(sum)
#for循环实现
# sum=0
# for i in range(1,101):
# sum+=i
# print(sum)
#改进，1-100的偶数求和
# sum=0
# for i in range(0,101,2):
# sum+=i
# print(sum)
#break 跳出整个循环体
#continue 跳出本次循环
#使用循环体改进猜数案例
# data=random.randint(1,100)
# for i in range(1,20):
#
# userdata=int(input("请输入一个1-100中的数字："))
# if userdata > data:
# print("你猜大了")
# continue
# elif userdata < data:
# print("你猜小了")
# continue
# else:
# print("你猜对了")
# break
#打印小星星 打印5行小星星，每行小星星数量递增
# line=1
# while line <= 5:
# print("*" * line)
# line+=1
#打印10行*，每行50个星星
for i in range(1,6):
 print("*"*50)
#嵌套打印小星星
#1.完成5行的简单输出 2.每行内部的*进行处理
#
# row=1
# while row<=5:
# col=1
# while col<=row:
# print("*",end="")
# col+=1
# print("")
# row+=1
#打印九九乘法表
row=1
while row<=9:
 col=1
 while col<=row:
 print("%d*%d=%d"%(row,col,row*col),end=" ")
 col+=1
 print("")
 row+=1
```

至于输出方式

```
name = "张三"
age = 24
money = 24.5

"""
python3.6后支持在字符串前面加f,变量用{}包裹起来
推荐，可读性好。
"""
def test02():
    print(f"姓名：{name},年龄：{age},零用钱:{money}")

"""
用逗号分隔开来多个变量
"""
def test03():
    print("姓名：",name,"年龄：",age,"零用钱：",money)


"""
使用format方法
"""
def test04():
    print("姓名：{}，年龄：{}，零用钱：{}".format(name,age,money))
    print("姓名：{0}，年龄：{1}，零用钱：{2}".format(name, age, money)) #{0}代表format后面对应的第一个变量
    print("姓名：{v1}，年龄：{v2}，零用钱：{v3}".format(v1=name, v2=age, v3=money))  # 使用显示名称

""""
使用%格式符，常见的格式符
    %s 字符串
    %d 整数
    %f 浮点数
"""
def test05():
    print("姓名:%s,年龄:%d,零用钱:%.2f" %(name,age,money)) # %.2f表示保留两位小数

test04()

```
