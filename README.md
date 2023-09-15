# Program-to-find-Smallest-Element-of-the-array-using-Recursion-in-Java

Smallest Element of  the array using Recursion in Java
Here, on this page, we will learn about the program to find the smallest element of the array using recursion in Java. We are given an array and we need to print the smallest element. We will discuss the approach using recursion and iteratively both to find the smallest element.

Example :

Input : arr[5]= {15, 60, -6, 0, 2,}
Output :  Smallest Element is : -6
Smallest Element of the array using Recursion
Method 1 (Using Recursion):
In this method we will discuss the recursive solution to find the smallest element of an array. We will do the following steps to achieve the smallest element.

Create a recursive function say smallest_element(int n, int arr).
Base Condition : If(n==1) return arr[0].
Else, return min(arr[n-1], smallest_element(n-1, arr).
Smallest Element using Recursion In Java
Time and Space Complexity
Time Complexity : O(n), where n is the size of the array. Space Complexity : O(1)
Code in Java
Run
//Largest Element of the array using Recursion in Java
public class Main {
     public static int findMinimum(int A[], int n)
    {
      // if size = 0 means whole array has been traversed
      if(n == 1)
        return A[0];
         
        return Math.min(A[n-1], findMinimum(A, n-1));
    }
     
    // Driver code
    public static void main(String args[])
    {
        int A[] = { 15, 60, -6, 0, 2};
        int n = A.length;
        // Function calling
        System.out.println("Smallest element in the array is: "+findMinimum(A, n));
    }
}
Output

Smallest element in the array is: -6
Related Pages
Finding Number of times x digit occurs in a given input
 
Finding number of integers which has exactly x divisors
 
Largest element in an array

Power of a Number

Prime Number

Prime Course Trailer

Related Banners
Get PrepInsta Prime & get Access to all 200+ courses offered by PrepInsta in One Subscription

Get Prime
Method 2 (Iterative Solution)
 

STEP 1: START
STEP 2: INITIALIZE arr[] =  {-5, 1, 7, 6, 3}
STEP 3: Lets suppose the element at index 0 is the minimum so min = arr[0]
STEP 4: Repeat the STEP 5 for(i=0; i< arr.length; i++)
STEP 5: Check if the arr[i] is less than the min if its then update the min to (min=arr[i])
STEP 6: PRINT “Smallest element in given array:”
STEP 7: PRINT min
STEP 8: END
Run
public class Main
{
   public static void main(String[] args) {  
  
        //Initialize array  
        int [] arr = new int [] {-5, 1, 7, 6, 3};  
        //Initialize min with first element of array.  
        int min = arr[0];  
        //Loop through the array  
        for (int i = 0; i < arr.length; i++) {  
            //Compare elements of array with min  
           if(arr[i] < min)  
               min = arr[i];  
        }  
        System.out.println("Smallest element present in given array: " + min);  
    }  
}
Output
Smallest element present in given array: -5
