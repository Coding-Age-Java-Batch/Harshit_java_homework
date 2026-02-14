import java.util.ArrayList;

public class CloneOfArray {
static void main(String[] args) {

        ArrayList<Integer> listA = new ArrayList<>();

        listA.add(10);
        listA.add(20);

        ArrayList<Integer> listB = (ArrayList<Integer>) listA.clone();

        System.out.println("List A: " +listA);
        System.out.println("List B: " +listB);

    }
}