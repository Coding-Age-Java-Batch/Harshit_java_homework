import java.util.*;
public class RearrangeArray {
public static void rearrange(int[] arr){
int[] temp = new int[arr.length];
int index = 0;

         for(int num : arr){
             if(num < 0){
                 temp[index++] = num;
             }
         }

         for(int num : arr){
             if(num >= 0){
                 temp[index++] =  num;
             }
         }

         for(int i = 0; i<arr.length; i++){
             arr[i] = temp[i];
         }
     }

    static void main(String[] args) {
        int[] arr ={1,-1,3,-4,6};
        rearrange(arr);
        System.out.println("ReArrange: " +Arrays.toString(arr));
    }
}
