def rotate_matrix(matrix):
    return [list(reversed(col)) for col in zip(*matrix)]

n = int(input("Enter the size of the matrix (n x n): "))
matrix = []
print("Enter the matrix row by row:")
for i in range(n):
    row = list(map(int, input().split()))
    matrix.append(row)

rotated_matrix = rotate_matrix(matrix)

print("Rotated matrix:")
for row in rotated_matrix:
    print(row)
