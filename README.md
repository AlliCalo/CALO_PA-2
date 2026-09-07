# CALO_PA-2
This repository contains the solutions for PA#2 of ECE 2112, focusing on NumPy specifically on array creation, vectorized operations, Boolean filtering, and saving arrays as numpy files. 
I. Intended Learning Outcomes
At the end of this laboratory activity, the student should be able to:
1. create and reshape NumPy arrays using appropriate NumPy functions;
2. perform vectorized numerical operations on an ndarray;
3. compute array statistics and use Boolean conditions to select elements; and
4. save computed NumPy arrays as .npy files.

# Problem A : REPRODUCIBLE NORMALIZATION PROBLEM

Create a reproducible random 5×5 integer ndarray named X. Use the following two statements before
performing any calculation:

<img width="785" height="693" alt="image" src="https://github.com/user-attachments/assets/e6a0a9c6-dbfd-4d2e-83d9-2e5039631766" />

This code uses a random seed of 2112 to ensure that the same results can be reproduced each time it is run. It generates a 5 × 5 array containing random integers from 10 to 100. 
The program then calculates the population mean and standard deviation of the array and uses these values to normalize the data by
computing the Z-scores through vectorized operations. Finally, it displays both the original and normalized arrays and verifies that 
the normalized data has a mean of 0 and a standard deviation close to 1. The normalized array 
is then saved to a file named X_normalized.npy using np.save().

# Problem B : CUBES DIVISIBLE BY 4 PROBLEM

Using NumPy, create the first 100 positive integers, cube every element, and reshape the result into a
10 × 10 ndarray named C. Thus, C begins with 13 and ends with 1003. 
Use a Boolean condition on C to obtain every cubed value divisible by 4. Store the selected values in
div by 4. Preserve NumPy’s normal row-major selection order.

 <img width="1192" height="667" alt="image" src="https://github.com/user-attachments/assets/4e8b7dd0-d68b-4645-9a2e-90a174167ebd" />
 
This code creates the first 100 positive integers, cubes each number, and arranges the results into a 10 × 10 array named C. It then uses Boolean indexing to select all cubed values 
that are divisible by 4 and stores them in a one-dimensional array named divide_by_4. The program also performs verification checks to 
confirm that C has a shape of (10, 10), that 50 values were extracted, and that the values range from 8 to 1,000,000. 
The filtered array is then saved as div_by_4.npy using np.save().

# Problem C : ABOVE-MEAN SQUARES PROBLEM

Create a 6 × 6 ndarray named S containing the squares of the first 36 positive integers in increasing
row-major order. Compute the mean of all elements of S and store it in S mean. Then use Boolean
filtering to select only the elements strictly greater than S mean. Store these values in above mean.

<img width="928" height="670" alt="image" src="https://github.com/user-attachments/assets/54b454cd-002a-4bb3-9584-bf3adcc6de6c" />

The code starts by generating the first 100 positive integers and raising each number to the third power. The resulting values are then arranged into a 10 × 10 array called C. Using Boolean indexing, 
the program identifies and extracts all values that are divisible by 4 and stores them in a one-dimensional array named divide_by_4. 
It also performs several checks to verify that C has the correct shape, that 50 elements were extracted, and that the values range 
from 8 to 1,000,000. Finally, the filtered array is saved as div_by_4.npy using np.save().
