import java.io.FileReader;
import java.io.FileNotFoundException;

public class ExceptionDemo {
public static void main(String[] args){

        try{
            FileReader file = new FileReader("Xyz.txt");
        }
        catch(FileNotFoundException e){
            System.out.println("Checked Exception caught: " +e);
        }
        try{
            int a = 10;
            int b = 0;
            int result = a / b;
        }
        catch(ArithmeticException e){
            System.out.println("Unchecked Exception caught: "+e);
        }
    }
}
