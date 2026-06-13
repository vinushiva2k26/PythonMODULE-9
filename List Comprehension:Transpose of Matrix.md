# 🧮 List Comprehension:Transpose of Matrix 

## 🎯 AIM:
To write a Python program to compute the **transpose** of a matrix using **list comprehension**.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create variables `r` and `c` to represent the number of rows and columns of the matrix.
3. Get the values of `r` and `c` from the user.
4. Define a function `create(r, c)` to create the matrix by reading the elements from the user.
5. Use **list comprehension** to calculate the transpose of the matrix.
6. Print the transposed matrix.
7. **Stop**

---

## 💻Program

```python
def create(r, c):
    matrix = []
    for i in range(r):
        row = list(map(int, input().split()))
        matrix.append(row)
    return matrix

r = int(input())
c = int(input())

matrix = create(r, c)

transpose = [[matrix[j][i] for j in range(r)] for i in range(c)]

for row in transpose:
    print(row)
```

## Output

```text
2
3
1 2 3
4 5 6
[1, 4]
[2, 5]
[3, 6]
```

## Result

Thus, the Python program was successfully executed to find the transpose of a matrix using list comprehension.


