import java.util.*;
public class CoomonElements {
static void main(String[] args) {

        ArrayList<Integer> A = new ArrayList<>();
        A.add(1);
        A.add(2);
        A.add(3);

        ArrayList<Integer> B = new ArrayList<>();
        B.add(2);
        B.add(3);
        B.add(4);

        ArrayList<Integer> result = new ArrayList<>();

        for(int x : A){
            for(int y : B){
                if(x == y){
                    result.add(x);
                }
            }
        }
        System.out.println(result);
    }
}