    class AreaCalculator {
     double area(int radius){
     return 3.14 * radius * radius;
     }
    int area(int length, int breadth){
     return length * breadth;
     }
    double area (double base, double heigth){
     return 0.5 * base * heigth;
     }
    public static void main(String[] args){
     AreaCalculator ac = new AreaCalculator();

        System.out.println("Area of circle: " +ac.area(5));
        System.out.println("Area of rectangle: " +ac.area(4,5));
        System.out.println("Area of Triangle: " +ac.area(6.0,4.0));
     }
    }