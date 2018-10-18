# Project4
Project Oct17,2018

str1=str(input("Please enter a sentence:"))
m=str1.split()
list1=[]
l=len(m)
for i in range(l):
    l1=len(m[i])
    if m[i][0]=="a" or m[i][0]=="e" or m[i][0]=="i" or m[i][0]=="o" or m[i][0]=="u" or m[i][0]=="y":
        n=m[i]+'yay'
        list1.append(n)
    else:
        for a in range(1,l1):
            if m[i][a]=="a" or m[i][a]=="e" or m[i][a]=="i" or m[i][a]=="o" or m[i][a]=="u" or m[i][a]=="y":
                n=m[i]+'yay'  
                list1.append(n)
            else:
                n=m[a+1:l1+1]+m[0:a+1]
                list1.append(n)
s=''.join(list1)
print(s)
                
    
    
