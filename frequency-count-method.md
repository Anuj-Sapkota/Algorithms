# Frequency Count Method

## 1. Method to find sum of all elements of an Array
    Algorithm Sum(A,n)
    {
        S = 0; ------> 1 times
        for (i=0;i<n;i++) ----> i = 0 (1 times), i<n (n+1 times), i++ (n times)
        {
            S = S + A[i]; ------> n time
        }
        return S; -------> 1 time
    }

----
    A = [8,3,9,7,2]
     length = 5 or n = 5

    Now the time function is the sum of the values meaning
        { the statement for(i=0; i<n; i++) said to be used n+1 time for simplicity}
----------------------
### Time
     Time Function:  f(n)= 2n + 3 
     Order of n: O(n) as the function is of order 1 

---
### Space
    A ---> size is n words
    n ---> 1 word
    s ---> 1 word
    i ---> 1 word
---------------------
    Total is n + 3 

    Order of polynomial is also: O(n)


--------------

## 2. Finding sum of two matrices

    Algorithm Add(A, B, n)
    {
        for (i=0; i<n; i++)
        {
            for (j=0; j<n; j++)
            {
                C[i,j] = A[i,j] + B[i,j]
            }
        }
    }

    A and B are square matrices of n * n dimensions

### 2.1 Time complexity
     Algorithm Add(A, B, n)
    {
        for (i=0; i<n; i++) ----------------> n + 1
        {
           // This whole inner loop will execure for n times due to the outer loop
            for (j=0; j<n; j++) ------------> n * (n + 1)
            {
                C[i,j] = A[i,j] + B[i,j] ---> n  * n 
            }
        }
    }

#### **Time Taken:** 
#### f(n) = $n+ (n \times (n + 1)) + (n \times n)$:
#### f(n) = $2n^2 + 2n + 1$
#### **Order**: $O(n^2)$

### 2.2 Space Complexity
    Total words used:

        A --> n x n
        B --> n x n
        C --> n x n 
        n --> 1
        i --> 1
        j --> 1
#### Space Function S(n) = $3n^2 + 3$
#### **Order**: $O(n^2)$

---
## 3. Multiplication of two matrices
