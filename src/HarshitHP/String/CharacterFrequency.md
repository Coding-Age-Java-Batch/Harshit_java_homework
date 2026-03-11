public class CharacterFrequecny {
public static void printFrequency(String str){
str = str.toLowerCase();
int[] freq = new int[200];

        for(int i = 0; i < str.length(); i++){
            char ch = str.charAt(i);
            freq[ch]++;
        }

        for(int i = 0; i < str.length(); i++){
            char ch = str.charAt(i);
            if(freq[ch] != 0){
                System.out.println(ch + ":" + freq[ch]);
                freq[ch] = 0;
            }
        }
    }

    static void main(String[] args) {
        printFrequency("Apple");
    }
}