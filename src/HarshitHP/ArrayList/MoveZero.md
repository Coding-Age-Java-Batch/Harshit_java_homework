import java.util.*;

public class MoveZero {

    public static void moveZero(int[] arr){

        int[] temp = new int[arr.length];
        int index = 0;

        for(int num : arr){
            if(num != 0){
                temp[index++] = num;

            }
        }

        for(int i = 0; i<arr.length; i++){
            arr[i] = temp[i];
        }
    }

public static void main(String[] args) {
int[] arr = {0,1,0,5,7};

        moveZero(arr);
        System.out.print(Arrays.toString(arr));
    }
}
