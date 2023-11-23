# Technojam-repos
<br>
<br>
1. Given an array of N integers, and an integer K, the task is to find the number of pairs of integers in the array whose sum is equal to K.
<br>
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
<br>
<br>
<br>
2. Given an array arr[] of size N-1 with integers in the range of [1, N], the task is to find the missing number from the first N integers.
<br>
<br>
import java.util.Arrays;
<br>
public class MissingNumber {
<br>
    public static int getMissingNumber(int[] arr, int n) {
    <br>
        int sum = Arrays.stream(arr).sum();
        <br>
        int expectedSum = n * (n + 1) / 2;
        <br>
        return expectedSum - sum;
        <br>
    }
    <br>
    public static void main(String[] args) {
    <br>
        int[] arr = {1, 2, 4, 6, 3, 7, 8};
        <br>
        int n = arr.length + 1;
        <br>
        System.out.println("The missing number from the first " + n + " integers is " + getMissingNumber(arr, n));
        <br>
    }
    <br>
}
<br>
<br>
<br>
<br>
3. Write a program to make a calculator.
<br>
<br>
import java.util.Scanner;
<br>
public class Calculator {
                <br>
    public static void main(String[] args) {
                <br>
        Scanner scanner = new Scanner(System.in);
                <br>
        System.out.print("Enter the first number: ");
                <br>
        double num1 = scanner.nextDouble();
                <br>
        System.out.print("Enter the second number: ");
                <br>
        double num2 = scanner.nextDouble();
                <br>
        System.out.print("Enter the operator (+, -, *, /): ");
                <br>
        char operator = scanner.next().charAt(0);
                <br>
        double result;
        <br>
        switch (operator) {
                <br>
            case '+':
                <br>
                result = num1 + num2;
                <br>
                break;
                <br>
            case '-':
                <br>
                result = num1 - num2;
                <br>
                break;
                <br>
            case '*':
                <br>
                result = num1 * num2;
                <br>
                break;
                <br>
            case '/':
                <br>
                result = num1 / num2;
                <br>
                break;
                <br>
            default:
                <br>
                System.out.println("Invalid operator!");
                <br>
                return;
                <br>
        }
        <br>
        System.out.println(num1 + " " + operator + " " + num2 + " = " + result);
                <br>
    }
                <br>
}
<br>
<br>
<br>
<br>
4. Find the factorial of a large number.
<br>
<br>
import java.math.BigInteger;
                <br>
public class Factorial {
                <br>
    public static void main(String[] args) {
                <br>
        int num = 1000;
                <br>
        BigInteger factorial = BigInteger.ONE;
                <br>
        for(int i = 1; i <= num; ++i) {
            <br>
            factorial = factorial.multiply(BigInteger.valueOf(i));
            <br>
        }
            <br>
        System.out.printf("Factorial of %d = %d", num, factorial);
            <br>
    }
            <br>
}
<br>
<br>
<br>
<br>
5. write a program to reverse an array
<br>
<br>
public class arrayReverse { 
            <br>
    static void reverse(int a[], int n) 
            <br>
    { 
            <br>
        int i, k, t; 
            <br>
        for (i = 0; i < n / 2; i++) { 
            <br>
            t = a[i]; 
            <br>
            a[i] = a[n - i - 1]; 
            <br>
            a[n - i - 1] = t; 
            <br>
        } 
        <br> 
        System.out.println("Reversed array is: \n"); 
            <br>
        for (k = 0; k < n; k++) { 
                          <br>
            System.out.println(a[k]); 
            <br>
        } 
            <br>
    } 
    <br>
    public static void main(String[] args){ 
            <br>
        int[] arr = { 10, 20, 30, 40, 50 }; 
            <br>
        reverse(arr, arr.length);
            <br>
    } 
            <br>
}
<br>
<br>
<br>
<br>
