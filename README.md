# NUMPY
## Important Numpy Functions and Properties
- array.dtype 
- array.ndim 
- array.shape
- np.arange()
## Vocab Numpy
- Vector - single dimensional array
- Matrix - two dimensional array
- 3d matrix - 3 dimensional array



**Main Idea**

NumPy is a Python library used for numerical computing, data analysis, scientific computing, and machine learning. Its biggest strength is that it processes array-based data faster than Python lists, uses memory more efficiently, and supports vectorized operations without needing manual loops.

**Key Points**

- NumPy’s main object is `ndarray`, which means a multidimensional array.
- NumPy arrays are usually **homogeneous**, meaning all elements have the same data type.
- A 1D array is like a vector, a 2D array is like a matrix, and a 3D array is like a tensor.
- You can create arrays using:
  ```python
  np.array([1, 2, 3])
  np.arange(start, stop, step)
  np.zeros()
  np.ones()
  np.linspace()
  np.random
  ```
- `np.arange(1, 30)` returns numbers from `1` to `29` because the `stop` value is not included.

**Array Attributes**

Important attributes:

```python
arr.ndim   # number of dimensions
arr.shape  # size of each dimension
arr.size   # total number of elements
arr.dtype  # data type
```

**dtype**

`dtype` tells you the data type stored in the array, for example:

```python
np.int32
np.float64
np.complex128
bool
object
```

You can specify the dtype when creating an array:

```python
arr = np.array([1, 2, 3], dtype=np.int32)
```

**Important Operations**

Indexing:

```python
arr[2]
```

Slicing:

```python
arr[1:4]
```

This returns the elements at index `1`, `2`, and `3`, but not index `4`.

Arithmetic operations:

```python
arr + 1
arr * 2
arr / 2
```

Aggregate functions:

```python
np.sum(arr)
np.mean(arr)
np.median(arr)
np.std(arr)
np.min(arr)
np.max(arr)
```

**2D Arrays**

You can transpose and reshape arrays:

```python
matrix.T
matrix.reshape(3, 2)
```

**Boolean Operations**

NumPy supports:

```python
np.logical_and(a, b)
np.logical_or(a, b)
np.logical_not(a)
np.array_equal(a, b)
```

**Sorting, Searching, and Counting**

```python
np.sort(arr)
3 in arr
np.argmin(arr)
np.argmax(arr)
np.count_nonzero(arr)
np.unique(arr)
```

**NumPy vs List**

Use NumPy when working with large numerical datasets, statistical calculations, matrices, machine learning, or when performance matters. Use Python lists for simple, small datasets or when the data contains different types.

**Knowledge Check Answers**

- Specify dtype when creating an array: **C**
- `arr[1:4]` returns indexes 1, 2, and 3: **B**
- Element-wise comparison means comparing each corresponding element: **B**