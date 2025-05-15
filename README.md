# python_5
code--1
#nested loops
n=int(input("enter the size of n"))
for i in range(n):
    for j in range(n):
        print('^',end=" ")
    print()
 output::
 enter the size of n 3
^ ^ ^ 
^ ^ ^ 
^ ^ ^ 


code::2
#nested loops
n=int(input("enter the size of n"))
for i in range(n):
    for j in range(n):
        print(i,end=" ")
    print()

  output::
enter the size of n 4
0 0 0 0 
1 1 1 1 
2 2 2 2 
3 3 3 3 

code---2
#nested loops
n=int(input("enter the size of n"))
for i in range(n):
    for j in range(n):
        print(j,end=" ")
    print()

  output::
  enter the size of n 4
0 1 2 3 
0 1 2 3 
0 1 2 3 
0 1 2 3 


code--3
#right angled triangle symmetric
n=int(input("enter the size of n"))
for i in range(n):
    for j in range(i):
        print('*',end=" ")
    print()
output::
enter the size of n 5

* 
* * 
* * * 
* * * * 

code--5
#right angled triangle using the single for loop
for i in range(5):
    print("*" *i)

output::
*
**
***
****


code--6

#right angled triangle using the single for loop
for i in range(5):
    print("* " *5)


 output::
    
* * * * * 
* * * * * 
* * * * * 
* * * * * 
* * * * * 



code--7

#hollow square
n=int(input("enter the size of n:"))
for i in range(n):
    for j in range(n):
        if i==0 or i==n-1  or j==0 or j==n-1:
            print('*',end=' ')
        else:
            print(' ',end=' ')
    print()


  output:;

enter the size of n: 5
* * * * * 
*       * 
*       * 
*       *
* * * * * 


coodee--9:
#hollow square
n=int(input("enter the size of n:"))
for i in range(n):
    for j in range(n):
        if i==0 or i==n-1  or j==0 or j==n-1 or i==j or i+j==n-1:
            print('*',end=' ')
        else:
            print(' ',end=' ')
    print()

output::
enter the size of n: 7
* * * * * * * 
* *       * * 
*   *   *   * 
*     *     * 
*   *   *   * 
* *       * * 
* * * * * * * 

code--10
#hollow square
n=int(input("enter the size of n:"))
for i in range(n):
    for j in range(n):
        if i==j or i+j==n-1:
            print('*',end=' ')
        else:
            print(' ',end=' ')
    print()

output::
enter the size of n: 7
*           * 
  *       *   
    *   *     
      *       
    *   *     
  *       *   
*           * 

code--11
#hollow square
n=int(input("enter the size of n:"))
for i in range(n):
    for j in range(n):
        if i==0 or i==n-1 or i==j or i+j==n-1:
            print('*',end=' ')
        else:
            print(' ',end=' ')
    print()

output::
enter the size of n: 7
* * * * * * * 
  *       *   
    *   *     
      *       
    *   *     
  *       *   
* * * * * * * 


code-12
#text right angled triangle
text='lali'
r=len(text)
for i in range(r):
    for j in range(i+1):
        print(text[j],end=' ')
    print()

output::
l 
l a 
l a l 
l a l i 


code--13:
#mirror image of right angle triangle
j=int(input("enter the size of n:"))
for i in range(5):
    for j in range(j):
        print('*',end=" ")
    print()
output::
enter the size of n: 5
* * * * * 
* * * * 
* * * 
* * 
* 
  or
  n=int(input())
for i in range(n):
    for j in range(n-i):
        print("*",end=' ')
    print()
output::
 5
* * * * * 
* * * * 
* * * 
* *
*


side angle pyramid::
code--14::
 n=int(input("Enter a number:"))
for i in range(1,2*n):
    s=i if i<=n else 2*n-i
    for j in range(s):
        print("*",end=' ')
    print()

output::
Enter a number: 6
* 
* * 
* * * 
* * * * 
* * * * * 
* * * * * * 
* * * * * 
* * * * 
* * * 
* * 
*


or
#half rhombus

n=int(input("enter a number:"))
for i in range(1,n+1):
    for j in range (i):
        print("*",end=' ')
    print()
for i in range(1,n+1):
    for j in range (n-i):
        print("*",end=' ')
    print()

outpur::
enter a number: 5
* 
* * 
* * * 
* * * * 
* * * * * 
* * * * 
* * * 
* * 
* 

code-14::

n=int(input())
for i in range(1,n+1):
    for j in range(n-i):
        print(" ",end=' ')
    for k in range(i):
         print('*',end=' ')
    print()
output::
5
        * 
      * * 
    * * * 
  * * * * 
* * * * * 

codee-14
#pyramid shape
n=int(input())
for i in range(1,n+1):
    for j in range(n-i):
        print(" ",end=' ')
    for k in range(2*i-1):
         print('*',end=' ')
    print()
output:;
5
        * 
      * * * 
    * * * * * 
  * * * * * * * 
* * * * * * * * * 


code::15

#pascal triangle
'''  1
  1  1
 1  2  1
1  3  3  1
'''

n=int(input("enter a number:"))
for i in range(n):
    for s in range(n-i-1):
        print(' ',end=' ')
    num=1
    for j in range(i+1):
         print(f"{num}  ",end=' ')
         num= num*(i-j)//(j+1)
    print()


  output::
  
enter a number: 6
          1   
        1   1   
      1   2   1   
    1   3   3   1   
  1   4   6   4   1   
1   5   10   10   5   1   


code-15:
#floyd's triangle
'''
1
2 3
4 5 6
7 8 9 10
'''

r=int(input("enter a row value:"))
n=1
for i in range(1,r+1):
    for j in range(i):
        print(n, end=' ')
        n+=1
    print()
output::
enter a row value 4
1 
2 3 
4 5 6 
7 8 9 10 
