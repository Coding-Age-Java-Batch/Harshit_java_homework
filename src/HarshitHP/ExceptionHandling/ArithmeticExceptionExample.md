import java.util.*;
public class ArithmeticExceptionExample {
static void main(String[] args) {
Scanner sc = new Scanner(System.in);

        System.out.print("Enter numerator number: ");
        int numerator = sc.nextInt();

        System.out.print("Enter denominator number: ");
        int denominator = sc.nextInt();

        try{
            int result = numerator/denominator;
            System.out.println("Result: "+result);
        }
        catch(ArithmeticException e){
            System.out.println("Number cannot divide by zero");
        }


    }
}
