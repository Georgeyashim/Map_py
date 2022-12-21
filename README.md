# Map_py

# LAMBDA FUNCTION

nums = [1, 2, 3, 4, 5, 6]
print('You have a list of ', nums)


square_nums = []

square = lambda  n : n ** 2

for n in nums:
    square_nums.append(square(n))

print(square_nums)

num1 = [2, 3, 5, 7, 11, 13]

trip_num1 = []

tripple = lambda m : m ** 3

for m in num1:
    trip_num1.append(tripple(m))

print(trip_num1)

# MAP FUNCTION

num2  = [2, 4, 6, 8, 10, 12, 14, 16, 18, 20]

odd = list(map(lambda n:n+1, num2))

print(odd)

print(len(num2))


num3 = [10, 20, 30, 40, 50, 60, 70, 80, 90, 100]

div = list(map(lambda n:n/10, num3))
print(div)

div23 = map(lambda a, c: a / c, num3, num2)

print(list(div23))

reap = map(lambda a, c:  a - c,  num3, num2)

print(list(reap))

#  FILTER FUNCTION

div90 = filter(lambda  a : a % 90 == 0, num3 )
print(list(div90))

div5 = filter(lambda a : a / 2 == 5, num2)
print(list(div5))
