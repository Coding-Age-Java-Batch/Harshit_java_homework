public class Palindrome {

    public static boolean isPalindrome(String str){

        int left = 0;
        int right = str.length()-1;

        while(left < right){
            char c1 = Character.toLowerCase(str.charAt(left));
            char c2 = Character.toLowerCase(str.charAt(right));

            if(c1 != c2){
                return false;
            }
            left++;
            right--;
        }
        return true;
    }

    static void main(String[] args) {
        System.out.println(isPalindrome("Level"));
        System.out.println(isPalindrome("Harshit"));
    }
}
