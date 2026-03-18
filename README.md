a, b = 0, 1
m, n = input().split()
m, n = int(m), int(n)
s = []
while a < n:  
    s.append(a)  
    a, b = b, a + b
s1 = [i for i in s if i >= m]
if len(s1) > 0:
    print(*s1)
else:
    print('В заданном диапазоне нет чисел Фибоначчи')
