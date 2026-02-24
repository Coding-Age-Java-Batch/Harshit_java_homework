import javax.swing.*;

public class ToggleCase {

    public static String toggleCase(String str){
        StringBuilder result = new StringBuilder();

        for(char ch : str.toCharArray()){
            if(Character.isUpperCase(ch)) {

                result.append(Character.toLowerCase(ch));
            }
           else if(Character.isLowerCase(ch)) {

                result.append(Character.toUpperCase(ch));
            }
           else{
                result.append(ch);
            }
        }
        return result.toString();
    }

    static void main(String[] args) {
        String input = "hELLO hARSHIT";
        String output = toggleCase(input);
        System.out.println(output);
    }
}
