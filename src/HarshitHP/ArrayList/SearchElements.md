import java.util.*;

public class SearchElements {
static void main(String[] args) {

        ArrayList<Integer> num = new ArrayList<>();

        num.add(10);
        num.add(22);
        num.add(33);
        num.add(44);

        if(num.contains(22)){
            System.out.println("Number in List");
        }
        else{
            System.out.println("Number is not in List");
        }
    }
}
