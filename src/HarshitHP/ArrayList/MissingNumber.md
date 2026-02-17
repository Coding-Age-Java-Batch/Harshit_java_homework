import java.util.*;

public class MissingNumber {

    public static int findMissing(int[] arr, int n){

        int expectedSum = n * (n+1) / 2;
        int actualSum = 0;

        for(int num : arr){
            actualSum = actualSum + num;
        }
        return expectedSum - actualSum;
    }

    static void main(String[] args) {
        int[] arr = {1,2,4,5};
        int n = 5;
        System.out.print("Missing Number is: " +findMissing(arr,n));
    }
}
