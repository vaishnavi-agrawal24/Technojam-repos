# Technojam-repos
<br>
Given an array of N integers, and an integer K, the task is to find the number of pairs of integers in the array whose sum is equal to K.
<br>
public class test1 {
<br>
    public static int getPairsCount(int[] arr, int n, int k) {
    <br>
        int count = 0;
        <br>
        for (int i = 0; i < n; i++) {
        <br>
            for (int j = i + 1; j < n; j++) {
            <br>
                if (arr[i] + arr[j] == k) {
                <br>
                    count++;
                <br>
                }
                <br>
            }
                <br>
        }
                <br>
        return count;
                <br>
    }
    <br>

    public static void main(String[] args) {
    <br>
        int[] arr = {1, 5, 7, -1};//here user can input there array
        <br>
        int n = arr.length;
        <br>
        int k = 6;
        <br>
        System.out.println("Number of pairs of integers in the array whose sum is equal to " + k + " is " + getPairsCount(arr, n, k));
        <br>
    }
    <br>
} 
<br>
