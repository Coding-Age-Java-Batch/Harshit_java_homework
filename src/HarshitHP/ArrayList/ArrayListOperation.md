import java.util.ArrayList;

public class ArrayListOperations {
static void main(String[] args) {

        ArrayList<String> languages = new ArrayList<>();

        languages.add("Java");
        languages.add("Python");
        languages.add("C++");

        System.out.println("After Adding: " +languages);

        languages.remove("C++");
        System.out.println("After removing C++: " +languages);

        int index = languages.indexOf("Python");
        if(index != -1){
            languages.set(index, "Go");
        }
        System.out.println("After updating Python to Go: " +languages);
    }
}
