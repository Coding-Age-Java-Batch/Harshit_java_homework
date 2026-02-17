import java.util.*;
public class ReplaceAll {

    static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        ArrayList<Integer> list = new ArrayList<>();

        System.out.print("Enter size: ");
        int n = sc.nextInt();

        System.out.println("Enter elements: ");
        for(int i=0; i<n; i++) {
            list.add(sc.nextInt());

        }
            System.out.print("Replace with: ");
            int value = sc.nextInt();

        Collections.fill(list,value);

        System.out.println("Result: "+list);
    }
}
