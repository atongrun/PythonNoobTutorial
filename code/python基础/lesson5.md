# %% [markdown]
# 条件判断和循环

# %%
age = 20
if age >= 28:
    print('your age is', age)
    print('adult')

# %%
age = 30
if age >= 18:
    print('your age is', age)
    print('adult')
else:
    print('your age is', age)
    print('teenager')

# %%
age = 18
if age >= 18:
    print('adult')
elif age >= 6:
    print('teenager')
else:
    print('kid')

# %%
age = 20
if age >= 6:
    print('teenager')
elif age >= 18:
    print('adult')
else:
    print('kid')

# %%
x=-2
if x:
    print('true')
else:
    print('False')



# %%
birth = input('birth: ')
if birth < 2000:
    print('00前')
else:
    print('00后')

# %%
s = input('birth: ')
birth = int(s)
if birth < 2000:
    print('00前')
else:
    print('00后')

# %%
height = 1.75
weight = 80.5

# 低于18.5：过轻
# 18.5-25：正常
# 25-28：过重
# 28-32：肥胖
# 高于32：严重肥胖

bmi=weight/height**2
print(bmi)

if bmi<18.5:
    print('过轻')
elif bmi>=18.5 and bmi<25:
    print('正常')
elif bmi>=25 and bmi<28:
    print('过重')
elif bmi>=28 and bmi<32:
    print('肥胖')
else:
    print('严重肥胖')

# %% [markdown]
# 上边的内容是条件判断

# %%
names = ['Michael', 'Bob', 'Tracy']
for name in names:
    print(name)

# %%
sum = 0
for x in [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]:
    sum = sum + x
    print(sum)
print(sum)

# %% [markdown]
# range(5)
# [0 , 5)
# 
# 0 1 2 3 4

# %%
# print(list(range(5)))
sum = 0
for x in range(101):  # 0 + 1 + 2 + ... + 100
    sum = sum + x
print(sum)

# %% [markdown]
# 上边是for循环

# %%
sum = 0
# n = 99
# while n > 0:
#     sum = sum + n
#     n = n - 2
# print(sum)

for i in range(100):  # i从0 - 99
    if i%2!=0:
        sum=sum+i
print(sum)

# %%
n = 1
while n <= 100:
    if n > 10: # 当n = 11时，条件满足，执行break语句
        break # break语句会结束当前循环
    print(n)
    n = n + 1
print('END')

# %%
n = 0
while n < 10:
    n = n + 1
    if n % 2 == 0: # 如果n是偶数，执行continue语句
        continue # continue语句会直接继续下一轮循环，后续的print()语句不会执行
    print(n)

# %%
n = 0
while n < 10:
    n = n + 1
    if n % 2 != 0: # 如果n是偶数，执行continue语句
        print(n)

# %%
n = 10
while n>0:
    print(n)
    n=n-1
    if n==1:
        n=n+10



# %%
x =1
while x:
    print('死循环')


