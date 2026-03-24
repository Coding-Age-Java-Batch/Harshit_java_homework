public class StringRotation {

    public static boolean isRotation(String str1, String str2){

        if(str1.length() != str2.length()){
            return false;
        }
        String temp = str1 + str1;

        return temp.contains(str2);
    }

    static void main(String[] args) {
        String str1 = "abcde";
        String str2 = "deabc";

        System.out.println(isRotation(str1, str2));
    }
}
