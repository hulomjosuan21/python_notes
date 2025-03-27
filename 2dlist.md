## 1
```python
def iterate_by_rows(matrix):
    row_sums = []
    for row in matrix:
        row_sums.append(sum(row))  # Store sum of each row
    return row_sums

def iterate_by_columns(matrix):
    col_sums = []
    for col in range(len(matrix[0])):  
        col_sums.append(sum(matrix[row][col] for row in range(len(matrix))))  # Store sum of each column
    return col_sums

def iterate_by_diagonals(matrix):
    main_diagonal_sum = sum(matrix[i][i] for i in range(len(matrix)))  # Top-left to bottom-right
    anti_diagonal_sum = sum(matrix[i][len(matrix) - 1 - i] for i in range(len(matrix)))  # Top-right to bottom-left
    return main_diagonal_sum, anti_diagonal_sum

def check_matrix_sums(matrix, n):
    row_sums = iterate_by_rows(matrix)
    col_sums = iterate_by_columns(matrix)
    main_diag, anti_diag = iterate_by_diagonals(matrix)

    # Check if all rows, columns, and both diagonals have sum equal to n
    return (all(sum_val == n for sum_val in row_sums) and 
            all(sum_val == n for sum_val in col_sums) and 
            main_diag == n and 
            anti_diag == n)

```

## 2
```python
def print_by_rows(matrix):
    print("Rows:")
    for row in matrix:
        print(" ".join(map(str, row)))  # Print each row

def print_by_columns(matrix):
    print("\nColumns:")
    for col in range(len(matrix[0])):  
        for row in range(len(matrix)):
            print(matrix[row][col], end=" ")  # Print column elements in order
        print()  # New line after each column

def print_by_diagonals(matrix):
    print("\nMain Diagonal:")
    for i in range(len(matrix)):
        print(matrix[i][i], end=" ")  # Print top-left to bottom-right elements
    print()

    print("\nAnti-Diagonal:")
    for i in range(len(matrix)):
        print(matrix[i][len(matrix) - 1 - i], end=" ")  # Print top-right to bottom-left elements
    print()
```
