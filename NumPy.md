# **NumPy Cheat Sheet for Machine Learning 📊**

A quick reference guide for essential **NumPy** operations, focusing on array manipulation, mathematical operations, and useful functions for machine learning. Easily copy and paste the code snippets you need!

---

## **📥 Importing NumPy**
```python
import numpy as np
```

---

## **📂 Creating Arrays**

### **Create 1D, 2D, and 3D Arrays**
```python
arr_1d = np.array([1, 2, 3])
arr_2d = np.array([[1, 2, 3], [4, 5, 6]])
arr_3d = np.array([[[1, 2], [3, 4]], [[5, 6], [7, 8]]])
```

### **Create Arrays with Zeros, Ones, and Constants**
```python
zeros_array = np.zeros((3, 3))
ones_array = np.ones((2, 2))
constant_array = np.full((2, 2), 7)
```

### **Create an Array with a Range of Values**
```python
arr_range = np.arange(0, 10, 2)  # [0, 2, 4, 6, 8]
```

### **Create an Array with Linearly Spaced Values**
```python
arr_linspace = np.linspace(0, 1, 5)  # [0. , 0.25, 0.5, 0.75, 1. ]
```

### **Create Random Arrays**
```python
random_array = np.random.rand(3, 3)      # Random values between 0 and 1
random_ints = np.random.randint(1, 10, (2, 2))  # Random integers
```

---

## **🔍 Exploring Arrays**

### **Get Array Properties**
```python
print(arr.shape)   # Shape of the array (rows, columns)
print(arr.size)    # Total number of elements
print(arr.ndim)    # Number of dimensions
print(arr.dtype)   # Data type of elements
```

### **Reshape Arrays**
```python
reshaped = arr.reshape(3, 2)  # Change shape to 3 rows, 2 columns
```

### **Flatten an Array**
```python
flattened = arr.flatten()
```

---

## **🛠 Array Indexing and Slicing**

### **Indexing (Access Elements)**
```python
print(arr[0, 1])  # Access element at row 0, column 1
```

### **Slicing (Select Elements)**
```python
print(arr[:, 1])   # Select all rows, column 1
print(arr[1:, :2]) # Select row 1 onwards, first 2 columns
```

---

## **🔄 Array Manipulation**

### **Concatenate Arrays**
```python
arr_concat = np.concatenate((arr1, arr2), axis=0)  # Vertically (rows)
```

### **Stack Arrays**
```python
arr_stack = np.vstack((arr1, arr2))  # Stack vertically
```

### **Split Arrays**
```python
split_arrays = np.split(arr, 3)  # Split into 3 equal parts
```

---

## **📈 Mathematical Operations**

### **Basic Operations**
```python
sum_arr = np.sum(arr)
mean_arr = np.mean(arr)
median_arr = np.median(arr)
std_arr = np.std(arr)
```

### **Element-wise Operations**
```python
arr_squared = arr ** 2
arr_sqrt = np.sqrt(arr)
arr_exp = np.exp(arr)
arr_log = np.log(arr)
```

---

## **📊 Linear Algebra Operations**

### **Matrix Multiplication**
```python
result = np.dot(arr1, arr2)
```

### **Transpose a Matrix**
```python
transposed = arr.T
```

### **Inverse of a Matrix**
```python
inverse = np.linalg.inv(arr)
```

### **Eigenvalues and Eigenvectors**
```python
eigenvalues, eigenvectors = np.linalg.eig(arr)
```

---

## **🗑 Handling Missing Values**

### **Check for NaN values**
```python
np.isnan(arr)
```

### **Replace NaN values**
```python
arr[np.isnan(arr)] = 0
```

---

## **🔗 Broadcasting and Vectorization**

### **Broadcasting Examples**
```python
arr + 10      # Adds 10 to every element
arr * [1, 2]  # Multiplies each column by corresponding value
```

### **Vectorized Operations**
```python
result = np.sin(arr)
```

---

## **💾 Saving and Loading Data**

### **Save and Load Arrays**
```python
np.save('array.npy', arr)
loaded_arr = np.load('array.npy')
```

### **Save and Load CSV**
```python
np.savetxt('data.csv', arr, delimiter=',')
loaded_csv = np.loadtxt('data.csv', delimiter=',')
```

---

## **📚 Additional Resources**

- [NumPy Official Documentation](https://numpy.org/doc/)
- [NumPy Cheat Sheet (PDF)](https://numpy.org/doc/stable/user/quickstart.html)
- [Machine Learning with NumPy](https://www.kaggle.com/learn/intro-to-programming)

---

Enjoy coding with **NumPy**! 🚀 If you find this guide helpful, feel free to share. 😊
