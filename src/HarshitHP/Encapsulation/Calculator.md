public class Calculator {

    private double result;

    public Calculator(){
        result = 0;
    }
    public void add(double number){
        result = result + number;
    }

    public void subtract(double number){
        result = result - number;
    }

    public void multiply(double number){
        result = result * number;
    }

    public void divide(double number){
        if(number != 0){
            result = result / number;
        }
        else{
            System.out.println("Error: Cannot divide ny zero!");
        }
    }
    public double getResult(){
        return result;
    }
    public void clear(){
        result = 0;
    }

    static void main(String[] args) {
        Calculator calc = new Calculator();

        calc.add(10);
        calc.add(5);

        calc.multiply(2);

        calc.divide(3);

        System.out.println("Final Result: "+calc.getResult());

        calc.clear();
        System.out.println("After clear: " + calc.getResult());

        calc.add(50);
        calc.subtract(20);
        System.out.println("New Calculation Result: "+calc.getResult());
    }
}
