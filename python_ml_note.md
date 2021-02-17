## Python for Data Science and Machine Learning Bootcamp

## 1. Conda

+ **Create virtual environment**: `conda create --name <env name>`, or with `conda create --name <env name> python=3.6` to specify python version
+ **Create virtual environment from `.yml`file**: `conda env create -f environment.yml`

+ **check and update package version**: `conda list python`, `conda update python`

+ **activate environment**: `conda activate <env name>`





## 2. Numpy

1. **create a numpy array**: `np.array([1, 2, 3])`

2. **`np.linspace(low, high, num of points) vs np.arange(low, high, step)`**: third arguments are different

3. **other ways to generate NumPy Arrays**:

   + `np.zeros((row, col))`: `np.zeros((2,3))`
   + `np.empty((row, col))` 
   + `np.ones((row, col))`
   + `np.random.rand()`: return array with random number from unifom distribution over `[0, 1)`, `np.random.rand((row, col))`
   + `np.random.randn((row, col))`: return a sample from "strandard distribution"
   + `np.random.randint(low, high, (row, col))`: Return random integers from `low` (inclusive) to `high` (exclusive).

4. `reshape(5,5)`: change the size of the array, 

   ```python
   arr = np.random.randint(1, 11, 25)
   ## arr :
   ## array([ 2, 10,  5,  6,  3,  9,  2, 10,  8,  9,  1,  4,  3,  9,  5,  7,  3,
   ##      9,  6, 10,  4,  6,  7,  1,  2])
   arr.reshape(5,5)
   ## arr:
   ## array([[ 2, 10,  5,  6,  3],
   ##    		[ 9,  2, 10,  8,  9],
   ##     		[ 1,  4,  3,  9,  5],
   ##     		[ 7,  3,  9,  6, 10],
   ##     		[ 4,  6,  7,  1,  2]])
   
   ```

5. `arr.max(), arr.min(), arr.argmax(), arr.argmin()`, `argmax `or `argmin` returns index of max or min

6. `arr.dtype()` to return the data type of the array elements