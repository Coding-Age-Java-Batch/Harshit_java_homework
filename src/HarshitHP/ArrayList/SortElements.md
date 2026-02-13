import java.util.*;

public class SortElements {

    static void main(String[] args) {

        ArrayList<Integer> num = new ArrayList<>();

        num.add(33);
        num.add(44);
        num.add(99);
        num.add(55);
        num.add(11);

        Collections.sort(num);
        System.out.println("Sorted value is: "+num);

    }
}