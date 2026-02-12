    class Calculator{
    int add(int a, int b){
      return a + b;
     }
    int add(int a, int b, int c){
      return a + b + c;
     }

    public static void main(String[] args){
     Calculator cl = new Calculator();
     int sum1 = cl.add(10,20);
        System.out.println("Sum of 10 and 20 is: " + sum1);

     int sum2 = cl.add(10,20,30);
       System.out.println("Sum of 10 , 20 and 30 is: " + sum2);
     }
    }