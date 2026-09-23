# HCL

## Write a Python program which accepts a sequence of comma separated 4 digit binary numbers as its input and then check whether they are divisible by 5 or not.The numbers that are divisible by 5 are to be printed in a comma separated sequence. Example: 0100,0011,1010,1001 Then the output should be: 1010
```
ans=input().split(",")
for i in ans:
    binary=i.strip()
    if(int(binary,2)%5==0):
        print(binary)

```
## output:
<img width="1532" height="262" alt="image" src="https://github.com/user-attachments/assets/ef70ebc1-776c-427b-9b0b-b5cc1ccc9f04" />


## Write a Python program that accepts a sentence and calculate the number of letters and digits. Suppose the following input is supplied to the program: hello world! 123 Then, the output should be: LETTERS 10 DIGITS 3
```
ans=input()
digits=0
letters=0
for ch in ans:
    if ch.isalpha():
        letters+=1
    elif ch.isdigit():
        digits+=1
print("LETTERS", letters)
print("DIGITS", digits)

```

## output:
<img width="1403" height="358" alt="image" src="https://github.com/user-attachments/assets/0e05aadb-5bce-499f-97a2-de04c083aa72" />

## Write a program which can compute the factorial of a given numbers.The results should be printed in a comma-separated sequence on a single line.Suppose the following input is supplied to the program:8 Then, the output should be:40320
```

n=int(input())
fact=1
for i in range(1,n+1):
    fact=fact*i
print(fact)


```
## output:
<img width="1262" height="273" alt="image" src="https://github.com/user-attachments/assets/7adb76fd-b244-4d2b-90d2-731fa6eff681" />
