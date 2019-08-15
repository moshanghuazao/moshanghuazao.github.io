---
layout: post
title:  "whilework"
date:   2019-08-15 19:15:24 +0800
categories: jekyll update
---

备注：循环嵌套练习题根据学生情况选择

###循环嵌套练习题：

1、求 100-200以内同时能被2、3、5整除的第一个数


i = 100

while i<200:

    if i%2==0 and i%3==0 and i%5==0:
        print(i)
        break
    i += 1

2、打印200以内能被7整除又不包含7的数


i = 0    
                                
while i<200:
                             
    if i%7==0 and i/10%10!=7 and i%10!=7:
        print(i)                         
    i += 1                               

3、9 * 9乘法表输出

i = 1

while i <= 9:

    j = 1
    while j <= i:
        print('{} x {} = {:2d}'.format(i,j,i*j),end=' |')
        j += 1
    i += 1
    print('')


4、求s=a+aa+aaa+aaaa+aa...a的值，其中a是一个数字。 例如2+22+222+2222+22222(此时共有5个数相加)，几个数相加有键盘控制。


n = int(input('几个数相加？'))

a = 6

i = 1

s = 0

while i <= n:

    j=0
    while j<i:
        s = s + a*(10**j)
        j += 1
    i += 1
    
print(s)


5、一球从100米高度自由落下，每次落地后反跳回原高度的一半；再落下，求它在 第10次落地时，共经过多少米？第10次反弹多高？


h = 100

i = 0

s = 0

while i < 10:

    s += h+h/2
    h = h/2
    i += 1
    
print(s,h)


5、打印以下图形：

      *********
      *       *
      *       *
      *********


n = 9

i = 1

print(' '* n+'*' * n)

while i<(n//2-1):

    print(' '*n+'*'+' '*(n-2)+'*')
    i += 1
    
print(' '* n+'*' * n)      

6、打印如下图形:

	 *******
	  *****
	   ***
	    *
	   ***
	  *****
	 *******


n = 7
                                   
mid = n // 2 + 1  
                      
i = 1   
                                
while i <= n:   
                        
    star_num = abs(mid-i)*2+1           
    space_num = (n-star_num)//2         
    print(' '*space_num + "*"*star_num) 
    i += 1                              

:

	     A
	    ABA
	   ABCBA
	  ABCDCBA
	 ABCDEDCBA
	ABCDEFEDCBA

n = 6

i = 1

word = ord('A')

while i <= n:

    print(' '*(n-i),end='')
    j = 0
    while j<i:
        print(chr(word+j),end='')
        j += 1
    k = 0
    while k<i-1:
        print(chr(word+j-k),end='')
        k += 1
    print('')
    i += 1

:

	******
	*****
	****
	***
	**
	*

n = 6

while n>0:

    i=0
    while i<n:
        print('*',end='')
        i += 1
    print('')
    n -= 1












