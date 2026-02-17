    import java.util.*;
    public class ArrayToArrayList {
    static void main(String[] args) {
    String[] arr = {"A", "B", "C"};

        ArrayList<String> list = new ArrayList<>(Arrays.asList(arr));

        System.out.println("ArrayList = " +list);
    }
    }