public class FinallyDemo {
static void main(String[] args) {

        try{
            int result = 5/0;
            System.out.println("Result: "+result);
        }
        catch(ArithmeticException e){
            System.out.println("AirthmeticException: " +e);
        }
        finally{
            System.out.println("...Execution Completed...");
        }
    }
}