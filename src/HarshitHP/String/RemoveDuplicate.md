public class RemoveDuplicate {

    public static String removeDuplicate(String str){
        String result = "";

        for(int i =0; i < str.length(); i++){
            char ch = str.charAt(i);

            if(result.indexOf(ch) == -1){
                result = result + ch;
            }
        }
        return result;
    }

    static void main(String[] args) {
        String input = "Java Programming";

        System.out.println(removeDuplicate(input));
    }
}