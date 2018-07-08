import numpy as np

#Question1
print("\nQuestion no1:\n")
arr = np.random.rand(10,1)
print(arr)
print(np.mean(arr))


#Question2
print("\nQuestion no2:\n")
B=np.random.rand(20,1)
print(B)
print(np.var(B))
print(np.std(B))


#Question3
print("\nQuestion no3:\n")
arrA=np.random.rand(10,20)
arrB=np.random.rand(20,25)
MulC=(np.matmul(arrA,arrB))
print("Multiplication of A and B is:\n",MulC)
SumC=(np.sum(MulC))
print("Sum of new Array is:\n",SumC)


#Question4
print("\nQuestion no4:\n")
A= np.random.rand(10,1)
print(A)
def func(x):
    return (1 / (1 + np.exp(-x)))

result = np.apply_along_axis(func, 0, A)

print('*'*50)

print(result)
