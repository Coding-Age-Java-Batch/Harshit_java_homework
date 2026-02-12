    public class Shape {
    void area(){
     System.out.println("Calculate area");
    }
    }

    class Rectangle extends Shape{
    int leanth;
    int breath;
    Rectangle(int lth, int bth){
    leanth = lth;
    breath = bth;
    }
    void area(){
    int area = leanth * breath;
    System.out.println("Area of reactangle: " +area);
    }

    public static void main(String[] args){
        Rectangle r = new Rectangle(20,5);
        r.area();
    }
    }