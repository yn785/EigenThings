# EigenThings

- This is just a representation of the power of SVD (Singular Value Decompasition)
- SVD basically states that any matrix can be represented into 3 other matrices.
- the 3 matrices are U S (aka sigma) and V^T:
- U and V^T are said to be Orthogonal Matrices, meaning: U^T = U^-1
- S is a diagnonal matrix

## SVD for regression

- SVD can be used for lineair regression:
- We know that if A is not a square matrix we can't use the inverse of A to solve A x = b
- However, We can use SVD to solve this.
- to get an exact solution b needs to be in the column space of A if not we can:
- A = U @ S @ V^T
- A* = U* @ S* @ V^T*
- So we have:
- A x= b
- U* @ S* @ V^T* x = b
- x = V @ S^-1@ U^T @ b
- This is the least squared solution for x

