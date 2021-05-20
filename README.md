# List

# count-occurrences-element-list/

def func(a,x):
    counter = 0
    for j in a:
        if j == x:
            counter += 1
    return counter

a=[]

num = int(input("Enter the number of elements in list: "))

for i in range(1,num+1):
    elements=int(input("Enter elements "))
    a.append(elements)

print(a)
x=int(input("Enter the number whose recurrence you want : "))
print("{} has occurence {} times".format(x,func(a,x)))










**#program-to-find-cumulative-sum-of-a-list/

a=[]
num=int(input("Enter the no of elements in the list: "))

for i in range(1,num+1):
    elements=int(input("Enter elements : "))
    a.append(elements)

print(a)
b=[]
j=0

for k in range(0,len(a)):
    j+=a[k]
    b.append(j)

print(b)









**#Program for the largest number in a list

def largest_number(list1):
    max=list1[0]
    for x in list1:
        if x>max:
            max=x
    return max


a=[]

num = int(input("Enter the number of elements in list: "))

for i in range(1,num+1):
    elements=int(input("Enter elements "))
    a.append(elements)

print(largest_number(a))







**#program to print the second highest number 

a=[]

num = int(input("Enter the number of elements in list: "))

for i in range(1,num+1):
    elements=int(input("Enter elements "))
    a.append(elements)

print(a)

if a[0]>=a[1]:
  mx=a[0]
else:
  mx=a[1]


if a[0]>=a[1]:
  secondmax=a[1]
else:
  secondmax=a[0]
  
  
n=len(a)
for i in range(2,n):
    if a[i]>mx:
        secondmax=mx
        mx=a[i]
    elif(a[i]>secondmax and mx != a[i]):
        secondmax=a[i]
print("Second highest number is : "+str(secondmax))











**#Python program to count the number of strings where the string length is 2 or more and the first and last character are same from a input list of strings.

def func(list1):
  z = 0

  for x in list1:
    if len(x) > 1 and x[0] == x[-1]:
      z += 1
  return z


a=[]

num = int(input("Enter the number of elements in list: "))

for i in range(1,num+1):
    elements=input("Enter elements ")
    a.append(elements)

print(func(a))









# Python program to find the list of words that are longer than n from an input list of words



a=[]
num = int(input("Enter the number of elements in list: "))

for i in range(1,num+1):
    elements=input("Enter elements ")
    n=int(input("Enter the no of alpahabets you want to see in the elements: "))
    if len(elements)<=n:
        a.append(elements)


print(a)
















# Python program to check whether a list contains a sublist



def is_Sublist(l, s):
	sub_set = False
	if s == []:
		sub_set = True
	elif s == l:
		sub_set = True
	elif len(s) > len(l):
		sub_set = False

	else:
		for i in range(len(l)):
			if l[i] == s[0]:
				n = 1
				while (n < len(s)) and (l[i+n] == s[n]):
					n += 1
				
				if n == len(s):
					sub_set = True

	return sub_set

a = [2,4,3,5,7]
b = [4,3]
c = [3,7]
print(is_Sublist(a, b))
print(is_Sublist(a, c))

