public class NestedTryCatch {
static void main(String[] args) {

        try{
            System.out.println("Outer Try: Starting program");

            try{
                int result = 10/0;
                System.out.println("Result: " +result);
            }
            catch(ArithmeticException e){
                System.out.println("Inner catch: Division by zero" +e.getMessage());
            }

            int[] numbers = {1,2,3};
            System.out.println(numbers[5]);
        }
        catch(ArrayIndexOutOfBoundsException e){
            System.out.println("Invalid array index!" +e.getMessage());
        }
        catch(Exception e){
            System.out.println("Genral catch: something went wrong");
        }
        System.out.println("Tnanks for coding");
    }
}
