# numpy-1
1, Create a null vector of size 10 but the fifth value which is 1.
 np.arange(10) == 4
array([False, False, False, False,  True, False, False, False, False, False], dtype=bool)
0np.arange(10) * 1
array([0, 0, 0, 0, 1, 0, 0, 0, 0, 0])
 np.arange(10) + 23
array([23, 23, 23, 23, 24, 23, 23, 23, 23, 23])

3.Create a 3x3 matrix with values ranging from 0 to 8
import numpy as np
x =  np.arange(0, 8).reshape(3,3)
print(x)


4. Find indices of non-zero elements from [1,2,0,0,4,0]

function myfind(c)
    a = similar(c, Int)
    count = 1
    @inbounds for i in eachindex(c)
        a[count] = i
        count += (c[i] != zero(eltype(c)))
    end
    return resize!(a, count-1)
end


5. Create a 10x10 array with random values and find the minimum and maximum values.
import numpy as np
x = np.random.random((5,5))
print("Original Array:")
print(x) 
xmin, xmax = x.min(), x.max()
print("Minimum and Maximum Values:")
print(xmin, xmax)



6. Create a random vector of size 30 and find the mean value.
import numpy as np
x = np.random.random(10)
print("Original array:")
print(x)
x.sort()
print("Sorted array:")
print(x)

