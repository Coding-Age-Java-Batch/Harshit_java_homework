    public class Calculator {

    int add(int a, int b){
        return a + b;
    }
    int sub(int a, int b){
        return a - b;
    }
    int mul(int a, int b){
        return a*b;
    }
    int div(int a, int b){
        if(b == 0){
            System.out.println("Cannot divided by zero");
        }
        return a/b;
    }

    public static void main(String[] args){

        Calculator ca = new Calculator();

        System.out.println("Addtion " +ca.add(10,20));
        System.out.println("Subtraction " +ca.sub(29,6));
        System.out.println("Multiply " +ca.mul(20,5));
        System.out.println("divide " +ca.div(30,3));

    }

}

