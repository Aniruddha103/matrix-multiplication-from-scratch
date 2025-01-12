## Matrix Multiplication in Python from scratch

This project demonstrates matrix multiplication implemented from scratch in Python and validates the results using NumPy's `dot` function.

---

### **Description**
Matrix multiplication is a fundamental operation in linear algebra, commonly used in fields like computer science, machine learning, and physics. This program includes:
1. A custom Python function to multiply matrices.
2. Verification of results using NumPy, a powerful numerical computation library.

---

### **Files**
- **`matrix_multiplication.ipynb`**: Contains the implementation of the custom matrix multiplication function, test matrices, and validation logic.

---

### **Usage**
1. Import the program or copy the function into your Python environment.
2. Run the script to see the results of multiplying two 2x2 matrices.

---

### **Key Components**
1. **Custom Matrix Multiplication**:
   - Function `multiply_matrices(A, B)` multiplies two matrices using a triple nested loop.
   - Ensures compatibility between matrix dimensions (columns of the first matrix = rows of the second).

2. **Test Data**:
   - Matrix `A`: Created using NumPy, values `[4, 5, 6, 7]`, reshaped into a 2x2 matrix.
   - Matrix `B`: Created using NumPy, values `[0, 1, 2, 3]`, reshaped into a 2x2 matrix.

3. **Validation**:
   - The result of the custom multiplication is validated using NumPy’s `np.dot()` method.

---

### **Example Output**
When running the program, you can expect the following output:
```python
[[10, 13],
 [22, 29]]

[[10 13]
 [22 29]]
```

---

### **How It Works**
1. **Input Matrices**: Matrices are generated using `np.arange` and reshaped to 2x2.
2. **Custom Function**: `multiply_matrices(A, B)` calculates the result through iterative addition and multiplication.
3. **Validation**: The result is compared to NumPy’s optimized `dot` function output.

---

### **Dependencies**
- Python 3.x
- NumPy library

---

### **Error Handling**
- The function raises a `ValueError` if the matrices cannot be multiplied due to dimension mismatch.

---

### **Next Steps**
- Expand the function to handle matrices of arbitrary dimensions.
- Optimize the function using NumPy for faster computation of large matrices.

