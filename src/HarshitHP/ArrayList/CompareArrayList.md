import java.util.*;

public class CompareArrayList {
static void main(String[] args) {
ArrayList<Integer> A = new ArrayList<>();
A.add(1);
A.add(2);
A.add(3);

        ArrayList<Integer> B = new ArrayList<>();
        B.add(1);
        B.add(2);
        B.add(3);

        if(A.equals(B)){
            System.out.println("Equal");
        }
        else{
            System.out.println("Not Equal");
        }
    }
}
