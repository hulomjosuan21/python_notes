## Iterate Row

```python
def iterate_by_rows(matrix):
    for row in matrix:  # Loop through each row
        for elem in row:  # Loop through each element in the row
            print(elem, end=" ")  # Print the element with space
    print()  # Print a new line after finishing all rows
```

## Iterate Column

```python
def iterate_by_columns(matrix):
    for col in range(len(matrix[0])):  # Loop through each column index (0 to number of columns)
        for row in range(len(matrix)):  # Loop through each row index (0 to number of rows)
            print(matrix[row][col], end=" ")  # Print the element in column-first order
    print()  # Print a new line after finishing all columns
```

## Sum Matrix

```python
def iterate_by_rows(matrix):
    row_sums = []
    for row in matrix:  # Loop through each row
        row_sum = sum(row)  # Calculate row sum
        row_sums.append(row_sum)
    return row_sums  # Return a list of row sums

def iterate_by_columns(matrix):
    col_sums = []
    for col in range(len(matrix[0])):  # Loop through each column index
        col_sum = sum(matrix[row][col] for row in range(len(matrix)))  # Sum column elements
        col_sums.append(col_sum)
    return col_sums  # Return a list of column sums

def check_matrix_sums(matrix, n):
    row_sums = iterate_by_rows(matrix)
    col_sums = iterate_by_columns(matrix)

    # Check if all rows and columns have sum equal to n
    return all(sum_val == n for sum_val in row_sums) and all(sum_val == n for sum_val in col_sums)
```
