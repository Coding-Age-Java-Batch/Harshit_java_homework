public class MultipleCatchExample {
static void main(String[] args) {
int[] arr = new int[5];

        try{
            int result = 10/0;
            System.out.println(arr[8]);
        }
        catch(ArithmeticException e){
            System.out.println("ERROR: Number cannot devide by zero");
        }
        catch(IndexOutOfBoundsException e){
            System.out.println("ERROR: Invalid Array Index");
        }
        System.out.println("Thanks for Coding....");
    }
}
