
1. Import TensorFlow library:

```python
import tensorflow as tf
```

2. Create tensors:

```python
# Create a 0-dimensional (scalar) tensor
tensor_0d = tf.constant(5)

# Create a 1-dimensional (vector) tensor
tensor_1d = tf.constant([1, 2, 3, 4, 5])

# Create a 2-dimensional (matrix) tensor
tensor_2d = tf.constant([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
```

```python
# Create a 1-dimensional tensor with variables
variable_tensor = tf.Variable([1, 2, 3, 4, 5])

# Change its values
variable_tensor.assign([6, 7, 8, 9, 10]) # Change values
```

3. Basic arithmetic operations:

```python
# Addition
tensor_a = tf.constant([1, 2, 3])
tensor_b = tf.constant([4, 5, 6])
tensor_sum = tf.add(tensor_a, tensor_b)

# Subtraction
tensor_diff = tf.subtract(tensor_a, tensor_b)

# Multiplication (element-wise)
tensor_product = tf.multiply(tensor_a, tensor_b)

# Division (element-wise)
tensor_div = tf.divide(tensor_a, tensor_b)
```

4. Matrix operations:

```python
# Matrix multiplication
tensor_c = tf.constant([[1, 2], [3, 4]])
tensor_d = tf.constant([[5, 6], [7, 8]])
tensor_matmul = tf.matmul(tensor_c, tensor_d)

# Transpose
tensor_transpose = tf.transpose(tensor_c)

# Inverse
tensor_inverse = tf.linalg.inv(tensor_c)
```

5. Reshaping tensors:

```python
# Reshape a tensor
tensor_1d = tf.constant([1, 2, 3, 4, 5, 6])
tensor_reshaped = tf.reshape(tensor_1d, (2, 3))
```

6. Broadcasting:

```python
# Broadcasting a tensor
tensor_e = tf.constant([1, 2, 3])
tensor_f = tf.constant([[4, 5, 6], [7, 8, 9]])
tensor_broadcast = tf.add(tensore, tensor_f)
```

7. Reduction operations:

```python
# Sum of all elements in a tensor
tensor_g = tf.constant([1, 2, 3, 4, 5])
tensor_sum = tf.reduce_sum(tensor_g)

# Mean of all elements in a tensor
tensor_mean = tf.reduce_mean(tensor_g)

# Maximum and minimum elements in a tensor
tensor_max = tf.reduce_max(tensor_g)
tensor_min = tf.reduce_min(tensor_g)
```

8. Concatenating tensors:

```python
# Concatenate two tensors along the first dimension
tensor_h = tf.constant([[1, 2], [3, 4]])
tensor_i = tf.constant([[5, 6], [7, 8]])
tensor_concat = tf.concat([tensor_h, tensor_i], axis=0)
```

9. Splitting tensors:

```python
# Split a tensor into multiple tensors along the first dimension
tensor_j = tf.constant([[1, 2], [3, 4], [5, 6], [7, 8]])
tensor_split = tf.split(tensor_j, num_or_size_splits=2, axis=0)
```

10. Slicing tensors:

```python
# Slice a tensor to extract a sub-tensor
tensor_k = tf.constant([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
tensor_slice = tensor_k[1:, 1:]
```