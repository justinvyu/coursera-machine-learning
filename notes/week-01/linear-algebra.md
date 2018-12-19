# Linear Algebra Review

## Matrices

- Dimension: rows, cols
- Matrix elements: A<sub>ij</sub> = "*i*, *j* entry" in the *i*th row, *j*th column

## Vectors

- An n by 1 matrix
  - Refer to a vector of size n as a n-dimensional vector
  - ex: 
- Vector elements: y<sub>i</sub> = *i*th element
- 1-indexed or 0-indexed

## Matrix Addition and Scalar Multiplication

- Add up each index one at a time to form a sum matrix
- Must add two matrices of the same dimension
- Multiplying by a scalar means that every vlaue in the matrix is multiplied by that value

## Matrix-Vector Multiplication

- Number of columns in matrix must match the dimension of the vector
- To get the product, multiply the *i*th row of the matrix with the elements of the vector, then add them up
  - Do the same for each row of the matrix
- Product of a "m by n" matrix and an "n by 1" vector is an "m by 1" vector

## Matrix-Matrix Multiplication

- Perform matrix-vector multiplication using each column of the second matrix
  - Append the result of the matrix-vector multiplication as a column of the product matrix
- Product of "a by n" matrix and "n by b" matrix is "a by b"
- Can be used to compare competing hypotheses (multiply dataset matrix and parameter matrix)

## Matrix Multiplication Properties

- Matrix multiplication **is not** commutative
- Matrix multiplication **is** associative
- Identity matrix has 1 along diagonals and 0 everywhere else

## Inverse and Transpose

- Matrix inverse: if A is an "m by m" matrix, and if it has an inverse, A(A<sup>-1</sup>) = A<sup>-1</sup>A = I (identity matrix)
- Transpose: A<sup>T</sup> -> each row of A becomes each col of A<sup>T</sup>
- Let A be an "m by n" matrix, and let B = A<sup>T</sup>.
  - Then B is an "n by m" matrix and B<sub>ji</sub> = A<sub>ij</sub>
