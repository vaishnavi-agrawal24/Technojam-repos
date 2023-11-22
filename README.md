# Technojam-repos
repo for technojam
<br>
Given an array of N integers, and an integer K, the task is to find the number of pairs of integers in the array whose sum is equal to K.
<br>
public class test1 {
    public static int getPairsCount(int[] arr, int n, int k) {
        int count = 0;
        for (int i = 0; i < n; i++) {
            for (int j = i + 1; j < n; j++) {
                if (arr[i] + arr[j] == k) {
                    count++;
                }
            }
        }
        return count;
    }

    public static void main(String[] args) {
        int[] arr = {1, 5, 7, -1};//here user can input there array
        int n = arr.length;
        int k = 6;
        System.out.println("Number of pairs of integers in the array whose sum is equal to " + k + " is " + getPairsCount(arr, n, k));
    }
} 
<br>
This is a Java program that finds the number of pairs of integers in an array whose sum is equal to a given number. Here’s how it works:

First, we define an array of integers and a number K.
We then use a nested loop to iterate over all possible pairs of integers in the array.
For each pair, we check if their sum is equal to K.
If so, we increment a counter variable.
Finally, we return the value of the counter variable.
Here’s the same program written in pseudocode:
<br>
function getPairsCount(arr, n, k):
    count = 0
    for i = 0 to n-1:
        for j = i+1 to n-1:
            if arr[i] + arr[j] == k:
                count = count + 1
    return count

arr = [1, 5, 7, -1]
n = len(arr)
k = 6
print("Number of pairs of integers in the array whose sum is equal to", k, "is", getPairsCount(arr, n, k))
