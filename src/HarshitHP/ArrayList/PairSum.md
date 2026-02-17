import java.util.*;
public class PairSum {
public static void findPairs(int[] arr, int target){
for(int i = 0; i< arr.length; i++){
for(int j = i+1; j< arr.length; j++){
if(arr[i] + arr[j] == target){
System.out.println(arr[i] + "," + arr[j]);
}
}
}
}

    static void main(String[] args) {
        int[] arr = {2,4,3,5,7};
        int sum = 7;

        findPairs(arr,sum);
    }
}
