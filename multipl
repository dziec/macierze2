def matrix_input():
    matrix1_dim1 = int(input("Enter first dimension of first matrix: "))
    matrix1_dim2 = int(input("Enter second dimension of first matrix: "))
    matrix2_dim1 = int(input("Enter first dimension of second matrix: "))
    matrix2_dim2 = int(input("Enter second dimension of second matrix: "))
    if matrix1_dim2 != matrix2_dim1:
        print("You can't multiply entered matrix.")
        print("Please enter correct value ")
        print("(second dimension of first matrix must ")
        print("be the same as first dimension of second matrix)")
        return matrix_input()
    else:
        dim = [
            [matrix1_dim1, matrix1_dim2],
            [matrix2_dim1, matrix2_dim2]
        ]
    matrix1 = [[int(input("Enter values in first matrix (in lines): ")) for row in range(0, dim[0][1])] for col in range(0, dim[0][0])]
    matrix2 = [[int(input("Enter value: in second matrix (in lines): ")) for row in range(0, dim[1][1])] for col in range(0, dim[1][0])]
    result = [matrix1, matrix2, dim]
    return result


def matrix_mul(mtrx):
    mtrx1 = mtrx[0]
    mtrx2 = mtrx[1]
    dim = mtrx[2]
    result = []
    n = dim[0][0]
    m = dim[1][-1]
    result = [0] * n
    for i in range(n):
        result[i] = [0] * m
    for i in range(len(mtrx1)):
        for j in range(len(mtrx2[0])):
            for k in range(len(mtrx2)):
                result[i][j] += mtrx1[i][k] * mtrx2[k][j]
    return result


print(matrix_mul(matrix_input()))
