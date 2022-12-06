# QuantitativeFin_JupyterNote_practices
A repository for practising numpy/pandas/matplotlib and doing some data analysis in Financial Field

---

## **Numpy techniques:** <br />

### Array

#### - Create a simple array:
import numpy as np 
1. make an array: arr = arr.array([1,2,3])
2. make a 2D array: arr = arr.array([1,2,3],[4,5,6])
3. tips: if elements in the array are different type, the precedency will be str > float > int. <br />

#### - Reading pictures:
import matplotlib.pyplot as plt
1. get image array: img_arr = plt.imread('...'), which will return a 3D array.
2. show the image by the image array: plt.imshow(img_arr).
3. tips: if we modify the array, for example: img_arr = img_arr-100, we will have different picture as we modified the picture directly by deducting 100 for each element in the array.

#### - Create more complicated array
1. make 2D array fill with ones: np.ones(shape(3,4)), which basically can be understood as an 3*4 matrix.
2. make evenly spaced numbers over an interval: np.linspace(0,10,num=20).
3. make arithmatic progression: np.arrange(10,50,step=2), each difference is 2 from 10 to 50 (not including 50).
4. make random 2D array with specified size: arr = np.random.randint(0,100,size=(5,3)), which is a 5*3 matrix with random element inside.

#### - Get Common properties from numpy array
1. get the shape: arr.shape
2. get the dimension: arr.ndim
3. get the number of elements in the array: arr.size
4. get the element data type in the array: arr.dtype

#### - Search and cut
example array: arr = np.random.randint(1,100,size=(5,6))
1. get the first row: arr[0]
2. get rows by their index: arr[[0,1,2]]
3. get first two rows: arr[0:2]
4. get first tow cols: arr[:,0:2]
5. reverse rows: arr[::-1]
6. reverse cols: arr[:,::-1]
7. reverse all: arr[::-1,::-1]




