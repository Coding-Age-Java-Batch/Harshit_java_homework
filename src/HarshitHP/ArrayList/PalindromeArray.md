public class PalindromeArray {

    public static boolean isPalidrome(int[] arr){

        int left = 0;
        int right = arr.length-1;

        while(left < right){
            if(arr[left] != arr[right]){
                return false;
            }
            left++;
            right--;
        }
        return true;
    }

    static void main(String[] args) {

        int[] arr = {1,2,3,2,1};

        if(isPalidrome(arr)){
            System.out.println("True (Palidrome)");
        }
        else{
            System.out.println("False (Not Palindrome)");
        }
    }
}
