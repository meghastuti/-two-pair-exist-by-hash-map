import java.io.*;
import java.util.HashSet;
public class PairExist
{
    static void printpairs(int arr[], int sum)
    {
        HashSet<Integer> hash = new HashSet<>();
        for (int i = 0; i < arr.length; i++)
        {
            int num = sum - arr[i];
        
            if (hash.contains(num)) 
        {
            System.out.print("The two numbers are "+ num +" and "+ arr[i]);
        }
          hash.add(arr[i]);
        }
    }
        public static void main(String[] args)
    {
        int arr[] = { 1, 4, 45, 6, 10, 8 };
        int sum = 16;
        printpairs(arr, sum);
    }
 }
